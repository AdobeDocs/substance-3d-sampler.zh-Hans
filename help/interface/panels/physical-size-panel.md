---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/interface/panels/physical-size-panel.html"
breadcrumb-title: ''
description: 了解如何使用Substance 3D Sampler中的“物理尺寸”面板来设置材质和纹理的真实尺寸。
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Physical Size Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 物理尺寸面板
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 13%

---


# 物理尺寸面板

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/3-2-0-cover.png)

</td>
<td width="58.30%" style="border: 0;" valign="top">

使用&#x200B;**物理尺寸面板**&#x200B;配置扫描样本和图像的真实物理尺寸。

</td>
</tr>
</table>

匹配数字环境中扫描样本和图像的真实物理尺寸，以跨应用程序创建物理上准确的视觉效果。\
通过下列工具和参数，可定义材质的物理尺寸，并在对象上应用材质时创建准确和逼真的视觉效果。

## 设置实际大小

>[!NOTE]
>
> 要设置素材的物理尺寸，需要导入图像图层。

若要计算示例/图像的物理尺寸，请启用&#x200B;**设置物理尺寸**。

### 输入图像大小

此部分允许您手动设置样本的大小，并提供自动计算物理尺寸的工具。

**参考图层：**&#x200B;参考计算物理尺寸的图像。\
**宽度(X)：**&#x200B;设置参考图层的物理宽度\
**Height(y)：**&#x200B;设置参考图层的物理Height\
**工具：**

![](../../assets/screenshot-2022-01-17-at-13-59-37.png)

使用测量诊断可以测量图像上两个点之间的距离（仅供参考）。

![](../../assets/screenshot-2022-01-17-at-14-00-06.png)

使用自动测量工具可以根据图像元数据 (dpi) 估计样本的实际大小。 这种方法仅对扫描样本准确。

![](../../assets/screenshot-2022-01-17-at-14-00-24.png)

测量工具允许您通过指定样本的两个特征之间的物理距离来校准物理尺寸。 这通常是计算样本物理尺寸的最佳方法。

### 3D 网格表面

这些工具可让您设置素材表面的外观。

**物理比例：**&#x200B;启用或禁用物理比例。 物理刻度是网格沿三个轴的圆周。\
用物理值缩放您的材质。 操作Height(Y)和深度(Z)的宽度(X)。\
**纹理拼贴：**&#x200B;设置素材拼贴

### 输出材质

帮助您使用真实生活的方面使素材的输出可视化。

**显示物理比例：**\
2D视口中的显示符合物理比例。\
**Height比例：**&#x200B;根据物理比例从3D视口设置/计算。
