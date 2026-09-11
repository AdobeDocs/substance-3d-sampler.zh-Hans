---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/scripting-and-development/create-a-plugin-with-python-and-qml.html"
breadcrumb-title: ''
description: 了解如何使用Python和QML为Substance 3D Sampler创建插件，以构建自定义用户界面和扩展功能。
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Create a Plugin with Python and QML
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 使用Python和QML创建插件
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---


# 使用Python和QML创建插件

本指南介绍如何使用Python和QML创建简单的自动保存插件。

## 增效工具结构

Sampler增效工具至少需要一个Python和QML文件才能导入，但也可包含其他文件，例如增效工具面板中用于图标的图像。 在下面的示例中，有3个文件：

* **autosave.py**&#x200B;包含插件的逻辑并确定其工作方式。
* **autosave.qml**&#x200B;定义增效工具在Sampler中的外观。
* **autosave.svg**&#x200B;是用作增效工具图标的矢量图形。

在单个文件夹中拥有增效工具所需的文件后，可通过“编辑”>“首选项”>“增效工具和脚本”将该增效工具添加到Sampler。 要了解有关管理插件的更多信息，请转到[此处](manage-installed-plugins-and-scripts.md)。

## Python

下面的代码是自动保存插件的完整python文件。 下面简要说明代码的作用，但代码中还包含带有更多信息的注释：

1. 导入相关模块。
   1. Qt是一个多平台GUI工具包。 QtcCore、QtQml和QtQuick是我们用来在autosave.py和autosave.qml之间进行通信的模块。
1. 定义每X分钟保存项目的方法&#x200B;**save()**。
1. 创建自动存储类。 此类指定&#x200B;**save()**&#x200B;方法如何连接到插件UI，以便参数可以更改插件的行为
1. 定义一个方法&#x200B;**register\_qml\_type()**&#x200B;以执行插件的设置。
1. 从Sampler中调用该插件。

### autosave.py

```
## Import QT & QML modules to create the UI

from PySide2 import QtCore, QtQml, QtQuick 

## Import Sampler API

import substance_sampler as ssa 

## Import other modules for this specific example

import datetime 

import os 

import threading 

 

 

## Save the project every X minutes

def save(interval): 

    global t 

    ssa.save_project() 

    if ssa.save_project(): 

        now = datetime.datetime.now() 

        print("Autosave: %d:%d:%d" % (now.hour, now.minute, now.second)) 

    t = threading.Timer(interval, save, [interval]) 

    t.start() 

 

 

t = None 

 

 

## Declare the API AutoSave

class AutoSave(QtQuick.QQuickItem): 

    def __init__(self, parent=None): 

        super(AutoSave, self).__init__(parent) 

 

## Declare a first API function

## This function can be called from the QML file

## with 2 arguments, one string and one integer

    @QtCore.Slot(str, int) 

    def start_auto_save(self, default_path, interval): 

        if not ssa.save_project(): 

            ssa.save_project_as(os.path.join(default_path, "autosave.ssa")) 

        global t 

        t = threading.Timer(10, save, [interval]) 

        t.start() 

        print("Launch Autosave") 

 

## Second function of the API

## With no argument

    @QtCore.Slot(None) 

    def stop_auto_save(self): 

        global t 

        t.cancel() 

        print("Stop Autosave") 

 

 

## Function to declare the API and the panel

## First argument is Python class of your API

## Second argument is name of the API you will use in the QML file

## Third and fourth is the API version. In this case, 1.0

## Last is the name of the panel in Sampler UI

def register_qml_type(): 

    QtQml.qmlRegisterType(AutoSave, "AutoSave", 1, 0, "AutoSave") 

 

 

## Execute the plugin in Sampler UI thread

ssa.run_in_main_thread(register_qml_type)
```


## QML

