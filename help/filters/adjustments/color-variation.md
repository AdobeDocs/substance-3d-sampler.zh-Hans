---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/adjustments/color-variation.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“颜色变化”滤镜为纹理添加颜色多样性和变化，以实现更自然的材料。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Color Variation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 颜色变化
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---


# 颜色变化

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-colorpalette-18-n-d.png)

**进入：**&#x200B;调整

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

“颜色变化”滤镜允许您一次替换base color或扩散通道中的多种颜色。 这类似于&#x200B;**颜色替换滤镜**，但是&#x200B;**颜色变化**&#x200B;允许您在一个滤镜中调整多个颜色，而&#x200B;**颜色替换**&#x200B;使您可以更好地控制用于替换颜色的蒙版，并且可以在多个通道上使用。

在下图中，**颜色变化滤镜**&#x200B;不仅用于调整基础白色以使其呈现淡蓝绿色，还用于增加许多较小斑点的对比度。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0047-color-variation-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0046-color-variation-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 参数

**基本参数**

* **颜色计数**： 1-10\
  修改将替换通道颜色的颜色数
* **明度变化**： 0-1\
  调整亮度值受替换颜色影响的程度
* **分段**：\
  基于用于在不同通道上应用颜色的蒙版。
* **颜色选择模式**：\
  选择是手动还是自动选择源颜色。 如果选择&#x200B;**手动**&#x200B;选择模式，请使用&#x200B;**2D 视图**&#x200B;中的手柄选择颜色。
  * **显示文本助手**：切换\
    此控件仅在&#x200B;**颜色选择模式**&#x200B;设置为&#x200B;**手动**&#x200B;时可见。 启用后，**显示文本助手**&#x200B;会将文本标签添加到&#x200B;**2D 视图**&#x200B;中的手柄，以便更轻松地区分颜色选择手柄
* **颜色X**：颜色选择\
  可用的颜色控件数量取决于与&#x200B;**颜色计数**&#x200B;一起选择的值。 对于每个颜色，选择新颜色以替换原始材料颜色。

## 使用指南

使用&#x200B;**颜色变化滤镜**，您可以一次快速修改base color通道的多种颜色。 对于某些材料，这对于进行较小的调整可能非常有用，但&#x200B;**颜色变化滤镜**&#x200B;最适合用单个滤镜完全彻底改变材料的颜色。

若要使用&#x200B;**颜色变化滤镜**：

1. 将&#x200B;**颜色变化滤镜**&#x200B;添加到图层堆叠
1. 调整要替换为&#x200B;**颜色计数**&#x200B;的颜色数。 此滤镜将替换通道的所有颜色 — **颜色计数**&#x200B;控件允许您设置现有颜色将被替换的新颜色数。
1. （可选）选择一个&#x200B;**分段**&#x200B;或另一个通道作为颜色的基础。 例如，您可以选择金属通道，然后使用&#x200B;**颜色选择模式>手动**&#x200B;将一个手柄放在黑金属值上，将另一个手柄放在白金属值上。 通过此设置，可以单独控制金属和非金属部分的颜色。
1. 选择&#x200B;**颜色选择模式**。 选中手动模式后，**2D 视图**&#x200B;中会显示手柄，可让您选择新颜色将替换的原始base color。 启用&#x200B;**显示文本助手**&#x200B;以跟踪哪个手柄链接到哪种颜色。
1. 使用&#x200B;**颜色1 - 10**&#x200B;控件修改颜色值。
1. 调整&#x200B;**明度变化**&#x200B;以调整明度受颜色替换影响的程度。 通过低&#x200B;**明度变化**，您可以完全拼合材料的颜色，或使用高&#x200B;**明度变化**&#x200B;来保持原始颜色的细节。
