---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/pavement.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的路面生成器，为材料创建逼真的路面和路面纹理。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Pavement
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 人行道
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 1%

---


# 人行道

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-pavement-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

将材料转换为人行道图案。 “路面”滤镜包括许多选项，可以快速轻松地改变图案的样式。

***路面滤镜**示例。*

</td>
</tr>
</table>

## 参数

**基本参数**

* **随机植入**：\
  随机种子确定在此过滤器中使用随机性的其他参数的随机值。
* **基础材质比例**： 0-1\
  控制每个砖块中使用的材料的比例
* **间距**： 0-1\
  修改砖块之间的空间量
* **角圆度**： 0-1\
  使砖块的角看起来或多或少是圆的。
* **边缘圆度**： 0-1\
  使砖块的边缘变平滑，使其在使用后看起来更磨损
* **倾斜强度**： 0-1\
  更改应用于每个砖块的随机倾斜的强度
* **随机仰角强度**： 0-1\
  修改砖块之间相对的Height变化。

**图案**

在&#x200B;**模式类型**&#x200B;中选择模式时，每个模式都有一组不同的可用参数。 试验各种参数以查看效果。

* **图案类型**：\
  选择要放置砖块的图案。

**联合**

* **联合** **Height**： 0-1\
  修改砖块之间的材料Height
* **关节宽度**： 0-1\
  调整砖块之间的材料与砖块边缘重叠的距离
* **关节宽度变化**： 0-1\
  调整&#x200B;**关节宽度**&#x200B;的随机性
* **联合明度**： 0-1\
  修改砖块之间材料的外观。 这可用于蒙版目的。

**高级参数**

* **表面强度**： 0-1\
  控制表面变形（如裂缝或凹陷）的法线强度。
* **表面大小（厘米）**： 0-1000\
  调整材料表示的物理尺寸
* **表面Height缩放(cm)**： 0-1000\
  更改高度图表示的物理空间
* **表面Smoothness**： 0-1\
  控制表面的变化量和细节量
* **表面波纹**： 0-1\
  通过随机修改Height和法线，向曲面添加损坏或变化
* **表面笔迹蒙版阈值**： 0-1\
  修改用于控制&#x200B;**表面笔触**&#x200B;的蒙版阈值
* **启用Scalemap**：切换\
  使用缩放映射根据砖块的位置调整字体大小
* **缩放映射强度**： 0-1\
  调整缩放映射对砖块比例的影响程度。
