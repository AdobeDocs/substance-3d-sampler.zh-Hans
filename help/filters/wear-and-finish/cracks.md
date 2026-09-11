---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/wear-and-finish/cracks.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的裂缝滤镜为材料添加逼真的裂纹图案和表面损坏效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Cracks
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 裂缝
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 1%

---


# 裂缝

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-cracks-18-n-d.png)

**英寸：**&#x200B;磨损和磨光

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用&#x200B;**裂缝筛选器**&#x200B;通过向材料添加裂缝和缝隙网络来老化并损坏文档。

**裂缝筛选器**&#x200B;应用于干净的大理石材料。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0043-cracks-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0042-cracks-out.jpg){width="200px"}

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
* **裂缝跨页**： 0-1\
  调整裂缝的扩散距离 — 这会修改裂纹宽度和长度。
* **裂缝数量**： 0-1\
  更改显示的裂缝数。

**蒙版**

* **使用自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D 视图中绘画自定义蒙版。
  * **自定义蒙版 — 反转**：切换\
    反转蒙版。

**裂缝**

* **裂缝颜色**：颜色选择\
  更改裂缝所显示的内表面的颜色。
* **粗糙度**： 0-1\
  调整裂缝的粗糙度值。
* **粗糙度不透明度**： 0-1\
  调整&#x200B;**裂缝粗糙度**&#x200B;值对粗糙度图的影响程度
* **裂缝**： 0-1\
  修改裂缝的金属值。
* **金属不透明度**： 0-1\
  调整&#x200B;**金属**&#x200B;值对金属映射的影响程度
* **Height强度**： 0-1\
  调整深度。 这会影响筛选器的高度图和法线图结果。

**高级参数**

* **正常强度**： 0-1\
  调整裂纹法线的强度。
* **Height范围**： 0-1\
  修改完整材料的Height范围。 要调整裂缝的Height，请使用&#x200B;**裂缝>裂缝Height强度**。
* **Height位置**： 0-1\
  偏移完整材料的高度图。
