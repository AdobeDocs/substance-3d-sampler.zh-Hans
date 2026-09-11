---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/generators/decal.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的贴花生成器为材料表面创建贴花图案和叠加纹理。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Decal
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 贴纸
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 1%

---


# 贴纸

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-decal-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

贴花滤镜允许您在特定位置添加其他素材的实例。 在添加可能不易通过流程生成的贴纸或特定细节时，此功能非常有用。

下图显示了正在使用&#x200B;**贴花滤镜**&#x200B;为混凝土添加损坏。

![](../../assets/3d-2d-filters-cropped-0045-decal-in.jpg)

加贴花前，混凝土基层干净无损。

![](../../assets/3d-2d-filters-cropped-0044-decal-out.jpg)

应用&#x200B;**贴花滤镜**&#x200B;后，会为素材添加逼真的裂缝和损坏。

</td>
</tr>
</table>

## 参数

**基本参数**

* **拼贴模式**：\
  确定是否平铺超出&#x200B;**2D视图**&#x200B;中的手柄。\
  H代表“水平”，V代表“垂直”。
* **底部素材颜色匹配**： 0-1\
  调整贴花材料的颜色以匹配其下方图层的颜色值。
* **正常混合模式**：\
  调整贴花材料和下层图层之间的法线混合方式
* **正常不透明度混合**： 0-1\
  更改贴花材料法线的不透明度
* **贴花Height位置**： 0-1\
  调整贴花相对于底层图层Height的Height
* **贴花Height比例**： 0-1\
  更改贴花素材的Height映射的对比度

**高级参数**

* **贴花变换**：\
  调整贴花的矩阵变换值。 通常，使用&#x200B;**2D 视图**&#x200B;中的手柄可以更轻松地调整贴花的变换。
* **贴花** **偏移**： -1到1\
  调整贴花的偏移量。

## 使用指南

要使用贴花滤镜，请执行以下操作：

1. 将贴花滤镜添加到您的图层堆叠
1. 贴花图层下将出现一个输入槽
1. 将贴花材料拖入贴花图层的输入槽

您可以通过选择贴花图层来调整&#x200B;**“属性”面板**&#x200B;中的滤镜参数。

您可以在&#x200B;**“属性”面板**&#x200B;中选择输入槽中的材料来调整贴花输入材料的参数。
