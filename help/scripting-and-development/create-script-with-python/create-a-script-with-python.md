---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/scripting-and-development/create-a-script-with-python.html"
breadcrumb-title: ''
description: 了解如何为Substance 3D Sampler创建Python脚本以自动化工作流程和扩展应用程序功能。
helpx_creative_field: ""
helpx_description: Sampler > Scripting and Development > Create a Script with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 使用Python创建脚本
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---


# 使用Python创建脚本

本指南介绍如何使用Python创建简单的自动保存插件。

## 脚本结构

脚本需要一个PY文件才能导入到Sampler。 您可以将下面的示例脚本另存为PY文件，然后将其导入Sampler。

## 脚本示例

下面的脚本通过为素材中的每个图层选择新的随机种子，自动创建素材的变体。 这对于确保您的素材可用于一般情况而不是依赖特定的随机种子非常有用。

### random\_seed\_variations.py

```
import substance_sampler as ssa 

from random import randrange 

 

## Get the current asset loaded in the layer stack

my_asset = ssa.get_selected_asset() 

 

## Create a list of all layers of the current asset

my_asset_layers = my_asset.get_layers() 

 

## Go through the layers list

for layer in my_asset_layers: 

## Go through all parameters of each layer

    for parameter in layer.parameters: 

## if the parameter is Random Seed, change is value

        if parameter.label == "$randomseed": 

            parameter.value = randrange(10000) 

            print(f"Random Seed for layer {layer.name}: {parameter.value}") 

 
```


上述代码包括说明每行中发生情况的注释。

## 导入脚本

将上面的脚本保存为计算机上的PY文件后，可以使用“编辑”>“首选项”>“增效工具和脚本”将其导入。 导入后，**脚本**&#x200B;选项将显示在&#x200B;**文件**&#x200B;和&#x200B;**编辑**&#x200B;旁边的菜单栏中。 在此处，您可以运行脚本。

您可以在[此处](../manage-installed-plugins-and-scripts.md)了解有关管理脚本的更多信息。
