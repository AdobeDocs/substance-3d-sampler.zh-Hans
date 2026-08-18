---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/scripting-and-development/manage-installed-plugins-and-scripts.html"
breadcrumb-title: ''
description: 了解如何在Substance 3D Sampler中管理已安装的增效工具和脚本，以安装、修改和删除自定义扩展。
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Manage installed plugins and scripts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 管理已安装的增效工具和脚本
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---


# 管理已安装的增效工具和脚本

要安装、修改或删除插件，请使用“编辑”>“首选项”，然后选择“插件和脚本”。

![](../assets/preferences-86.png)

在增效工具和脚本面板中，您可以启用显示增效工具输出的“日志”面板。 这对于故障排除和调试非常有用。 启用后，您可以从Sampler主界面中的右侧栏打开“日志”面板。 可以像停放其他Sampler面板一样停放“日志”面板。

## 增效工具与脚本

增效工具和脚本的主要区别在于，增效工具包含脚本不包含的用户界面元素。 增效工具至少需要一个PY和一个QML文件。 QML文件定义UI元素，而PY文件定义插件的行为。 另一方面，脚本仅包含PY文件。

插件的UI元素意味着可以通过使用参数来修改插件的行为。 例如，示例的自动保存增效工具包含允许修改自动保存之间的时间的控件。 增效工具将成为Sampler界面的一部分，可以像标准Sampler面板一样停放和移动。

脚本不允许这种级别的灵活性，而是执行给定的任务。 例如，无论何时调用“导出所有”脚本，该脚本的行为始终相同。 可以从顶部菜单栏访问脚本 — 仅当将脚本添加到Sampler后，“脚本”菜单才可用。

## 管理增效工具

默认情况下，唯一可用的选项是“添加插件”。 这将打开一个文件资源管理器，您可以在其中选择要加载的PY文件。

![](../assets/manageplugins.png)

>[!NOTE]
>
> 增效工具需要PY和QML文件才能工作。 选择要导入的PY文件时，Sampler将在文件夹中搜索QML文件。 如果未找到QML文件，则加载增效工具将失败。

安装插件后，有一些选项可用：

* 通过拖动插件左侧的手柄，可以对插件重新排序。
* 使用切换开关打开或关闭插件。
* 使用每个插件右侧的菜单按钮重新加载、删除或打开插件的文件夹位置。

已安装的插件最初将显示在Sampler主界面的右侧栏中。 在这里，您可以打开、停放和移动插件面板，就像标准的Sampler面板一样。

## 管理脚本

脚本的管理方式与插件类似。

![](../assets/managescripts.png)

安装脚本后，有一些选项可用：

* 使用脚本左侧的手柄重新排序脚本。
* 使用切换开关打开或关闭脚本。
* 使用每个脚本右侧的菜单按钮删除脚本，或打开脚本的文件夹位置。
* 导入后，在&#x200B;**%\AppData\Roaming\Adobe\Adobe Substance 3D Sampler\scripts**&#x200B;中复制脚本
* 要编辑脚本，应修改由Sampler复制的脚本
