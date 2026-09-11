---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/filters/hdri-tools/hdr-merge.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的HDR合并工具，将多个曝光度图像合并为单个高动态范围图像。
helpx_creative_field: ""
helpx_description: Sampler > Filters > HDRI Tools > HDR Merge
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: HDR 合并
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---


# HDR 合并

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/S_HDRMerge_18_N_D.png)

**进入：**&#x200B;个HDRI 工具

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用&#x200B;**HDR合并** **筛选器**&#x200B;可合并SDR（标准动态范围）图像集合以创建HDR图像。

以下图像显示&#x200B;**HDR合并**&#x200B;的结果。

![](../../assets/3d-2d-filters-cropped-0027-hdr-merge-in.jpg)

在完成&#x200B;**HDR合并**&#x200B;之前，**3D视图**&#x200B;中的球面会反映默认环境光。 默认情况下，**2D 视图**&#x200B;会显示第一个扫描图像的导入图像数据，在本例中是公开率最低的图像。

![](../../assets/3d-2d-filters-cropped-0026-hdr-merge-out.jpg)

添加&#x200B;**HDR合并** **滤镜**&#x200B;后，球面会反映新环境光 — 从输入图像生成的HDR图像。

</td>
</tr>
</table>

## 参数

**基本参数**

* **输入曝光增量(EV)**： 0-2\
  设置最高和最低输入曝光之间的曝光差异。 高曝光delta将增加合并操作产生的对比度。
* **输出自动曝光**：切换\
  启用或禁用自动曝光调整。
* **输出曝光偏移(EV)**： -5至5\
  抵消曝光度。

## 使用指南

观看以了解如何使用&#x200B;**HDR合并滤镜**&#x200B;以及其他有助于将SDR图像转换为HDR环境光的滤镜。

使用&#x200B;**HDR Merge** **筛选器**&#x200B;的基本步骤如下：

1. 导入要合并到图层堆叠中的图像集。
1. 将&#x200B;**HDR合并筛选器**&#x200B;添加到图层堆叠。
1. 修改参数以确保曝光度值正确。
