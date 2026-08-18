---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/delight-ai-powered.html"
breadcrumb-title: ''
description: 在Substance 3D Sampler中使用AI驱动的“消光”滤镜从图像中删除光照信息并创建中性基础材质。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Delight (AI Powered)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Delight（AI驱动）
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---


# Delight（AI驱动）

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-lightgeneric-18-n-d.png)

**在：**&#x200B;个工具中

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用“愉悦”可以从基色通道中移除光照信息。 在将图像转换为材质时，这一点非常重要，因为材质通常不应包含光照信息。 素材是解释光线应该如何与表面反应的信息集合，因此，如果已经将光线信息烘焙到不应包含光线信息的通道中，这可能会破坏素材逼真地表示表面的能力。

*A **n图像在经过**&#x200B;点光（AI驱动）滤镜**处理前后的示例。 请注意，阴影和高光已被移除，仅保留基色。*

![](../../assets/120-0-comparison.png)

以下图像显示了使用&#x200B;**点光（AI驱动）滤镜**&#x200B;处理前后的素材。

![](../../assets/3d-2d-filters-cropped-0043-delighter-in.jpg)

在上述图像中，该材料仍然包括基本颜色通道中的大量光照信息。 基色通道中不应存在砖块之间的深色阴影。

![](../../assets/3d-2d-filters-cropped-0042-delight-out.jpg)

经过此令人愉悦的滤镜后，阴影部分已去除，以创建一个物理上更精确的基本颜色通道。 尽管此示例中的结果可能不明显，但令人愉悦的图像是将图像转换为材质的重要步骤。

在源图像中，光线来自静态源，但材质需要能够处理来自任何角度的光线。 例如：如果光源图像自上而下发光，那么在不经过愉悦步骤的情况下将其转换为素材，光源图像可能会显示在自下而上发光的3D空间中。 该材质将很快显得格格不入，因为仅有一个光源时，它同时看起来像在投射来自多个光源的阴影。

</td>
</tr>
</table>

## 参数

愉悦感没有参数 — 它会自动工作。

## 使用指南

如何使用它？

将&#x200B;**Delighter滤镜**&#x200B;添加到图层栈叠的顶部。

### 何时使用它？

使用&#x200B;**图像到材质(B2M)**&#x200B;时，一旦您从图像中提取了所有通道并使材质可平铺，请使用愉悦效果从基色中删除光照信息。 **图像到材质（由AI提供支持）**&#x200B;包含令人愉悦的传递，因此您不应同时使用&#x200B;**Delighter（由AI提供支持）滤镜**。
