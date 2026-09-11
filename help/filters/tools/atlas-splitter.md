---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/atlas-splitter.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的Atlas Splitter工具将纹理地图集拆分为单个纹理地图，以进行材料编辑。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Atlas Splitter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atlas Splitter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---


# Atlas Splitter

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-atlassplitter-18-n-d.png)

**在：**&#x200B;个工具中

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

**Atlas Splitter**&#x200B;是整理和查看地图集元素的有用工具。

以下图像显示了正在运行的&#x200B;**Atlas Splitter**。

![](../../assets/3d-2d-filters-cropped-0039-atlas-splittter-in.jpg)

上图显示了添加到图层堆叠中的地图集材料。 使用&#x200B;**Atlas Splitter**&#x200B;从地图集中选择特定元素。

![](../../assets/3d-2d-filters-cropped-0038-atlas-splitter-out.jpg)

将&#x200B;**Atlas Splitter**&#x200B;添加到图层堆叠后，可专注于单一叶子或地图集材料的任何其他元素。

</td>
</tr>
</table>

## 参数

**基本参数**

* **网格视图**：切换\
  在网格视图和元素的单个视图之间切换。 如果启用，将显示以下附加参数：
  * **网格不透明度**： 0-1\
    修改网格的不透明度
  * **网格选区不透明度**： 0-1\
    修改所选元素周围边框的不透明度
  * **自动缩放**：切换\
    切换是否缩放贴图集元素以填充每个网格方形。
* **自动裁剪**：切换\
  选择是否调整所选形状的裁剪。 如果启用，将显示其他选项：
  * **自动裁剪模式**：\
    选择如何裁剪选定元素以填充材料空间。
* **形状选区**： 1-10\
  更改所选的贴图集元素。 对于包含10个以上元素的地图库，您可以在&#x200B;**形状选区**&#x200B;值中键入一个数字以更改滑块的范围。
* **旋转**： 0-1\
  旋转元素

**高级参数**

* **小形状容差**： 0-1\
  调整要由&#x200B;**Atlas Splitter**&#x200B;选取的形状的最小大小。 这对于筛选伪影很有用
* **自动旋转**：切换\
  如果启用，元素将自动旋转以具有相似的方向。
* **缩小不透明度蒙版**： 0-4\
  调整不透明度蒙版的缩放比例。 请注意，增加此值可能会降低不透明度蒙版的品质。
* **形状检测精度**：\
  选择要使用的形状检测算法。
* **膨胀宽度**： 0-32\
  修改膨胀 — 这会将元素边框的颜色凸出到蒙版区域，以帮助避免阿特拉斯元素边缘的透明度问题。 查看&#x200B;**2D 视图**&#x200B;中的base color频道以查看结果。
* **自定义背景颜色**：切换\
  如果启用，则会显示一个控件，用于修改正常通道的背景颜色：
  * **正常背景颜色**：颜色选择\
    在材料的透明部分中选择法线通道的自定义背景色。
* **Height背景色**： 0-1\
  调整Height通道的背景色。 通常最好使Height背景与地图集元素边框的平均Height匹配，以避免元素边框处出现伪影。
