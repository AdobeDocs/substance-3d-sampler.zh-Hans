---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/tools/atlas-creator.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的贴图集创建器工具，从多个图像创建纹理贴图集，以便有效地整理材质。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Atlas Creator
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atlas Creator
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---


# Atlas Creator

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-atlasgenerator-18-n-d.png)

**在：**&#x200B;个工具中

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

利用&#x200B;**地图集创建器** **滤镜**，您可以将素材和图像转换为地图集。 然后，您可以使用&#x200B;**Atlas Scatter**&#x200B;和&#x200B;**Atlas Splitter**&#x200B;等其他滤镜在素材中使用贴图集元素。

以下图像显示&#x200B;**地图集创建者**&#x200B;处理丛林绿叶之前和之后的地图集。

![](../../assets/3d-2d-filters-cropped-0041-atlas-creator-in.jpg)

在上图中，贴图集图像已导入并转换为素材，但它仍然不是贴图集素材，因为不透明度贴图不考虑单个元素。

![](../../assets/3d-2d-filters-cropped-0040-atlas-creator-out.jpg)

运行&#x200B;**贴图集创建器**&#x200B;后，将生成不透明度贴图，并且贴图集元素之间的区域将填充基本颜色通道。

</td>
</tr>
</table>

参数

**基本参数**

* **移除小形状**： 0-1

  使用此选项可调整贴图集中对象的最小大小。 这对于删除伪影很有用。
* **不透明度 — 色度影响**： 0-2

  根据颜色值微调贴图集元素的边缘。
* **添加不透明度**：图像/画笔

  导入要用作蒙版的文件或使用画笔直接在&#x200B;**2D视图**&#x200B;中绘制应不透明的区域。

使用指南

## 准备地图集图像

在使用&#x200B;**贴图集创建器滤镜**&#x200B;之前，最好确保正确准备贴图集图像。

**Atlas创建器**&#x200B;基于图像颜色工作，不考虑透明度。 这意味着，准备地图集图像的最佳方法是确保元素之间的间距是一致的黑色或白色，这使&#x200B;**地图集创建者**&#x200B;可以更轻松地生成不透明度蒙版。

## 从图像生成贴图集素材

**贴图集创建器**&#x200B;用于将贴图集图像转换为素材贴图集。

1. 将源图像导入图层栈栈。
1. 如果系统提示您选择材质创建模板，请选择“图像到材质”。 否则，对于图层栈栈中的图像，请在图像上方添加&#x200B;**图像到材质（AI驱动）滤镜**。
1. 等待&#x200B;**图像到材质**&#x200B;筛选器将源图像转换为材质。 调整参数，直到您对结果满意为止。
1. 将&#x200B;**Atlas创建器滤镜**&#x200B;添加到图层栈栈顶部。
1. 调整&#x200B;**Atlas创建器**&#x200B;的参数，直到您对结果满意为止。

1. 将图像添加到图层栈栈。 如果系统提示您选择素材创建模板，请选择&#x200B;**用作位图**。
1. 选择图像图层后，在&#x200B;**属性面板**&#x200B;中，将&#x200B;**输出用法**&#x200B;更改为&#x200B;**基色**。
1. 将&#x200B;**Atlas创建器**&#x200B;添加到图层栈栈顶部。
1. 调整&#x200B;**Atlas创建器**&#x200B;的参数，直到您对结果满意为止 — 在&#x200B;**2D视图**&#x200B;中查看不透明度通道，以更清楚地查看滤镜结果。
1. 使用&#x200B;**导出面板**&#x200B;导出生成的通道。
