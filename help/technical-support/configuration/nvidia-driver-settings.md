---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/configuration/nvidia-driver-settings.html"
breadcrumb-title: ''
description: 了解如何为Substance 3D Sampler配置NVIDIA驱动程序设置，以优化GPU性能并解决“迟缓”行为。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > NVIDIA Driver Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: NVIDIA驱动程序设置
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---


# NVIDIA驱动程序设置

如果您使用的是NVIDIA GPU，但发现性能缓慢，通常有两个原因：

1. 驱动程序缺失或不是最新版本
1. Sampler使用的GPU不正确

## 更新驱动程序

要更新NVIDIA驱动程序，请执行以下操作：

1. 转到NVIDIA的驱动程序下载页面 — <https://www.nvidia.com/Download/index.aspx?lang=en-us>
1. 选择您的GPU型号并下载驱动程序。
1. 使用下载的文件安装驱动程序。

安装最新的驱动程序后，打开Sampler以查看性能是否得到了改进。 如果性能较低，则Sampler可能使用了错误的GPU。

## 配置Sampler

要检查Sampler使用的GPU，请执行以下操作：

![](../../assets/nvidiacontrolpanel.png)

1. 打开NVIDIA控制面板。 要打开NVIDIA控制面板，请执行以下操作之一：
   1. 使用“开始”菜单搜索NVIDIA控制面板
   1. 在系统托盘中，右键单击Geforce图标，然后选择NVIDIA控制面板。
1. 在NVIDIA控制面板中，选择左侧菜单中的管理3D设置。
1. 选择程序设置选项卡。
1. 在“Select a Program to Customize（选择要自定义的程序）”下，使用下拉列表查找Sampler。
1. 如果下拉列表中未列出Sampler，请使用“添加”。
   1. 浏览以查找Sampler的安装位置（默认安装位置为&#x200B;**C：/Program Files/Adobe/Adobe Substance 3D Sampler**）。
   1. 从安装位置选择&#x200B;**Adobe Substance 3D Sampler.exe**。
1. 选择Sampler后，在“选择此计划的首选图形处理器：”下，选择“高性能NVIDIA处理器”。
1. 单击“应用”。

完成此流程后，打开Sampler以查看性能是否得到了改进。
