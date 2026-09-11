---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/end-to-end-physical-size-workflow.html"
breadcrumb-title: ''
description: 了解如何使用Substance 3D Sampler中的端到端物理尺寸工作流程来创建与现实世界规模相匹配的物理上准确的材料。
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > End to end Physical Size Workflow
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 端到端的物理尺寸工作流程
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 端到端的物理尺寸工作流程

匹配数字环境中扫描样本和图像的真实物理尺寸，以跨应用程序创建物理上准确的视觉效果。

## 导入扫描文档

1. 选择材料创建模板。
1. 选中物理尺寸复选框。

   ![](../assets/screenshot-2022-01-20-at-16-15-53.png)
1. 有两种方法可设置物理尺寸：

   3a。 单击手动测量 — 测量工具可校准样本的两个特征之间的物理尺寸。\
   在两点之间跟踪 — > enter

   ![](../assets/screenshot-2022-01-20-at-16-31-26.png)

   3b. 自动测量 — 自动测量工具允许您根据图像物理尺寸(dpi)获取样本的估计元数据。 它速度更快，但仅适用于扫描，因为它使用存储的dpi来计算精确的起始大小。

   <b>您现在可以处理扫描</b>
1. 添加裁剪并根据样本进行调整。 您可以看到更新后的2D视口右下角显示的物理尺寸。

   在2D视口中显示物理比例，以准确查看您正在处理的贴图。\
   您可以将2D 视图设置为适合物理尺寸，以便屏幕比的DPI与材料比例相匹配。 换句话说，您可以将真实样本放在屏幕旁边，以验证尺寸。

   ![](../assets/cq5dam.web.1280.png)
1. 添加“色调均化”以去掉任何渐变。
1. 添加拼贴以修正拼贴
1. 如果需要，变形变换对于仅重新对齐地图的某些部分非常有用。

   <b>准备导出</b>
1. 导出为

   选择Sbsar格式，Sampler会将物理尺寸作为元数据放入其中。 它允许其他应用程序读取和使用此信息。\
   也可以导出图像；它将尊重物理尺寸比例。

   如果您在任何时候都需要使用该物理尺寸，请使用&#x200B;*物理尺寸面板*。

   当导出为图像时，现在可以强制图像大小遵循物理尺寸比。

## 视频教程

您还可以查找视频教程，以帮助您了解此功能：
