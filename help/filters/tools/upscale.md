---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/upscale.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“放大”工具，通过AI支持的放大技术提高纹理分辨率。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 放大
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 2%

---


# 放大

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![筛选图标](../../assets/SAPR_SuperResolution_18_N_D.png)

**在：**&#x200B;个工具中

</td>
<td style="border: 0;" valign="top">

## 描述

<b>放大</b>滤镜使用AI从它下面的图层上放大PBR通道（基色、粗糙度、正常、金属、Height）的样本。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">



</td>
<td style="border: 0;" valign="top">

![](../../assets/F5W_vAHaYAQLsz7.jpg)

</td>
</tr>
</table>

在本例中，我们首先使用1024x1024px图像，但输出结果是4098x4098px。 使用<b>放大</b>筛选器的结果定义得更多。

</td>
<td style="border: 0;" valign="top">

>[!NOTE]
>
> **高级筛选器**
> 
> <b>放大</b>是高级筛选器。\
> 要在最大容量下使用它并避免结果模糊，我们建议在“图层输入最大值”或“图层输入最小值”中将图层设置为<b>放大</b>以下。
> 
> 可以使用多少<b>个放大</b>滤镜没有限制，但高于8k分辨率的放大取样可能会显着影响性能。

</td>
</tr>
</table>

## 参数

<b>基本参数</b>

* <b>向上示例</b>：切换按钮组\
  选择要放大的乘法系数

## 操作方法

![](../../assets/SAPR_Upscale_screen_001.png)

在上图中，[图像到材质（AI驱动）](image-to-material.md)处理了低分辨率图像。

![](../../assets/SAPR_Upscale_Screen_003.png)

已添加<b>放大</b>筛选器以对结果进行放大取样。 它对细节进行卤化处理，以达到较高的分辨率来保持材料的质量。 您可以在属性中选择以2为单位或以4为单位增加像素取样。
