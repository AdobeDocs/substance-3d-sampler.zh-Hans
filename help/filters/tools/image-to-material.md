---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/image-to-material.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“图像到材质”工具，通过AI驱动的处理将单个图像转换为完全PBR材质。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Image To Material
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 图像到材质
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 图像到材质

![](../../assets/sat-icon-image-to-material.png)

**图像到材质**&#x200B;模板允许从单个输入图像生成高质量的PBR材质。

此模板有两个主要算法：

* **AI支持**
* **B2M**

有关每种算法的详细说明，请参阅下文。

## 示例

以下是从单个输入图像生成的素材通道示例：

![](../../assets/sat-image-to-material.jpg){width="500px"}

## 算法

要将&#x200B;**图像到材质**&#x200B;模板的算法更改，请单击模板名称下方的下拉列表：

![](../../assets/image-to-material-algo-setting.png)

### 由AI提供支持

<b>AI Powered</b>算法使用机器学习来识别形状和对象，并准确生成、正常、Height和粗糙度地图，以及去除任何阴影或高光中的反照率。

神经网络已经接受过广泛的材料训练，比如织物、有机物、室内和室外表面。

>[!NOTE]
>
> 在高分辨率图像上计算“图像到材质”（AI支持）将需要更长的时间，我们建议在工作时使用[图层分辨率](../../interface/preferences/layer-resolution.md)系统来优化您的工作流程。

### B2M

**B2M**&#x200B;算法使用基于Substance的位图到材质方法通过过程技术生成多个通道，例如基色、法线、金属、粗糙度和环境遮蔽。

此算法可能会产生不太精确的结果，但适用于更广泛的输入图像。

## Adobe Capture

Adobe Capture移动应用程序（Android和iOS）上也提供了此功能。 您可以随时随地拍摄照片，并直接在手机上预览效果。

轻松将结果发送到Substance 3D Sampler以进行进一步编辑。

![](../../assets/capture-qr-code.gif)

>[!NOTE]
>
> 此功能仅适用于Adobe版Substance 3D Collection订阅。
