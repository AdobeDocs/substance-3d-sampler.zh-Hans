---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/texture-generators.html"
breadcrumb-title: ''
description: 了解如何在Substance 3D Sampler中使用纹理生成器为材料创建创建程序化的纹理和图案。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 纹理生成器
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---


# 纹理生成器

![](../assets/sa_whats-new-screen_v4-3-0_generators.png)

纹理生成器使用<b>参数噪声、图案</b>和<b>邋遢</b>选项改进了材料创建控制。 生成的图像可用于蒙版或通道映射中。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../assets/Capture-decran-2024-01-31-105700.png)

</td>
<td style="border: 0;" valign="top">

纹理生成器是Substance 3D Sampler中的一种资源。 可使用“纹理生成器”图标在“资源”面板中筛选这些资源。

</td>
</tr>
</table>

## 如何使用纹理生成器

### 通道映射

在3D视图、2D 视图或图层堆叠中拖放纹理生成器，然后选择一个通道以使用它。

![](../assets/DndTexgen.gif)

将在右侧输入有纹理生成器的堆叠中创建填充滤镜。 您可以在“属性”面板中访问纹理生成器属性。

#### 滤镜

某些滤镜（如<b>镶板</b>）默认使用图案蒙版的纹理生成器。其他人则使用图像或纹理生成器，如<b>图案</b>滤镜。\
在滤镜中，可以在任何图像属性中使用纹理生成器，例如<b>自定义蒙版</b>。

滤镜可以建议要使用的生成器，当您单击图像属性时，这些生成器将显示在新的资源选取器中。

![](../assets/suggested-filter.png)

#### 教程

您将在我们的[学习页面](https://creativecloud.adobe.com/cc/learn/app/substance-3d-sampler)上找到所有Substance 3D Sampler教程。

[使用Sampler的纹理生成器设计衣料](https://creativecloud.adobe.com/cc/learn/substance-3d-sampler/web/fabric-texture-generator?locale=en)

[用Substance 3D Sampler在几分钟内材料碳纤维](https://creativecloud.adobe.com/cc/learn/substance-3d-sampler/web/create-carbon-fiber-material?locale=en)

[利用Substance 3D Sampler在几分钟内完成格子结构材料](https://creativecloud.adobe.com/cc/learn/substance-3d-sampler/web/create-plaid-fabric-material?locale=en)

## 如何创建自定义纹理生成器

您可以通过图层堆叠操作中的&#x200B;*导入*&#x200B;按钮导入使用Adobe Substance 3D Designer制作的纹理生成器。 必须在Designer中以特定方式构建这些代码，才能在Sampler中导入时正常工作。

### 类型

选择“纹理生成器”作为图形<b>类型</b>。

![](../assets/typetexgen.png)

#### 输出

筛选器的筛选器输出节点必须定义<b>标识符</b>或<b>用法</b>：

* 纹理生成器的主输出不应有任何用法。 然后，它可以被3D Sampler识别为主要输出。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../assets/patternMask.png)

</td>
<td style="border: 0;" valign="top">

![](../assets/PatternMaskusage.png)

</td>
</tr>
</table>

* 纹理生成器的<b>辅助输出</b>需要使用<b>用法</b>。\
  其组名将是主输出<b>标识符</b>。

>[!NOTE]
>
> 如果您构建自己的滤镜和纹理生成器以协同工作，我们建议根据<b>输出标识符</b>使用<b>自定义用法</b>。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../assets/patterndata2.png)

</td>
<td style="border: 0;" valign="top">

![](../assets/patterndata2usage2.png)

</td>
</tr>
</table>

>[!IMPORTANT]
>
> 如果希望自定义纹理生成器位于筛选器建议资源列表中，则需要在Substance图形中添加以下用户数据：
> 
> alchemist：：suggestedfilters=[FilterName，FilterName2]；

>[!NOTE]
>
> userdata可以与[自定义筛选器](../filters/custom-filters.md)一起使用。

#### 格式化

将过滤器导出为Substance存档文件(.sbsar)

>[!NOTE]
>
> 您可以在Sampler中公开滤镜参数以直接控制滤镜。 了解如何[此处](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter)