QML文件定义插件的UI。 QML代表Qt标记语言，其行为类似于其他标记语言，如HTML和XML。 您可以[在此处了解有关QML的更多信息](https://doc.qt.io/qt-6/qmlapplications.html#:~:text=QML%20is%20a%20user%20interface%20specification%20and%20programming,imperative%20JavaScript%20expressions%20combined%20with%20dynamic%20property%20bindings.)。

autosave.qml的一般结构如下：

1. 导入模块。
   1. 文件中使用的UI元素需要导入的Qt模块。
   1. 还导入在&#x200B;**autosave.py**&#x200B;中创建的Autosave API类。 QML文件在第20行引用此类。
1. 创建需要跟踪的变量。
   1. **autoSaveFolder**&#x200B;是将Sampler文件自动保存到的文件夹。
   1. **timing**&#x200B;是自动保存之间的时间量（秒）。
   1. 使用&#x200B;**textColor**，以便在单个位置更新插件UI中的文本颜色。
1. 实例化Python API
1. 定义用户界面。
   1. 这包括对在&#x200B;**autosave.py**&#x200B;中创建的python API的挂接。 例如：
      1. 只要更改了“自动存储间隔(min)：”元素，第47行就会更新QML文件中的&#x200B;**计时**&#x200B;变量值。
      1. 行64从API调用&#x200B;**start\_auto\_save**&#x200B;函数，并将&#x200B;**计时**&#x200B;和&#x200B;**autoSaveFolder**&#x200B;变量作为参数传递。
1. 创建用于清理默认文件路径的方法。

### autosave.qml

```
/* 

Import Qt modules to design the UI 

https://doc.qt.io/qt-5/qtqml-syntax-basics.html 

*/ 

import QtQuick 2.15 

import QtQuick.Controls 2.15 

import Qt.labs.platform 1.1 

import AutoSave 1.0 // Import API defined in the Python file 

 

Rectangle { 

  id: root 

  anchors.fill: parent 

  color: "#333333" 

 

  property var autoSaveFolder: removeQmlFilePathPrefix(StandardPaths.writableLocation(StandardPaths.DocumentsLocation)) 

  property var timing: 300 

  property var textColor: "#b3b3b3" 

 

  AutoSave { 

      id: api // Instantiate the Python API 

  } 

 

  Column { 

    id: controls 

    anchors.top: parent.top + 10 

    anchors.left: parent.left + 10 

    anchors.right: parent.right 

    width: parent.width 

    spacing: 20 

    leftPadding: 10 

    topPadding: 10 

 

    Column { 

        spacing: 5 

        Text { 

            id: timingTitle 

            text: "Autosave every (min): " 

            color: root.textColor 

        } 

        SpinBox { 

            id: timingControl 

            from: 1 

            to: 10 

            stepSize: 1 

            value: 5 

 

            onValueModified: ()=>{ 

                root.timing = timingControl.value * 60 

            } 

        } 

    } 

    Row { 

        Text { 

            text: "Off" 

            color: root.textColor 

            anchors.verticalCenter: toggle.verticalCenter 

        } 

        Switch { 

            id: toggle 

            checked: false 

 

            onClicked: ()=>{ 

                if (checked === true) { 

                    api.start_auto_save(root.autoSaveFolder, root.timing) // Call a function of the API with 2 arguments 

                } 

                else if (checked === false) { 

                    api.stop_auto_save() // Call a function of the API 

                } 

            } 

        } 

        Text { 

            text: "On" 

            color: root.textColor 

            anchors.verticalCenter: toggle.verticalCenter 

        } 

 

    } 

    Column { 

        spacing: 5 

        Text { 

            text: "Default Autosave Path" 

            color: root.textColor 

            } 

        Row { 

            id: folderInput 

            TextField { 

                id: folderText 

                text: root.autoSaveFolder 

                readOnly: true 

            } 

            Button { 

                id: folderSelection 

                text: qsTr("...") 

                width: 40 

                onClicked: ()=>{ 

                    folderDialog.open() 

                    } 

            } 

        } 

    } 

 

    FolderDialog { 

        id: folderDialog 

 

        onAccepted: ()=>{ 

            root.autoSaveFolder = removeQmlFilePathPrefix(folderDialog.currentFolder) 

        } 

    } 

 

  } 

      function qmlFilePathPrefix() { 

        if (Qt.platform.os === "windows") { 

            return "file:///" 

        } 

        return "file://" 

    } 

    function removeQmlFilePathPrefix(filePath) { 

        var prefix = qmlFilePathPrefix() 

        return filePath.toString().replace(prefix, '') 

    } 

}
```


## SVG

您可能已经注意到，**autosave.py**&#x200B;或&#x200B;**autosave.qml**&#x200B;中未明确调用或提到&#x200B;**autosave.svg**。 这是因为Sampler会查找与PY文件同名的SVG文件，并自动将其用作增效工具图标。

>[!NOTE]
>
> 如果增效工具文件夹包含的文件名与增效工具的PY文件不匹配，增效工具将不会包含图标。 这样可能会产生您的增效工具没有显示在Sampler UI中的外观。 在这种情况下，请将光标移到Sampler的右栏上以突出显示您的增效工具。
> 
> 您的浏览器不支持HTML5视频元素

如果增效工具文件夹不包含SVG文件，将改用默认增效工具图标。

以下是可用于上面创建的自动保存SVG的示例插件。

[autosave.svg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/sadoc/files/234455541/234455542/1/1662460696349/autosave.svg)

## 自动保存插件的限制

上面创建的自动保存插件功能正常，但不完美。 例如，在启用自动存储后调整自动存储间隔将不会实际更改自动存储之间的时间 — 您需要禁用并重新启用自动存储，才能将UI中的值发送到API。

如果您不熟悉如何将Python和QML结合使用，则修复此错误是一种有用的方式，有助于您了解增效工具的不同部分之间是如何进行通信的。
