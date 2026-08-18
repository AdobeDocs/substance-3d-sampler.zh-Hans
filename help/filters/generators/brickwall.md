---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/generators/brickwall.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的砖墙生成器为材质创建逼真的砖墙图案和砖石纹理。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Brickwall
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 墙砖
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---


# 墙砖

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-brickwall-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

说明墙砖滤镜会根据它下面的图层生成砖块图案。 这可用于创建砖墙（顾名思义），还可用于地板或其他任何使用砖块的地方。

在下图中，粘土材料被转换为&#x200B;**墙式滤镜**&#x200B;的砖墙。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0053-brickwall-in.jpg){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0052-brickwall-out.jpg){width="200px"}

</td>
</tr>
</table>

</td>
</tr>
</table>

## 参数

**预设**

从众多预设中进行选择，可快速模拟特定样式。

**基本参数**

* **随机植入**：随机数\
  用于确定此过滤器中其他随机值的随机值。\
  单击该数字以获取新的随机值。 选择随机值后，单击参数名称将该值重置为0。
* **砖砌砌法**：\
  根据所选样式将砖块合并在一起
* **程序块类型**：\
  选择砖的样式
* **磁贴**： 1-25\
  更改X轴和Y轴上的拼贴量。
* **偏移**： 0-1\
  修改每行砖块与前一行的偏移量。
* **使用自定颜色**：切换\
  根据所选样式将砖块合并在一起

**混合**

* **混合模式**：\
  更改砖块的组织方式。 使用&#x200B;**混合模式**&#x200B;创建第二组可以从基集独立控制的砖。\
  将&#x200B;**混合模式**&#x200B;设置为&#x200B;**无**&#x200B;后，此部分将不会显示其他参数。
* **程序块类型2**：\
  选择第二组砖块的样式。
* **Height偏移**： 0-1\
  偏移第二组砖块的Height

**水泥**

* **水泥颜色**：拾色器\
  更改砖块之间水泥的颜色。
* **水泥粗糙度**： 0-1\
  更改砖块之间水泥的粗糙度。
* **水泥间隙**： 0-1\
  更改砖块之间水泥的宽度。 更改砖块大小。
* **水泥级别**： 0-1\
  更改水泥的Height
* **水泥无序**： 0-1\
  调整水泥的平整度。 高价水泥可以升到砖之上。

**年龄**

* **砖块无序**： 0-1\
  在三维空间中随机调整每个砖块的旋转。
* **砖块散碎**： 0-1\
  在砖块中添加裂缝
* **砖形边缘**： 0-1\
  损坏砖块并破裂砖块边缘
* **砖块未卡住**： 0-1\
  随机移除砖块
* **砖色变化**： 0-1\
  改变砖块的颜色以使墙看起来不那么均匀
* **砖块污迹**： 0-1\
  向砖块添加Dirt

**高级参数**

* **Height混合强度**： 0-1\
  调整Height的混合。 值为0时忽略基础材质的Height，只使用墙式滤镜参数生成Height信息。 值1使用基础材质生成Height信息。
* **正常强度**： 0-1\
  调整墙式滤镜生成的法线的强度。 值为0实际上意味着没有法线。
* **环境遮蔽强度**： 0-1\
  调整AO的强度。 值为0有效地表示没有环境遮蔽。

使用指南

“墙砖”滤镜将底层材料分解为单独的砖块，然后重新排列。 因此，墙式滤镜最适合用于岩石或金属等硬表面 — 换言之，这些材料最适合在现实世界中用作砖。

墙式滤镜可用于创建基础材质，然后将其上的其他效果（如苔藓、雪或Dirt）图层化。
