---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/features-and-workflows/flatten-layers.html"
breadcrumb-title: ''
description: 了解如何在Substance 3D Sampler中拼合图层以提高性能并简化图层栈栈，同时了解影响。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 拼合图层
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 1%

---


# 拼合图层

拼合图层有助于提高性能并简化图层栈栈，但务必要注意拼合图层可能会对项目产生的影响。

## “拼合图层”按钮有何作用？

拼合图层会将当前选定图层下的所有图层合并为一个图层。 生成的拼合图层具有与原始图层相同的外观，但您不能再对原始的单个图层进行调整。

### 为什么拼合图层？

每当您在图层栈栈中更改图层时，Sampler都需要重新计算该图层及其上方所有图层的输出。 每个额外的计算层意味着额外的处理时间和内存使用。 拼合多个图层可减少处理这些图层所需的时间和内存。 例如，Sampler只需处理单个图层即可，而无需重新计算10个图层。

此外，拼合图层可产生更简单的图层栈栈，更易于导航和理解。

### 何时不应拼合图层？

无法在图层栈栈中单独访问任何拼合的图层，因此您无法对拼合结果中的参数进行任何更改。 因此，如果不再需要更改这些图层的结果，则只应拼合图层。

## 拼合的图层参数

当原始图层中的参数丢失时，拼合图层会有自己的一组参数，您可以调整这些参数来控制如何使用每个生成的通道。

对于每个渠道，您可以：

* <b>输出用法</b>：更改用于输出的通道。 拼合图层时，将创建一个TIFF并为每个通道命名，而且会自动分配给该通道。
* <b>来自Alpha通道的不透明度</b>：切换不透明度是否基于Alpha通道结果。
* <b>移除</b>：移除此图层中的通道。 对于不包含有用信息的通道，此选项非常有用。 例如，最好移除全部白色不透明度通道，因为这样做可以释放内存，而不会影响视觉效果。
