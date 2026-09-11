---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/hdri-tools/exposure-preview.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的“曝光度预览”工具，可以在应用更改之前预览HDRI图像中的曝光度调整。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > Exposure Preview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 曝光度预览
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---


# 曝光度预览

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-exposurepreview-18-n-d.png)

**进入：**&#x200B;个HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用&#x200B;**曝光预览**&#x200B;**滤镜**，您可以快速预览曝光度值的频谱。

在下方，您可以看到&#x200B;**曝光度预览滤镜**&#x200B;的作用。

![](../../assets/3d-2d-filters-cropped-0029-exposure-preview-in.jpg)

在上图中，已创建环境光，并且HDR图像数据在&#x200B;**2D 视图**&#x200B;中可见。

![](../../assets/filters-cropped-0028-exposure-preview-out.jpg)

将&#x200B;**曝光预览** **滤镜**&#x200B;添加到图层栈栈后，新的通道 — “环境诊断”可用，可显示各种曝光下的环境光。

</td>
</tr>
</table>

## 参数

**基本参数**

* **最小曝光(EV)**： -8至8\
  设置最公开图像的曝光度。
* **最大曝光度(EV)**： -8至8\
  设置最公开图像的曝光度。

## 使用指南

**曝光度预览滤镜**&#x200B;的工作方式与其他Sampler滤镜略有不同。 此工具旨在帮助为您的环境光找到正确的曝光度，但它实际上根本不会影响环境声道 — 相反，当您将&#x200B;**曝光预览滤镜**&#x200B;添加到图层堆叠时，将可以使用另一个声道在&#x200B;**2D 视图**&#x200B;环境诊断声道中查看。

如果您查看环境诊断通道，则应该能够看到一些曝光值各异的2D环境图像实例。 调整&#x200B;**曝光预览滤镜**&#x200B;的参数以更改环境诊断通道中可见的曝光范围。
