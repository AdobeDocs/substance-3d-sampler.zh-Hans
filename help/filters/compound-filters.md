---
helpx_url: 'https://helpx.adobe.com/substance-3d-sampler/filters/compound-filters.html'
breadcrumb-title: ''
description: 了解如何在Substance 3D Sampler中创建和使用复合滤镜，以将多个滤镜组合到单个可重用的图层中。
helpx_creative_field: ''
helpx_description: Sampler > Filters > Compound Filters
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 复合滤镜
user-guide-description: ''
user-guide-title: ''
source-git-commit: dc832dc546735437051226f4e1e731b55147b3ea
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# 复合滤镜

利用此功能，您可以创建一种新类型的滤镜，这些滤镜在界面中表示为单个图层并由多个滤镜组成。

>[!NOTE]
>
> 自Substance 3D Sampler 3.1.0以来的支持

## 描述

复合筛选器是&#x200B;**.ssafilter**&#x200B;文件，它是以下文件夹的。7zip压缩文件夹：

* 使用JSON格式的说明文件： **myfilter\_name.json**
* **资源**&#x200B;文件夹包含：
  * 滤镜缩略图： icon.png
  * 外部文件依赖项

### 描述文件内容

* 名称：界面中显示的复合过滤器的标签
* ID：复合滤镜的唯一标识符
* 类别：按类别对资源进行分组时，在“资源”面板中使用的复合筛选器的类别
* 版本：用于定义复合滤镜版本的增量数字。
* Node：要使用的节点列表
* 链接：不同节点之间的连接列表

### 示例

```JSON
{ "SamplerFilter":  
 { 
 "Name": "My filter", 
 "Category": "My filter category", 
 "Id": "my_unique_id", 
 "Version": 2, 
 "Node": [ 
        { 
            "Id": "foo", 
            "InternalFilter": "Foo" 
        }, 
        { 
            "Id": "bar", 
            "File": "bar.sbsar" 
        } 
    ], 
    "Link": [ 
        { 
            "From": { "Node": "FilterInput", "Usage": "baseColor" }, 
            "To": { "Node": "foo", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "FilterInput", "Usage": "normal" }, 
            "To": { "Node": "foo", "Usage": "normal"} 
        }, 
        { 
            "From": { "Node": "foo", "Usage": "baseColor" }, 
            "To": { "Node": "bar", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "bar", "Usage": "baseColor" }, 
            "To": { "Node": "FilterOutput", "Usage": "baseColor"} 
        }, 
        { 
            "From": { "Node": "foo", "Usage": "normal" }, 
            "To": { "Node": "FilterOutput", "Usage": "normal"} 
        } 
    ] 
}}
```

## 分步创建

1. 创建新文件： **my\_new\_filter.json**
1. 定义其名称、ID、类别……
1. 定义所需的节点列表
1. 如果需要外部文件，请在&#x200B;**.json**&#x200B;旁边创建&#x200B;**资源**&#x200B;文件夹
1. 将您的文件添加到&#x200B;**资源**&#x200B;文件夹中
1. 编写节点之间的链接列表
1. 验证JSON是否有效（无拼写错误、缺少昏迷或缺少括号）
1. 如需缩略图，请在&#x200B;**资源**&#x200B;文件夹中添加图像&#x200B;**icon.png**
1. 选择&#x200B;**.json**&#x200B;文件和&#x200B;**资源**&#x200B;文件夹，然后将它们压缩为7zip

## 文档

### Version

使用版本号可以跟踪不同的小版本。 打开使用先前版本的复合滤镜完成的图层栈叠时，将显示一条通知，建议您升级到最新版本。

### 节点

节点可以引用Substance 3D Sampler的内部筛选器。 定义用于定义节点与内部筛选器&#x200B;**InternalFilter**&#x200B;的标签之间的链接的唯一标识符&#x200B;**Id**

```JSON
{ 
  "Id": "step1_identifier", 
  "InternalFilter": "Dirt" 
}
```

节点可以引用不在Substance 3D Sampler中的SBSAR文件。 定义用于定义节点与SBSAR文件的文件名&#x200B;**File**&#x200B;之间的链接的唯一标识符&#x200B;**Id**。 SBSAR文件必须位于.alchfilter文件旁边的&#x200B;**资源**&#x200B;文件夹中。

```JSON
{ 
  "Id": "step1_identifier", 
  "File": "foo.sbsar" 
}
```

>[!NOTE]
>
> **filterImg**&#x200B;和&#x200B;**filterMat**&#x200B;不能用作节点ID

### 令

链接是对两个节点如何链接并由两个元素组成的说明：

* 发件人：节点使用的用法
* 收件人：节点的使用情况输出

每个元素有3个属性：

* 节点：声明要使用的节点的&#x200B;**Id**
  * 设置复合筛选器的输入，节点ID为&#x200B;**FilterInput**
  * 设置复合图层的输出，节点ID为&#x200B;**FilterOutput**
* 用法：声明要使用的用法。 有3个选项：
  * 一次仅使用一次，并通过链接声明链接（baseColor、normal、Height、ambientOcclusion、粗糙度、金属、扩散、Specular、光泽度、镜面等级、不透明度、发射度、scan1、...）
  * 也可以指定列表[&quot;baseColor&quot;， &quot;normal&quot;]。 **From**&#x200B;列表的第一项将与&#x200B;**To**&#x200B;列表的第一项匹配。 等等……
  * 使用&#x200B;**\***可以让Substance 3D Sampler在对“从”节点和“到”节点的所有使用方式的相同使用方式之间进行匹配（不能将&#x200B;**\***与另一个链接合并，但可以在同一节点之间合并单个链接和列表链接）
* 组：如果节点的用法是同一用法的好几倍，则可以使用“组”属性选择特定的用法。 即：对于混合滤镜，要获取底部素材的baseColor，请使用&#x200B;*素材1*，要获取顶部素材的baseColor，请使用&#x200B;*素材2*

```JSON
Link between two nodes  
{ 
  "From": { "Node": "node1","Usage": "baseColor", "Group": ""}, 
  "To": { "Node": "node2", "Usage": "baseColor"} 
} 
 
Link between outputs of layers below of the compound filter and the compound filter: 
{ 
  "From": { "Node": "FilterInput", "Usage": "*" }, 
  "To": { "Node": "node1", "Usage": "*"} 
} 

Link to declare outputs of the compound filter: 
{ 
  "From": { "Node": "node1", "Usage": "*" }, 
  "To": { "Node": "FilterOutput", "Usage": "*"} 
}
```
