---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/sphere-light.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“球面光”工具将球面光源添加到HDRI环境中以实现点光源效果。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Sphere Light
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 球面光
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# 球面光

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-spherelight-18-n-d.png)

**进入：**&#x200B;个HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

为您的环境添加球面光。

</td>
</tr>
</table>

## 参数

**基本参数**

* **形状颜色模式**：\
  选择用于确定光线颜色的方法。 可用参数将基于此选择而更改。
  * **温度（开氏温度）**
    * **温度**： 1000 - 27000\
      调整光线的色温。
  * **RGB**
    * **颜色**：颜色选择\
      选择光线的颜色。
  * **图像输入**
    * **形状图像输入**：图像/画笔\
      导入要用作颜色的图像。 您可以使用画笔工具直接在&#x200B;**2D视图**&#x200B;中绘画，但使用此滤镜可能会产生无法预料的结果。
  * **示例背景**
    * 取样背景无法使新参数可用，而是将浅色基于背景值。
* **曝光(EV)**： 0-10\
  调整光线的曝光度或亮度。
* **球面半径**： 0-1\
  调整光线的大小。
* **位置模式**：\
  更改确定光源位置的方法。 **位置坐标**&#x200B;部分中的参数将根据选择而更改。

**位置坐标**

可用参数取决于为&#x200B;**基本参数>位置模式**&#x200B;所做的选择。 如果选择&#x200B;**距原点距离**，则可以使用以下参数：

* **距原点距离**： 0-20\
  调整光线到相机的距离。
* **相机位置**： 0-1\
  在X、Y和Z轴上调整相机与光线的相对位置。

如果选择&#x200B;**全球位置**，则可以使用以下参数：

* **向上矢量**：\
  改变朝上的方向。
* **球面世界位置**： -2到2\
  调整球面光在X、Y和Z轴上的位置。
* **距原点距离**： 0-20\
  调整光线到相机的距离。
* **相机位置**： 0-1\
  在X、Y和Z轴上调整相机与光线的相对位置。

**形状**

* **球面硬度**： 0-1\
  柔化或硬化球体光线的边缘
* **着色**：\
  根据实际光线的不同样式更改光线的曝光度渐变。 选择&#x200B;**着色光**&#x200B;后，将显示其他参数：
  * **着色的光世界位置**： -1到1\
    修改光源上阴影区域的位置
  * **Penumbra透明度**： 0-1\
    调整光线阴影区域的不透明度级别。

**背景**

* **背景灰度系数**：\
  选择用于确定背景灰度系数的颜色系统。
