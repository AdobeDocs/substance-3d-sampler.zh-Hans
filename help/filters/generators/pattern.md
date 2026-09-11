---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/generators/pattern.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的图案生成器为材料纹理创建程序化的图案和重复设计。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Pattern
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 图案
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 1%

---


# 图案

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-pattern-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

从可用选项之一中为材料添加图案，或使用图像或画笔自定义自己的图案。

***图案滤镜**&#x200B;应用于牛仔布的示例。*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0011-pattern-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0010-pattern-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 参数

<b>基本参数</b>

* <b>随机植入</b>： 0-1\
  随机种子确定在此过滤器中使用随机性的其他参数的随机值。
* <b>图案</b>：图像选择器和/或绘画\
  在纹理生成器中选择一个图案或导入一个图案
* <b>颜色模式选择</b>：仅材料或纯色\
  <b>材料</b>模式影响所有&#x200B;*PBR通道*，而<b>仅颜色</b>模式仅影响材料的&#x200B;*基色*。
* <b>颜色量</b>： 1-10\
  从图案中选择现用颜色的数量
* <b>色相</b>： 0-1\
  调整图案的色相
* <b>蒙版颜色</b> ：切换\
  根据<b>颜色量</b>，为选定的颜色添加蒙版
* <b>替换颜色： </b>切换\
  根据<b>颜色量</b>，替换选定的颜色
* <b>粗糙度</b>： 0-1\
  根据<b>粗糙度量</b>，设置所选颜色的颜色
* <b>金属</b>： 0-1\
  根据<b>粗糙度量</b>，设置所选颜色的颜色
* <b>浮雕模式</b>：切换\
  选择所选颜色的浮雕方向，取决于<b>颜色量</b>
* <b>浮雕强度： </b>0-1<b>\
  </b>根据<b>颜色量</b>，调整所选颜色的浮雕强度
* <b>浮雕距离： </b>0-1\
  根据<b>“颜色量”</b>，使所选颜色的浮雕区域拉伸和平滑
* <b>浮雕颗粒： </b>0-1\
  根据<b>颜色量</b>，以所选颜色添加颗粒
