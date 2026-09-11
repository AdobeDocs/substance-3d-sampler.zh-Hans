---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/tools/warp.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的变形工具，将方向变形和扭曲效果应用于纹理和材料图层。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Tools > Warp
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 变形
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---


# 变形

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-warp-18-n-d.png)

**在：**&#x200B;个工具中

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

**变形滤镜**&#x200B;允许您根据生成的多个噪声来变形材料。

</td>
</tr>
</table>

## 参数

**基本参数**

* **随机植入**：\
  随机种子确定在此过滤器中使用随机性的其他参数的随机值。
* **噪声选择**：\
  选择变形所基于的噪声。 不同的噪声可以创造出不同的效果。
* **噪声比例**： 0-10\
  调整源噪声的比例。 噪声将始终平铺。
* **类型**：\
  选择用于变形材料的方法。 如果选择&#x200B;**定向翘曲**&#x200B;或&#x200B;**多定向翘曲**，将显示其他参数：
  * **变形角度**： 0-1\
    调整变形的方向
* **强度**： 0-1\
  调整变形的强度。
* **自定义噪声**：切换\
  启用以使用自定义噪声，而不是&#x200B;**噪声选择**&#x200B;下的选择。 可用参数将根据&#x200B;**自定义噪声**&#x200B;是启用还是禁用而变化。 如果启用，将显示以下参数：
  * **自定义噪声模糊**： 0-1\
    模糊自定义噪声
  * **自定义噪声**：图像/画笔\
    导入自定义噪声映射以用作变形源。
* **每个通道的变形**：切换\
  启用后，将显示其他部分，以独立控制每个通道的变形。 对于每个通道，可以使用以下参数：
  * ***频道名称***：切换\
    切换此通道是否受&#x200B;**变形筛选器**&#x200B;影响。
  * **混合模式**：\
    选择如何将此通道的变形结果与基础图层混合
  * **不透明度**： 0-1\
    更改此通道的滤镜结果的不透明度。
