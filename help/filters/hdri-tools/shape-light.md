---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/hdri-tools/shape-light.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“形状光照”工具将自定义形状的光源添加到HDRI环境中，以实现创意光照。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Shape Light
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 形状光照
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---


# 形状光照

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-shapelight-18-n-d.png)

**进入：**&#x200B;个HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

创建矩形或圆盘形状的光。

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
* **热点曝光(EV)**： 0-10\
  调整热点的曝光度。 热点有时可能难以或无法看到 — 在新的&#x200B;**形状光滤镜**&#x200B;中，将&#x200B;**形状温度**&#x200B;设置为1000并将&#x200B;**热点曝光** **(EV)**&#x200B;设置为10，以便查看形状中心的热点。
* **形状**：\
  设置光线的形状。

**位置**

* **热点位置**： 0-1\
  偏移热点位置
* **矩阵偏移**： -2到2\
  更改形状光线的位置。 您还可以在&#x200B;**2D视图**&#x200B;中拖动光线以调整其位置。

**形状**

* **形状曝光(EV)**： 0-10\
  调整光线的曝光
* **形状硬度**： 0-1\
  柔化光线的边缘
* **热点大小**： 0-1
* **热点衰减**： 0-1\
  调整热点边缘的柔和度。

**背景**

* **背景灰度系数**：\
  选择用于确定背景灰度系数的颜色系统。
