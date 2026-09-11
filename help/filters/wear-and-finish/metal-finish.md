---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/wear-and-finish/metal-finish.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“金属光洁度”滤镜，将各种金属表面光洁度和纹理应用于材料。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Metal Finish
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 金属光洁
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---


# 金属光洁

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/metal-finish-filter-icon.png.img.png)

**英寸：**&#x200B;磨损和磨光

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

将您的材料转换为具有多种饰面和样式的金属。

*使用&#x200B;**金属光洁度滤镜将原始金属材料转换为拉丝金属表面。***

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0023-metal-finish-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0022-metal-finish-out.jpg){width="200px"}

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
* **仅修改金属质感**：切换\
  启用后，此滤镜将限制它对金属通道的更改。
* **金属颜色模式**：\
  基于现有金属选择颜色或选择您自己的颜色。 选择&#x200B;**自定颜色**&#x200B;后，将显示以下控件：
  * **金属颜色**：颜色选择\
    为金属光洁度选择自定义颜色。
* **完成类型**：\
  选择要应用于金属的样式。 每种样式都有不同的参数，您可以通过这些参数调整其外观。 可显示下列参数：
  * **强度**： 0-1\
    调整所选光泽的强度。
  * **缩放**： 0-1\
    修改驱动所选光洁度的图案比例。
  * **粗糙度**： 0-1\
    控制金属的粗糙度值。
  * **珠子比例**： 0-1\
    适用于&#x200B;**沙着**。 设置用于创建喷砂效果的珠粒大小。
  * **磨光**： 0-1\
    可用于&#x200B;**强制转换**。 调整抛光量，该量可以平滑材料的较高部分。
  * **图案**：\
    适用于&#x200B;**磨削**。 设置磨床使用的图案。
  * **浮雕详细信息**： 0-1\
    适用于&#x200B;**Raw**。 调整正常强度。
  * **方向**： 0-1\
    适用于&#x200B;**画笔**。 更改画笔效果的方向。
  * **画笔长度**： 0-1\
    适用于&#x200B;**画笔**。 更改用于创建画笔效果的描边长度。
  * **画笔**： 0-1\
    适用于&#x200B;**已激活**。 在镀锌光漆上叠加刷过的外观。

**蒙版**

* **使用自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D 视图中绘画自定义蒙版。
  * **自定义蒙版 — 模糊**： 0-1\
    模糊蒙版。
  * **自定义蒙版 — 反转**：切换\
    反转蒙版。

**高级参数**

* **Base color**：切换\
  设置滤镜是否影响base color声道。
* **金属**：切换\
  设置金属声道是否受滤镜影响。
* **粗糙度**：切换\
  设置滤镜是否影响粗糙度声道。
* **Specular level**：切换\
  控制Specular level声道是否受滤镜影响。 如果启用，将显示其他控件：
  * **Specular level** **— 值**： 0-1\
    调整Specular声道的值。

>[!NOTE]
>
> 当前存在一个已知错误，如果在禁用控件时没有控件重新启用&#x200B;**Specular level**&#x200B;控件，该控件可能会消失。 如果您失去了&#x200B;**Specular level**&#x200B;控件但需要恢复它，您可以使用undo（在macOS上为ctrl + z或cmd + z）来撤消禁用切换功能。

* **正常**：切换\
  设置正常通道是否受滤镜影响。 如果启用，将显示其他控件：
  * **正常强度**： 0-1\
    通过滤镜调整正常修改的强度。
* **Height**：切换\
  设置滤镜是否影响Height声道。
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
* **不透明度**：切换\
  设置不透明度通道是否受滤镜影响。 如果启用，将显示其他控件：
  * **不透明度 — 值**： 0-1\
    更改素材的不透明度。
