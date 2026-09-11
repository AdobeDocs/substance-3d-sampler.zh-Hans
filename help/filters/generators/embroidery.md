---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/embroidery.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的刺绣生成器为材料创建刺绣织物图案和缝合纹理。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Embroidery
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 刺绣
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# 刺绣

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-embroidery-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

“刺绣”滤镜让您可以快速将图像转换为刺绣补丁。 您可以自定义修补程序外观，并使用色彩管理工具充当多个材料的蒙版。

下图显示了正在使用的&#x200B;**刺绣滤镜**。

![](../../assets/3d-2d-filters-cropped-0035-embroidery-in.jpg)

在上图中，已导入源图像。 请注意，图像是不透明的，具有白色背景。

![](../../assets/3d-2d-filters-cropped-0034-embroidery-out.jpg)

在上图中，**刺绣滤镜**&#x200B;已添加到图层堆叠中，并且已将源图像转换为刺绣修补。 请注意，虽然源图像不透明，但&#x200B;**刺绣滤镜**&#x200B;的输出仍具有透明度。

</td>
</tr>
</table>

## Tajima刺绣增效工具

有兴趣试试Tajima刺绣增效工具？ \
在[此处](../../pipeline-and-integrations/tajima-exporter-plugin.md)了解有关它的详细信息。

## 参数

<b>基本参数</b>

* <b>随机植入</b>：\
  此过滤器中所有其他随机参数所基于的随机植入。
* <b>图像</b>：图像/蒙版\
  从系统选择图像，或绘画自定义蒙版。
* <b>颜色计数</b>： 1-8\
  刺绣滤镜将尝试将导入的图像拆分为单独的颜色 — 修改此值以更改使用的颜色数量。
* <b>密度</b>： 80-300\
  选择纤维的密度。
* <b>设计</b>：填充，轮廓，填充+轮廓，Topstitch\
  选择刺绣模式：*填充*&#x200B;填充所有颜色区域，*轮廓*&#x200B;创建颜色区域轮廓，*填充+轮廓*&#x200B;在每个颜色区域上创建两个颜色，*顶纹*&#x200B;创建颜色区域的最贴心轮廓。
* <b>填充/轮廓： </b>0-1\
  更改颜色区中纤维的分布方式。
* <b>线程</b>：\
  调整线程的Thickness和长度。
* <b>平滑区域： </b>0-1\
  平衡颜色区域并影响线程行为。
* <b>瑕疵</b>： 0-1\
  向串接添加瑕疵，以帮助分解图案

<b>颜色1</b>

使用控件单独调整每个颜色区域。

* <b>填充</b>：切换\
  使颜色区域可见或不可见。
* <b>Height</b>： \
  偏移螺纹的方向

<b>拼接完成</b>

* <b>自定颜色：</b>\
  自定义整个刺绣的颜色
* <b>粗糙度： </b>0-1\
  更改粗糙度值，让刺绣变得粗糙或光滑。
* <b>金属： </b>0-1\
  更改金属值可为串接添加金属感。
* <b>Anisotropy level： </b>0-1\
  更改Anisotropy level以突出金属感。

<b>高级</b>

* <b>正常强度</b>： 0-1\
  调整法线的强度。
* <b>Height范围：</b> 0-1\
  调整刺绣在基础材质上的Height位置。
* <b>Height位置：</b> 0-1\
  调整刺绣在基础材质上的Height位置。

## 使用指南

“刺绣”滤镜起初可能会有些混乱，但借助几个重要的参数即可快速开始为素材添加补丁。

>[!NOTE]
>
> 如果您之前使用过[织造](weave.md)滤镜，则刺绣滤镜的工作方式类似。

要使用刺绣滤镜，请执行以下操作：

1. 将刺绣滤镜添加到您的图层堆叠。
1. 使用<b>基本参数>图像</b>将图像添加到滤镜，或将图像添加到刺绣滤镜下方的图层栈栈（不在其中一个输入插槽中）。 如果未将图像添加到<b>基本参数>图像</b>，则滤镜将自动从扫描通道（如果可用）中选取图像。
1. 调整<b>基本参数>颜色计数</b>，直到色彩平衡看起来适合您的图像。 最多使用8种颜色，启用或禁用颜色以隔离所需的颜色。\
   “刺绣”滤镜最适合用于平面颜色和插图图像。
1. 调整其他参数以微调修补的外观。

可以在“刺绣”滤镜中使用透明图像，但默认情况下，这些功能也会影响材料的不透明度贴图 — 图像的透明部分也会使材料变得透明。 要使用“刺绣”滤镜创建补丁并将其放置在下方图层的顶部，请使用“贴花”滤镜。

1. 创建贴花滤镜。
1. 将“刺绣”滤镜添加到“贴花”滤镜的输入槽。
1. 按照正常步骤调整刺绣图案。

贴花图层将刺绣输入转换为贴花，因此刺绣图层的透明度将告知贴花图层如何遮盖刺绣图案。 使用贴花图层，您还可以移动素材上的图案或启用拼贴等功能。
