---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/perforate.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的穿孔生成器，在材质和纹理中创建穿孔图案和孔阵列。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Perforate
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 穿孔
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---


# 穿孔

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-perforation-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用“穿孔”滤镜将孔添加到素材中。

*应用&#x200B;**穿孔滤镜**&#x200B;之前和之后。*

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0007-perforate-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0006-perforate-out.jpg){width="200px"}

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
* **图案选择**：\
  选择孔的形状或选择“自定图案”以创建您自己的孔。
* **穿孔位置**：\
  选择法线和Height是退回到素材中还是从素材中脱颖而出
* **穿孔倒角大小**： 0-1\
  更改孔边上倒角的大小
* **孔大小**： 0-1\
  更改孔的大小
* **使用蒙版**：切换\
  启用&#x200B;**蒙版部分**，可以使用该部分用画笔或图像遮盖穿孔。
* **使用比例图**：切换\
  允许使用比例图。 启用后，将显示以下参数：
  * **比例图乘数**： 0-1\
    调整比例尺地图对射孔比例尺的影响程度
  * **反转比例图**：切换\
    反转比例图的值
  * **自定义比例图**：图像/画笔\
    导入图像以用作比例图，或使用画笔直接在&#x200B;**2D** **视图**&#x200B;中绘制比例图

**蒙版**

此部分仅在启用&#x200B;**基本参数>使用蒙版**&#x200B;时可见

* **反转蒙版**：
* **蒙版模糊**： 0-1\
  调整应用于蒙版的模糊
* **蒙版阈值**： 0-1\
  修改蒙版阈值。 同时使用&#x200B;**蒙版模糊**&#x200B;和&#x200B;**蒙版阈值**&#x200B;值可微调蒙版的边缘。
* **自定义蒙版**：图像/画笔\
  导入图像以用作蒙版或直接在&#x200B;**2D视图**&#x200B;中绘制您自己的蒙版

**穿孔**

* **穿孔大小**： 0-1\
  更改每个穿孔的大小 — 包括孔和倒角。
* **穿孔Y数量**： 1-64\
  调整Y轴上的穿孔数
* **穿孔X数量**： 1-64\
  调整X轴上的穿孔数
* **穿孔密度**： 0-1\
  随机蒙版穿孔
* **穿孔偏移**： 0-1\
  调整每一第二行孔的偏移量
* **穿孔颜色不透明度**： 0-1\
  调整孔穴倒角区域的颜色的透明度
* **穿孔颜色**：颜色选择\
  选择每个射孔的倒角区域的颜色
* **穿孔粗糙度**： 0-1\
  修改孔的粗糙度值
* **穿孔金属**： 0-1\
  修改射孔的金属值

**高级参数**

* **明度**： 0-1
* **对比度**： -1到1
* **色相转换**： 0-1
* **饱和度**： 0-1
* **正常强度**： -1到1\
  调整每个穿孔法线的强度
* **Height强度**： 0-1\
  调整每个射孔Height图的强度
