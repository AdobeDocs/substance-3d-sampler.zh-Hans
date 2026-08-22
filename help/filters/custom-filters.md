---
helpx_url: 'https://helpx.adobe.com/cn/substance-3d-sampler/filters/custom-filters.html'
breadcrumb-title: ''
description: 了解如何在Substance 3D Sampler中使用自定义滤镜，通过Substance Designer滤镜和自定义效果扩展功能。
helpx_creative_field: ''
helpx_description: Sampler > Filters > Custom Filters
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 自定义筛选器
user-guide-description: ''
user-guide-title: ''
source-git-commit: dc832dc546735437051226f4e1e731b55147b3ea
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---


# 自定义筛选器

## Substance自定义过滤器

可以通过“图层栈栈”操作中的&#x200B;*导入*&#x200B;按钮，导入使用Adobe Substance 3D Designer制作的滤镜。

### 创建Substance过滤器

必须在Designer中以特定方式构建滤镜，才能在导入Sampler后正常工作。

过滤器的输入和输出节点必须定义标识符或使用方式。

>[!NOTE]
>
> 可以使用&#x200B;**用法**&#x200B;或&#x200B;**标识符**（用法具有优先级）。

#### 格式化

将过滤器导出为Substance存档文件(.SBSAR)

>[!NOTE]
>
> 您可以在Sampler中公开滤镜参数以直接控制滤镜。 了解如何[此处](https://experienceleague.adobe.com/zh-hans/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter)

#### 创建筛选器以修改图像

![](../assets/image-template.png)

| 图像名称 | 使用情况 |
| --- | --- |
| *扫描1* | **扫描1** |
| *扫描2* | **扫描2** |
| *...* | **...** |

#### 创建滤镜以修改通道

![](../assets/material-template.png)

| 频道名称 | 使用情况 |
| --- | --- |
| *基色* | **基色** |
| *扩散* | **扩散** |
| *Specular* | **Specular** |
| *Specular level* | **specularlevel** |
| *金属质感* | **金属质感** |
| *粗糙度* | **粗糙度** |
| *光泽度* | **光泽度** |
| *正常* | **正常** |
| *Height* | **Height** |
| *环境遮蔽* | **ambientOcclusion** |
| *不透明度* | **不透明度** |

>[!IMPORTANT]
>
> 为Sampler创建自定义筛选器时，需要在Substance图表中添加以下用户数据：
>
> alchemist：：type=filter；

>[!IMPORTANT]
>
> 如果您的包中有一个用于处理图像的图形（scan1到scanX）和一个用于处理素材的图形（PBR通道），则Sampler可以根据滤镜在图层栈栈中的插入位置选择正确的图形。
>
> 在“图像”图表中，添加以下用户数据：
>
> * alchemist：：type=filter；alchemist：:variation:：type=multi
>
> 在“材料”图表上，添加以下用户数据：
>
> * alchemist：：type=filter；alchemist：:variation:：type=material

### 特定参数

特定参数由应用程序进行全局管理。 它是一种在自定义滤镜中使用应用程序、项目和图层栈叠的全局参数的方法。

#### 法线贴图格式

控制应用程序上的正常格式。 在Sampler中设置为DirectX

**参数标识符**： normalformat， normal_format， $normalformat， $normal_format

#### 输入计数

当您想要修改图像（scan1到scanX）时，可以使用&#x200B;**图像计数**&#x200B;参数来使用图层栈栈中的图像数量。

* **参数标识符**： input_count
* **参数类型**： integer1

#### 材质输入

如果要在图层栈叠中显示素材槽，如Atlas Scatter或飞溅：

* 添加一组新的输入节点（“基色”、“正常”、... ）
* 背景的所有输入节点（图层栈栈中的底部素材）应位于组&#x200B;**素材1**&#x200B;中
* 要在顶部添加的第一个素材的所有输入节点应位于组&#x200B;**素材2**&#x200B;中，如果您需要多个素材槽，则等等。
* 添加材料输入参数：
  * **参数标识符**： material_input
  * **参数类型**： integer1

#### 工作流类型

如果要根据项目的工作流程显示/隐藏某些参数（“PBR金属/粗糙度”或“PBRSpecular/光泽度”），可以使用“工作流程类型”参数

**参数标识符**： workflow_type

**参数类型**： integer1，下拉列表

选项：

* 0： PBR金属/粗糙度
* 1：PBRSpecular/光泽度

![](../assets/workflow-type.jpg){width="300px"}
