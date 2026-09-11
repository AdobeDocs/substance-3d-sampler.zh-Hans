---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/wear-and-finish/moss.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的苔藓滤镜，为材料添加逼真的苔藓生长和有机表面效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Moss
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 苔藓
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---


# 苔藓

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/moss-filter-icon.png)

**英寸：**&#x200B;磨损和磨光

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用&#x200B;**苔藓滤镜**&#x200B;将苔藓和地衣添加到您的素材。 **Moss**&#x200B;使用材料的遮蔽图在裂缝和缝隙中自然生长。

下图显示了应用&#x200B;**苔藓滤镜**&#x200B;之前和之后的Dirt素材。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0021-moss-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0020-moss-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 参数

**基本参数**

* **随机植入**：\
  此过滤器中所有其他随机参数所基于的随机植入。
* **Moss全局跨页**： 0-1\
  调整材料上的苔藓覆盖范围。
* **苔藓颜色**：颜色选择\
  选择苔藓的主色。
* **辅助苔藓颜色**：颜色选择\
  选择苔藓的次要颜色。
* **Moss重新分区**：\
  选择用于应用苔藓的方法。 默认情况下，**遮蔽**&#x200B;使用材料的AO映射来应用苔藓，但其他选项将具有不同的效果。 如果选择&#x200B;**自定义** **蒙版**，则将显示&#x200B;**蒙版** **部分**。

**蒙版**

仅当在&#x200B;**基本参数>苔藓重新分区**&#x200B;下选择&#x200B;**自定义蒙版**&#x200B;时，才会显示此部分。

* **自定义蒙版 — 模糊**： 0-1\
  模糊蒙版。
* **自定义蒙版 — 反转**：切换\
  反转蒙版。
* **自定义蒙版**：图像/画笔\
  选择要用作蒙版的图像，或使用画笔直接在2D 视图中绘画自定义蒙版。

**苔藓**

此部分下的可用参数取决于在&#x200B;**基本参数>苔藓重新分区**&#x200B;下选择了哪个选项。

* **遮蔽**
  * **苔藓遮蔽传播**： 0-1\
    根据遮蔽控制苔藓的蔓延。
  * **苔藓遮蔽蒙版**： 0-1\
    使用遮蔽映射作为蒙版调整苔藓数量。
* **整体**
  * **Moss整体传播**： 0-1\
    调整显示的苔藓数量。
* **顶**
  * **顶苔藓阈值**： 0-1\
    控制用于确定是否显示苔藓的阈值。
  * **顶部苔藓角度**&#x200B;根据法线图调整苔藓应用于素材的方式。
* **全部**
  * **全部**&#x200B;包括上述&#x200B;**遮蔽**、**整体**&#x200B;和&#x200B;**顶部**&#x200B;的所有参数。

以下参数可用，与在&#x200B;**基本参数>苔藓重新分区**&#x200B;下选择的选项无关。

* **苔藓花朵大小**： 0-1\
  更改苔藓的粒度。
* **苔藓颗粒强度**： 0-1\
  调整苔藓颗粒的可见性。
* **苔藓丛大小**： 0-1\
  控制苔藓结块在一起的趋势。
* **苔藓结块锐度**： 0-1\
  调整块边缘的柔和程度。
* **苔藓结块强度**： 0-1\
  控制苔藓结块的强度。
* **苔藓羽化**： 0-1\
  调整苔藓蒙版的边缘羽化方式。
* **苔藓凹凸强度**： 0-1\
  改变苔藓的崎岖不平。
* **顶苔藓阈值**： 0-1

**技术参数**

* **正常强度**： 0-1\
  调整苔藓法线的强度。
* **环境遮蔽强度**&#x200B;控制苔藓环境遮蔽的强度。
