---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/generators/gravel.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的砾石生成器，为材料创建逼真的砾石和石头骨料纹理。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Gravel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 砾石
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# 砾石

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-gravel-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

“砾石”滤镜以自然的方式在材料顶部分层砾石，填充裂缝。

这些图像显示&#x200B;**砾石滤镜**&#x200B;正用于用砾石填满泥浆材料的裂缝。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0029-gravel-in.jpg)

</td>
<td style="border: 0;" valign="top">

![](../../assets/3d-filters-cropped-0028-gravel-out.jpg)

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
* **数量**： 0-1\
  更改在材料上散布的砾石量。
* **主色**：颜色选择\
  选择砾石的base color
* **辅助颜色**：颜色选择\
  选择砾石的次要颜色
* **底材料颜色匹配**： 0-1\
  调整砾石颜色受基础材料颜色影响的程度
* **启用空腔蒙版**：切换\
  启用后，砾石将填充型腔，而不会扩散到材料的较高部分。 这可以产生更逼真的砾石散布效果。
* **散布体积阈值**： 0-50\
  根据Height值调整散布的音量
* **随机蒙版**： 0-1\
  设置砾石百分比以随机遮住
* **石头大小**： 1-10\
  控制石头的大小
* **石头大小变化**： 0-1\
  控制石头大小的随机性
* **石头圆度**： 0-1\
  使石头更圆或更加angular
* **石头粗糙度**： 0-1\
  修改石头的粗糙度值
* **石头Height**： 0-1\
  修改石头的Height。 这会影响石头与地下材料的融合方式。
* **石头高程**： 0-1修改石头基程。 高程设置石头所在的地板，而Height设置石头与地板的Height。
* **石头仰角随机**： 0-1\
  将随机值添加到每块石头的高度。
* **表面Smoothness**： 0-1\
  磨平石头顶部
* **使用自定义蒙版**：切换\
  启用或禁用自定义蒙版来绘画石头位置。 仅在启用&#x200B;**“使用自定义蒙版”**&#x200B;后，才会显示以下参数。
  * **蒙版模糊**： 0-1\
    模糊已绘制蒙版的边缘
  * **自定义蒙版**：图像/画笔\
    单击画笔以绘画一个自定义蒙版，其中将会显示石头。 单击正方形以导入要用作蒙版的图像。

**高级参数**

* **表面大小（厘米）**： 0-1000\
  修改材料所表示的曲面的大小。 增大砂石的表面尺寸，即砂石的物理尺寸变大，也会相应地改变砂石的表面尺寸。
* **深度** **（厘米）**： 0-100\
  修改由高度图表示的物理深度。 深度的增加意味着石块的物理尺寸高于其他区域，因此石块的正常强度增加。
