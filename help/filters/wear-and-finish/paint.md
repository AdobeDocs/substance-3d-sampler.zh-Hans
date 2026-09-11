---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/wear-and-finish/paint.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的绘画滤镜为材料添加绘画图层、涂层和涂抹表面效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Paint
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 颜料
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---


# 颜料

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-paint-18-n-d.png)

**英寸：**&#x200B;磨损和磨光

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用&#x200B;**绘画滤镜**，您可以用Thickness变化的绘画图层来覆盖材料。

*上面添加了一个磨损的绘画的金属材料。*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0017-paint-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0016-paint-out.jpg){width="200px"}

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
* **颜色**：颜色选择\
  设置绘画颜色。
* **粗糙度**： 0-1\
  设置绘画所覆盖区域的粗糙度。
* **Thickness**： 0-1\
  调整颜料的粘度和Thickness。 这会影响基础Height和正常信息在绘画中的可见程度。
* **剥落**： 0-1\
  在绘画已从基础材料上剥离的位置添加修补程序。
* **颗粒**： 0-1\
  更改绘画表面的颗粒。
* **颗粒大小**： 1-5\
  调整用于创建颗粒的纹理比例。

**蒙版**

* **空腔蒙版**：切换\
  根据高度图中的型腔创建蒙版。 如果启用，将显示以下参数：
  * **空腔大小**： 0-1\
    调整用于创建空腔蒙版的Height范围。
  * **空腔强度**： 0-1\
    根据腔体深度调整蒙版的不透明度。
  * **空腔反转蒙版**：切换\
    反转腔蒙版以更改它影响高点还是低点。
* **使用自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D 视图中绘画自定义蒙版。
  * **自定义蒙版 — 模糊**： 0-1\
    模糊蒙版。
  * **自定义蒙版 — 反转**：切换\
    反转蒙版。

**高级参数**

* **基色**：切换\
  设置滤镜是否影响base color声道。
* **金属**：切换\
  设置金属色通道是否受滤镜影响。
  * **金属值**： 0-1\
    调整绘画区域的金属色值。
* **粗糙度**：切换\
  设置滤镜是否影响粗糙度声道。
* **正常**：切换\
  设置正常通道是否受滤镜影响。 如果启用，将显示其他控件：
  * **正常 — 强度**： -1到1\
    调整法线的强度。
* **Height**：切换\
  设置滤镜是否影响Height声道。 如果启用，将显示其他控件：
  * **Height — 强度**： 0-1\
    调整高度图的对比度。
* **不透明度**：切换\
  设置不透明度通道是否受滤镜影响。 如果启用，将显示其他控件：
  * **不透明度 — 值**： 0-1\
    更改素材的不透明度。
* **Emissive**：切换\
  设置滤镜是否影响emissive声道。 如果启用，将显示其他控件：
  * **Emissive — 颜色**：颜色选择\
    设置emissive通道的颜色。
* **Ambient occlusion**：切换\
  设置滤镜是否影响ambient occlusion声道。 如果启用，将显示以下其他控件：
  * **Ambient occlusion — 强度**： 0-1\
    调整生成的AO的强度。
  * **环境遮蔽** **- Radius**： 0-1\
    调整AO效果的半径。
