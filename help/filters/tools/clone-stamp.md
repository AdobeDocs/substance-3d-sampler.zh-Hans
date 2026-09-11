---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/clone-stamp.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的仿制图章工具来仿制和绘画纹理区域，以便无缝地编辑和修复材料。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Clone Stamp
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 仿制图章
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# 仿制图章

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-clonestamp-18-n-d.png)

**在：**&#x200B;个工具中

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

**仿制图章工具**&#x200B;可帮助您手动复制或修补材料的各个部分。 这对于修复接缝或删除材料中的错误非常有用。**仿制图章滤镜**&#x200B;是左侧边栏中可用的工具之一。

以下图像显示了正在使用&#x200B;**仿制图章**&#x200B;从雪材料中清除碎片。

![](../../assets/3d-2d-filters-cropped-0049-clone-stamp-in.jpg)

在上图中，雪的材料包括许多树枝和其他散落的碎屑。

![](../../assets/3d-2d-filters-cropped-0048-clone-stamp-out.jpg)

**仿制图章**&#x200B;工具用于移除一些细枝并将它们替换为干净的雪。

</td>
</tr>
</table>

## 仿制图章教程

## 参数

<b>基本参数</b>

* <b>展开蒙版</b>： 0-1\
  调整滤镜将尝试匹配下层材料的绘画区域周围的距离。
* <b>渐隐混合</b>： 0-1\
  柔化仿制区域的边缘，以帮助与基础材料融合。
* <b>模糊蒙版</b>： 0-1\
  调整仿制图章边缘的细节量。 增加此值将使克隆区域的边缘变得更类似斑点。
* <b>保持比例</b>：切换\
  关闭后，允许您调整盖章区域的比例。
  * <b>水平</b>： 0-2
  * <b>垂直</b>： 0-2
* <b>旋转</b>： -180到180\
  旋转盖章区域。
* <b>水平翻转</b>：切换\
  沿水平轴镜像压印区域。
* <b>垂直翻转</b>：切换\
  沿垂直轴镜像压印区域。

<b>渐隐混合</b>

使用渐隐混合控件可单独调整材料中每个声道的渐隐混合。

<b>高级</b>

* <b>正常强度</b>： 0-2\
  调整图章区域的法线强度。
* <b>源位置</b>： \
  0-1：调整水平源位置。\
  0-1：调整垂直源位置。
* <b>目标位置</b>：\
  0-1：调整水平目标位置。\
  0-1：调整垂直目标位置。
* <b>拼贴模式</b>：下拉菜单\
  启用或禁用拼贴。

## 使用指南

单击&#x200B;**仿制图章工具**，在图层堆叠顶部创建一个新的仿制图章滤镜图层。 您还可以使用&#x200B;**图层面板**&#x200B;中的&#x200B;**添加图层按钮**&#x200B;添加仿制图章滤镜。

创建仿制图章滤镜图层将自动打开&#x200B;**视口**&#x200B;中的&#x200B;**2D 视图**。 选择“仿制图章”图层后，**工具栏**&#x200B;会显示在&#x200B;**2D 视图**&#x200B;的顶部。

![](../../assets/alchemist-2020-2-clone.gif){width="300px"}

要开始使用仿制图章工具，请单击并拖动&#x200B;**2D 视图**&#x200B;中有问题的区域。 材料将开始根据源自动更新。 使用&#x200B;**仿制图章工具**&#x200B;的区域将突出显示。

## 工具栏

<table>
<tr style="border: 0;">
<td width="16.67%" style="border: 0;" valign="top">

![](../../assets/CloneStampBrushToolbar.png)

</td>
<td width="83.33%" style="border: 0;" valign="top">

选择仿制图章图层后，2D 视图中会显示一个工具栏，其中包含其他控件。

* 选择<b>画笔工具</b>以添加到蒙版，或选择<b>擦除工具</b>以从蒙版中移除。
* 设置当前所选工具的大小。
* 访问其他控件：
  * <b>画笔拼贴</b>： \
    切换X和Y画笔拼贴。
  * <b>叠加：</b>\
    将鼠标悬停在2D 视图上时切换是否显示叠加。
* 查看2D 视图控件。

</td>
</tr>
</table>

>[!NOTE]
>
> 与其他视口工具栏一样，您可以拖动工具栏顶部的手柄以在视口内重新定位工具栏，双击手柄在垂直和水平模式之间切换，或使用双V形来隐藏或扩展工具栏。

## 源选择

在2D 视图中按住Ctrl键并单击，以添加新源。 添加新源将在<b>图层面板</b>的仿制图章图层下创建额外的图章。 您可以单独控制每个图章。

>[!NOTE]
>
> 通常最好尽量避免让源点靠近要仿制的区域。 如果源点靠近有问题的区域，则可以仿制有问题的区域。

## Shortcuts

| 操作 | Windows + Linux | MacOs |
| --- | --- | --- |
| 增加画笔大小 | &rbrack;或Ctrl +鼠标滚轮 | &rbrack;或Cmd +鼠标滚轮 |
| 减小画笔大小 | &lbrack;或Ctrl +鼠标滚轮 | &lbrack;或Cmd +鼠标滚轮 |
| 设置源 | Ctrl +左键单击 | Cmd +左键单击 |
