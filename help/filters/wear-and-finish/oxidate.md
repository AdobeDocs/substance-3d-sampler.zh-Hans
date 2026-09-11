---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/oxidate.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“Oxidate”（氧化）滤镜，为陈旧的金属外观材料添加氧化和褪色效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Oxidate
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 氧化
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# 氧化

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-oxidate-18-n-d.png)

**英寸：**&#x200B;磨损和磨光

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

在素材顶部添加一层氧化层。*应用了&#x200B;**氧化滤镜**的褶皱表面。*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0019-oxidate-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0018-oxidate-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 参数

**基本参数**

* **随机植入**：\
  随机种子确定在此过滤器中使用随机性的其他参数的随机值。
* **目标区域**：切换\
  启用以更改在材料上应用氧化效果的方式。 启用后，将显示以下控件：
  * **目标区域强度**： 0-1\
    调整目标区域效果的扩散。
  * **正在分配**： 0-1\
    调整氧化性跨页的距离。
* **颜色**：颜色选择\
  选择滤镜的base color。 这些base color会修改构成氧化效果的所有颜色的色相。
* **颜色变化**： 0-1\
  调整颜色变化效果的缩放比例。
* **密度**： 0-1\
  更改效果的覆盖密度。
* **边缘出血**： 0-1\
  修改氧化效果边缘渗入非氧化区域的方式。
* **修补程序**： 0-1\
  这是一个单独的控件，用于修改氧化区域和非氧化区域之间的蒙版。 将其与密度和其他控件相结合，以微调被氧化区域的边缘。
* **碎片**： 0-1\
  将氧化区域切掉，以显示底层材料。
* **污渍**： 0-1\
  调整材料顶部的染色量。
* **腐蚀粗糙度**： 0-1\
  调整氧化区域的粗糙度。
* **腐蚀金属**： 0-1\
  调整被氧化区域的金属值。
* **强度**： 0-1

**蒙版**

* **使用自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D 视图中绘画自定义蒙版。
  * **自定义蒙版 — 模糊**： 0-1\
    模糊蒙版。
  * **自定义蒙版 — 反转**：切换\
    反转蒙版。
  * **自定义蒙版不透明度**： 0-1\
    调整蒙版的不透明度。

**技术参数**

以下参数允许您为整个材料调整命名值，而无需添加调整图层，例如&#x200B;**亮度/对比度**&#x200B;或&#x200B;**色相/饱和度**

* **明度**： 0-1
* **对比度**： -1到1
* **色相转换**： 0-1
* **饱和度**： 0-1
* **正常强度**： 0-1
* **Height范围**： 0-1
* **Height位置**： 0-1
* **Ambient occlusion强度**： 0-1
