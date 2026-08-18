---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/wear-and-finish/corrode.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的腐蚀滤镜为金属材料添加腐蚀和化学降解效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Wear and Finish > Corrode
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 腐蚀
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---


# 腐蚀

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/corrode-filter-icon.png)

**英寸：**&#x200B;磨损和磨光

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

腐蚀的滤镜模仿酸侵蚀材料、留下孔洞并损坏表面的效果。

</td>
</tr>
</table>

## 参数

**基本参数**

* **随机植入**：\
  随机种子确定在此过滤器中使用随机性的其他参数的随机值。
* **受影响的区域**：\
  选择曲面曲率如何影响滤镜效果。
* **穿孔级别**： 0-1\
  调整创建的孔数。
* **曲率位置**： 0-1\
  修改要影响的曲率范围。
* **曲率平滑**： 0-1\
  平滑曲率图。
* **损坏距离**： 0-1\
  控制腐蚀区域的损伤半径。
* **损坏强度**： 0-1\
  调整受影响区域的损坏程度。
* **Height强度**： 0-1\
  控制损坏对Height地图的影响。
* **凸出位置**：切换\
  在Height图上切换损坏的方向。 禁用后，损坏将侵蚀表面；启用后，损坏将从表面向外累积。

**蒙版**

* **使用自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D视图中绘制自定义蒙版。
  * **自定义蒙版 — 模糊**： 0-1\
    模糊蒙版。
  * **自定义蒙版 — 反转**：切换\
    反转蒙版。

**高级参数**

某些“高级参数”会影响整个材质，而不仅影响由此滤镜修改的区域。

* **明度**： 0-1\
  调整完整素材的亮度或亮度。
* **对比度**： -1到1\
  调整完整素材的反照率对比度。
* **色相转换**： 0-1\
  偏移完整素材中颜色的色相值。
* **饱和度**： 0-1\
  调整完整素材的饱和度。
* **正常强度**： 0-1\
  在法线图受&#x200B;**腐蚀滤镜**&#x200B;影响的地方调整其强度。
* **Height范围**： 0-1\
  增加完整素材的Height映射中的值范围。
* **Height位置**： 0-1\
  偏移完整材料的Height。
* **环境遮蔽强度**： 0-1\
  调整由于&#x200B;**腐蚀滤镜**&#x200B;引起的AO冲击的强度。
