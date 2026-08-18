---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/interface/panels/share-panel.html"
breadcrumb-title: ''
description: 了解如何使用Substance 3D Sampler中的“导出”面板将素材导出为文件或将其直接发送到其他应用程序。
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Export panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: “导出”面板
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 3%

---


# “导出”面板

在<b>导出面板</b>中，您可以将资源导出为常规文件或直接将资源发送到其他应用程序。

## 发送至...

使用“发送到……”(Send to...)选项，可直接将资源发送到系统上安装的其他应用程序。 这通常比导入和导出资源快得多。

目前，Sampler支持发送至：

* **Substance 3D Painter**：导入可在为资源添加纹理时使用的材质和环境。
* **Substance 3D Stager**：导入环境光以更改场景氛围。 仅适用于环境光照，对于材质禁用。

素材始终以SBSAR发送，环境则以EXR发送。

## 导出

单击&#x200B;**导出为……**&#x200B;以导出您当前正在处理的资源。 从左侧菜单中选择是修改“常规”设置还是“材质”设置。

### 常规设置

选择“常规”设置后，可更改材料的名称和保存位置。 您还可以切换是否为素材创建子文件夹。 在以可创建多个文件的图像格式导出时，此功能非常有用。

### 材质设置

选择“材料”设置后，可更改各种参数以控制材料的导出方式：

| 设置 | 描述 |
| --- | --- |
| 格式化 | 选择导出为SBS、SBSAR还是特定图像格式的图像集合 |
| 预设 | 选择一个预设以自动组织特定应用程序的导出。 [此处提供了有关预设的更多信息](../../getting-started/export/default-presets/default-presets.md)。 只有在选择图像格式时，预设才可用。 |
| 压缩 | 选择压缩是优先于速度还是效率<br> <ul> <li> **自动**：允许Sampler选择。 <li> **最佳**：使较小文件的压缩效率最大化。 <li> **无**：无压缩表示打开和关闭导出的文件较快，但文件较大。 </ul> |
| 解决方法 | 更改导出的分辨率。 根据所选格式<br>，此选项的显示方式不同 <ul> <li> **SBSAR/SBS**：为素材选择默认宽度和Height。 这些可以稍后更新。 <li> **图像格式**：选择&#x200B;**图层输出**，以便按照图层栈栈定义的大小导出每个地图，或选择&#x200B;**覆盖全部**，以便指定导出的宽度和Height。 |
| 材质模型 | 选择是导出为Adobe标准素材还是导出为OpenPBR素材。 选择的选项应取决于在管道中使用哪些其他应用程序。 系统将根据材质模型提供不同的渠道。 |
| 渠道 | 切换应将哪些渠道作为资源的一部分导出。 |

>[!NOTE]
>
> 有关“导出”对话框选项和其他信息（如文件格式）的详细信息，请参阅[导出文章](../../getting-started/export/export.md)及其[导出窗口](../../getting-started/export/export-window/export-window.md)子文章。

对导出设置满意后，单击&#x200B;**导出**。 您的导出将显示在导出队列中，该队列显示最近导出的列表。 单击任何导出上的文件夹图标以打开该导出的文件位置。
