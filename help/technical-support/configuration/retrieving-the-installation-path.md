---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/configuration/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: 了解如何检索Substance 3D Sampler在不同平台上的安装路径以用于脚本编写和配置目的。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 检索安装路径
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 6%

---


# 检索安装路径

本页根据版本和平台，对检索应用程序安装路径的方法进行了重新分组。

## Windows

### Creative Cloud 桌面版

1. 打开Windows注册表编辑器(**regedit**)。
1. 导航到注册表项： ** HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Paths\**
1. 打开名为&#x200B;**Adobe Substance 3D Sampler.exe**&#x200B;的子密钥
1. 密钥的值包含安装该密钥的应用程序可执行文件的路径

>[!NOTE]
>
> 此注册表项仅从版本3开始可用。\
> 对于旧版本，可从&#x200B;**HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts**&#x200B;中的文件关联检索安装路径。

### Substance 3D Standalone

1. 打开Windows注册表编辑器(**regedit**)。
1. 导航到注册表项： **HKEY\_LOCAL\_MACHINE\ SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. 查找与应用程序版本的AppID匹配的子项（请参阅下表）
1. 密钥的值包含应用程序安装位置的路径

| Version | AppId |
| --- | --- |
| **1.x (2019.x)到2.x** | {B3506E85-E98F-4D48-A010-BE4DEE27D108} |
| **3.x（或更高版本）** | {ED4A4ABC-9B7D-44B8-984A-C8A994B69CFD} |

### 蒸汽

应用程序安装在Steam安装文件夹的&#x200B;**steamapps/common/**&#x200B;子文件夹中。

## Mac

在Mac上，该应用程序安装在以下软件中：

| Version | 路径 |
| --- | --- |
| **3.x或更高版本** | **/Applications/Adobe Substance 3D Sampler.app** |
| **旧版** | **/Applications/Substance Alchemist.app** |

## Linux

在Linux上， rpm软件包安装在以下路径中：

| Version | 路径 |
| --- | --- |
| **3.x或更高版本** | **/opt/Adobe/Adobe\_Substance\_3D\_Sampler** |
| **旧版** | **/opt/Allegorithmic/Substance\_Alchemist** |
