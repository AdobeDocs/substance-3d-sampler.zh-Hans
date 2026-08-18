---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/height-to-normal.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“Height到正常”工具可将Height映射转换为用于材质创建工作流程的正常映射。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Height to Normal
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 正常Height
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# 正常Height

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-heighttonormal-18-n-d.png)

**在：**&#x200B;个工具中

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

根据Height声道生成普通声道数据。

在下图中，您可以看到&#x200B;**正常筛选Height**&#x200B;正在使用。

![](../../assets/h2n-in.jpg)

在上图中，没有来自素材的正常数据。 只有Height映射可用，且显示在&#x200B;**2D视图**&#x200B;中。

![](../../assets/h2n-out.jpg)

使用&#x200B;**Height到正常筛选器**，从顶部图像中显示的Height映射生成正常数据。 由于生成的法线图，光线从第二张图像中的素材反弹得更加逼真。

</td>
</tr>
</table>

## 参数

**基本参数**

* **使用世界单位**：切换\
  更改是否使用真实世界单位测量参数。 这将修改哪些参数可用。
  * **如果启用“使用世界单位”：**
    * **表面大小（厘米）**： 0-500\
      设置UV空间的大小（以世界单位表示）
    * **深度(cm)**： 0-10\
      设置Height映射表示的距离。 如果Height映射表示较小的距离，则Height映射值之间的较大差异可能会对法线角度产生较小的影响。 如果Height映射表示很大的距离，则Height映射值之间的微小差异可以表示法线映射上的大角度。
  * **如果禁用“使用世界单位”：**
    * **强度**： 0-3\
      调整法线角度的陡度
* **合并底部标准**： 0-1\
  将现有法线映射添加到此筛选器的结果。

**蒙版**

* **自定义蒙版**：切换\
  启用或禁用自定义蒙版的使用。 如果启用，将显示以下参数：
  * **蒙版**：图像/画笔\
    选择要用作蒙版的图像，或使用画笔直接在2D视图中绘制自定义蒙版
  * **自定义蒙版 — 模糊**： 0-1\
    模糊蒙版
  * **自定义蒙版 — 反转**：切换\
    反转蒙版
