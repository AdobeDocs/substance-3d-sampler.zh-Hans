---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/wear-and-finish/rust.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的铁锈滤镜为金属材料和表面添加逼真的铁锈和腐蚀效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Rust
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 铁锈
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# 铁锈

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-rust-18-n-d.png)

**英寸：**&#x200B;磨损和磨光

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用&#x200B;**铁锈滤镜**&#x200B;向您的材料中添加一层被氧化的金属。

在下图中，您可以看到在添加&#x200B;**铁锈滤镜**&#x200B;之前和之后的金属材质。

![](../../assets/3d-filters-cropped-0002-rust-out.jpg){width="200px"}

</td>
</tr>
</table>

## 参数

**基本参数**

* **随机植入**：\
  随机种子确定在此过滤器中使用随机性的其他参数的随机值。
* **铁锈跨页**： 0-1\
  控制铁锈的跨页或数量。
* **边缘影响**： 0-1\
  根据曲率图调整铁锈与边缘交互的方式。
* **跨页Smoothness**： 0-1\
  增大此范围以使生锈的区域更斑点，或减小此范围以使它们更细致。
* **仅影响Metal**：切换\
  启用后，**铁锈滤镜**&#x200B;将仅影响具有大于0的金属值的区域。

**铁锈**

* **铁锈形状**：\
  更改铁锈所基于的模式。
* **铁锈强度**： 0-1\
  修改铁锈效果的强度。 增加此值会使铁锈看起来更古老且更强烈。

**剥落**

* **剥落比例**： 0-1\
  更改剥落铁锈的比例。
* **正常剥落强度**： 0-1\
  调整皮正常的可见性。
* **剥落Height强度**： 0-1\
  在Height图上调整剥落的影响。

**滴**

* **液滴强度**： 0-1\
  更改滴落效果的强度。
* **滴定方向**： 0-1\
  调整滴子的方向以适应重力或风。
* **滴长度**： 0-1\
  调整水滴从源位置延伸的距离。

**蒙版**

* **使用蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D视图中绘制自定义蒙版。
  * **自定义蒙版 — 模糊**： 0-1\
    模糊蒙版。
  * **自定义蒙版 — 反转**：切换\
    反转蒙版。
