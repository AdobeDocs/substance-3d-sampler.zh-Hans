---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/make-it-tile.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“为其拼贴”工具，可从非拼贴纹理自动创建无缝拼贴图案。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Make it Tile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 使其平铺
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---


# 使其平铺

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-tiling-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用&#x200B;**使其为拼贴滤镜**&#x200B;使您的素材可拼贴。 **拼贴滤镜**&#x200B;还使您的素材可拼贴，但每个滤镜的工作方式不同。 如果您发现&#x200B;**使其为拼贴滤镜**&#x200B;不起作用，请尝试&#x200B;**拼贴滤镜**。

在下图中，您可以看到&#x200B;**使其成为拼贴滤镜**&#x200B;如何将非拼贴素材转换为可拼贴素材。 这种素材拼贴效果很好，因为它遵循类似于网格的图案，没有特定的点来吸引焦点。

![](../../assets/3d-2d-filters-cropped-0015-make-it-tile-in.jpg)

在上图中，红线显示材料的边界。 很明显，焊缝很牢固，并且这种材料不平铺。

![](../../assets/3d-2d-filters-cropped-0014-make-it-tile-out.jpg)

在&#x200B;**使其成为拼贴**&#x200B;后，此素材拼贴就能够很好地拼贴，并且没有红线，因此将不可能在素材边界处看到接缝。

</td>
</tr>
</table>

## 参数

**基本参数**

* **阈值**： 0-1\
  调整顶部图层的大小和匹配。
* **Smoothness**： 0-1\
  平滑顶层接缝。
* **对比度**： 0-1\
  调整接缝的对比度。 降低对比度与模糊接缝具有相同的效果。
* **污点去除**：切换\
  如果启用，滤镜将尝试去除顶部和底部图层之间接缝附近的人为标记。
* **Color Equalizer**： 0-50\
  使颜色值色调均化以降低接缝的可见性。
* **Height匹配**：\
  更改滤镜顶部和底部图层的Height映射混合方式。 若要更清楚地查看结果，请在&#x200B;**2D视图**&#x200B;中查看Height通道。 请注意，Height匹配不会影响Height声道以外的声道，因此法线和AO不会受Height匹配更改的影响。

**高级参数**

* **色度影响**： 0-1\
  调整颜色值对接缝的影响程度。
* **蒙版反转**：切换\
  反转顶部和底部图层蒙版。
* **Height匹配Smoothness**： 0-16\
  调整顶部和底部图层之间的Height匹配模糊。
* **左/右修补程序源**： -1到1\
  调整左侧和右侧修补程序的源位置。
* **顶部/底部修补程序源**： -1到1\
  调整顶部修补程序和底部修补程序的源位置。

## 使用指南

**使其平铺****滤镜**&#x200B;的工作方式是相互叠加素材的多个副本。

下图显示了图层的布局：

* 绿色周边显示&#x200B;**使其平铺滤镜**&#x200B;生成的素材的边缘
* 红线显示底部图层的边框。 底层在X轴和Y轴上的UV空间偏移50%，因此红线是需要覆盖的拼贴接缝。
* 蓝色正方形和半圆形覆盖红色接缝。 此滤镜的参数允许您调整蓝色形状的边框，以确保红色接缝不可见，同时使蓝色接缝尽可能平滑。

![](../../assets/makeittilediagram.png){width="512px"}

左右半圆相互匹配，确保素材拼贴水平方向；上下半圆确保素材拼贴垂直方向。 中间的蓝色方块将移除所有剩余接缝，以创建一个完全可平铺的材料，没有接缝。
