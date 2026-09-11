---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/adjustments/equalize.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“色调均化”滤镜，可自动重新分布亮度值并增强图像对比度。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Adjustments > Equalize
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 均衡
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---


# 均衡

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-equalize-18-n-d.png)

**进入：**&#x200B;调整

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

均衡滤镜根据距离范围调整局部对比度。 “色调均化”滤镜的目标是减少每个通道中的巨大差异。 因此，作为图像到材质(B2M)工作流程的一部分，它通常很有用 — 图像到材质（AI驱动）滤镜在滤镜中包括一个用于改进结果的均衡通道。

以下图像显示了正在使用的&#x200B;**均衡筛选器**。

![](../../assets/3d-2d-filters-cropped-0033-equalizer-in.jpg)

在添加&#x200B;**色调均化滤镜**&#x200B;之前，此材料的高度图和base color存在显着差异。

![](../../assets/3d-2d-filters-cropped-0032-equalizer-out.jpg)

添加&#x200B;**均衡滤镜**&#x200B;后，高度图和base color声道都更均匀，并且不会丢失细节。

</td>
</tr>
</table>

## 均衡滤镜教程

## 参数

<b>基本参数</b>

* <b>输入平铺</b>：切换\
  启用后，将材料视为重复平铺，因此边界附近的更改将受另一边界上的颜色值影响。
* <b>半径</b>： 0-1\
  将“色调均化”效果扩散到更广阔的区域。
* <b>颜色溢出</b>： 0-1\
  控制向周围区域渗出的颜色。
* <b>本地详细信息</b>： 0-1\
  调整“色调均化”滤镜尝试保留局部细节的方式。

<b>*频道*</b>

每个通道的控件工作方式相同。

* <b>覆盖常用参数</b>：切换\
  启用此选项可自定义此声道的均衡效果。 启用后，将显示其他控件：
  * <b>输入平铺</b>：切换\
    启用后，将材料视为重复平铺，因此边界附近的更改将受另一边界上的颜色值影响。
  * <b>半径</b>： 0-1\
    将色调均化效果扩散到更广的区域。
  * <b>保留本地差异</b>：切换\
    启用后，均衡效果可以在更高的分辨率下工作以保持细节
* <b>目标模式</b>：\
  选择如何偏移均衡效果。 默认情况下，“色调均化”会尝试将颜色向通道的平均颜色移动。 使用“参数”可改为偏向选定的颜色或值。 选择“参数”后，将显示其他控件：
  * <b>目标</b>：颜色选择\
    选择要用作“色调均化”算法目标的颜色或值。
* <b>自定颜色变化</b>： HSL滑块\
  对指定通道运行均衡算法后，调整结果的色相、色度（饱和度）和明亮度(明亮度)。

<b>蒙版</b>

* <b>自定义蒙版</b>：切换\
  启用或禁用此滤镜的自定义蒙版
* <b>自定义蒙版</b>：图像/画笔\
  选择要用作蒙版的图像，或使用画笔直接在2D 视图中绘画自定义蒙版
* <b>自定义蒙版反转</b>：切换
