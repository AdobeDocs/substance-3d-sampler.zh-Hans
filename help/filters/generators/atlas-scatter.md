---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/atlas-scatter.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的Atlas Scatter生成器，在材料表面上从纹理地图集中散点元素。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Atlas Scatter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atlas Scatter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---


# Atlas Scatter

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/S_AtlasScatter_18_N_D.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

Atlas Scatter筛选器将Atlas材料中的元素散点在底层材料上。 Atlas Scatter可用于以自然方式在材料上散布树叶、岩石或垃圾等内容。

以下图像显示了正在运行的&#x200B;**Atlas Scatter筛选器**。

![](../../assets/3d-2d-filters-cropped-0037-atlas-scatter-in.jpg)

在使用&#x200B;**Atlas Scatter滤镜**&#x200B;之前，我们有一个基本的泥浆材料 — 不是很令人兴奋。

![](../../assets/3d-2d-filters-cropped-0036-atlas-scatter-out.jpg)

通过在鹅卵石地图集中添加&#x200B;**Atlas Scatter滤镜**，材料会变得更有意思，因为鹅卵石会散布在地面上，与下面的泥浆真实地融为一体。

</td>
</tr>
</table>

## 参数

**基本参数**

* **X数量**： 1-64\
  X轴中的实例数
* **Y数量**： 1-64\
  Y轴中的实例数
* **混合模式**：\
  用于与底层图层混合的方法
* **缩放**： 0-5\
  实例规模
* **位置随机**： 0-2\
  增大或减小实例相对于网格位置的随机偏移
* **Height比例**： 0-1\
  调整实例Height
* **遵从背景**： 0-1\
  更改基础Height值对分散实例的影响程度
* **背景颜色**：
  * **色相：** 0-1\
    调整实例的色相
  * **饱和度：** 0-1\
    调整实例的饱和度
  * **值：** 0-1\
    调整实例值

**蒙版**

* **自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 启用后，将显示以下控件：
  * **自定义蒙版：**\
    选择要用作蒙版的文件，或使用画笔模式手动应用蒙版。
  * **反转蒙版：**&#x200B;切换\
    反转蒙版的值
* **蒙版随机**： 0-1\
  随机隐藏实例百分比

**大小**

* **随机缩放**： 0-1\
  应用于每个实例的随机缩放量
* **缩放无重叠**： 0-1\
  调整每个实例的缩放比例以避免实例重叠

**Height**

* **Height偏移**： -1到1\
  从基层0偏移实例Height
* **Height偏移随机**： 0-1\
  为每个实例的Height偏移量添加一个随机值
* **从背景斜率倾斜**： 0-1\
  根据背景斜率调整法线的倾斜度
* **背景Smoothness**： 0-2\
  调整背景Smoothness

**旋转**

* **旋转**： 0-1\
  按设置值旋转所有实例
* **旋转随机**： 0-1\
  为每个实例的旋转添加一个随机值
* **从背景斜率旋转**：\
  根据底层材料的斜率旋转实例

**Atlas材料调整**

* **颜色调整**：\
  调整贴图集的HSV值
* **颜色随机**：\
  为&#x200B;**颜色调整**&#x200B;中设置的HSV值添加随机性
* **从背景粗糙度**： 0-1\
  请使用背景粗糙度，而不是每个实例的粗糙度。
* **粗糙度调整**： -1到1\
  添加或删减每个实例的粗糙度值。
* **正常随机**： 0-1\
  将每个实例的法线旋转一个随机值
* **重新计算Ambient occlusion**：切换\
  如果启用，将根据修改的Ambient occlusion值重新计算Height值

**Atlas形状检测**

* **模式范围**：\
  根据职位限制图集内的可用资产。 将X和Y值保留为0，以使用地图集中的所有资源。
* **缩小贴图集不透明度**： 0-4
* **形状检测精度**：\
  选择要检测形状的算法。 不同的地图集将适用于不同的检测算法。 没有一种故障模式比其它任何一种模式的计算成本都高。
* **忽略小于**&#x200B;的形状： 0-1\
  使用此选项可避免将非常小的形状拾取为单独的元素。

使用指南

Atlas Scatter滤镜是一种在材料间散点资源（如树叶、石头或垃圾桶）的有效方法。 要使用Atlas Scatter滤镜，需要使用Atlas材料来处理滤镜。

>[!NOTE]
>
> 地图集材料是保存单独资源收藏集（或地图集）的材料。 例如，Sampler默认情况下包括干桂叶 — 这是地图集材料，因为它在一个材料中保存着一组叶子，其中每片叶子彼此分开。 Atlas Scatter节点使用一种算法将atlas材料中的每个叶作为单独的元素进行处理。

要使用Atlas Scatter过滤器，请执行以下操作：

1. 将Atlas Scatter过滤器添加到您的图层堆叠
1. 在“Atlas Scatter”图层下方，将显示一个输入槽
1. 将atlas材料拖入Atlas Scatter输入插槽

您可以通过选择散点图层，在&#x200B;**“属性”面板**&#x200B;中调整Atlas Scatter参数。

通过选择输入插槽中的材料，可在&#x200B;**“属性”面板**&#x200B;中调整贴图集材料的参数。
