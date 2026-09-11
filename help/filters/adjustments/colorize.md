---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/adjustments/colorize.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“着色”滤镜对纹理和材料应用色调和单色着色效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Colorize
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 着色
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---


# 着色

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/S_ColorFill_18_N_D.png)

**进入：**&#x200B;调整

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

着色可让您将颜色添加到通道选区，而不会丢失细节。

>[!NOTE]
>
> 虽然“着色”滤镜允许您修改正常声道，但除非您对正常声道的工作方式及其对材料的影响有清楚的了解，否则最好不要这样做。 这是一种高级功能，通常只应在特定情况下需要。

在这些图像中，**着色滤镜**&#x200B;已用于调整base color，以生成更丰富的木材材料。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0045-colorize-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0044-colorize-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 参数

**基本参数**

此部分中可用的参数根据&#x200B;**通道选择**&#x200B;而更改。

* **频道选择**：\
  选择滤镜将影响的通道。 最好在2D 视图中查看所选通道，以便直接查看滤镜的结果。
  * ***Base color/Emissive选项***
    * ***通道名称*** **— 颜色**：颜色选择\
      选择用于为通道着色的颜色
    * ***频道名称*** **— 保持明度**：切换\
      如果启用，将保留原始明亮度中的颜色值或亮度值
    * ***频道名称*** **— 强度**： 0-1\
      调整着色效果的强度。
  * ***普通通道选项***
    * **正常 — 斜率角度**： 0-90\
      修改法线的渐变
    * **法向 — 方向**： 0-360\
      调整法线脸部的方向
    * **正常 — 保持明度**：切换\
      如果启用，将保持原始法线的明度
    * **正常 — 强度**： 0-1\
      调整着色效果的强度。
* **自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D 视图中绘画自定义蒙版
  * **自定义蒙版 — 模糊**： 0-1\
    模糊蒙版
  * **自定义蒙版 — 反转**：切换\
    反转蒙版
