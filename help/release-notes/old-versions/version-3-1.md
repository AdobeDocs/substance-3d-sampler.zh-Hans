---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/release-notes/old-versions/version-3-1.html"
breadcrumb-title: ''
description: 查看Substance 3D Sampler版本3.1的发行说明，了解拾色器、SVG支持以及互操作性改进。
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 3.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本3.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 0%

---


# 版本3.1

Adobe Substance 3D Sampler 3.1引入了新的拾色器，支持SVG文件，并改进了与Stager、Photoshop和Illustrator的互操作性。

发行日期：*2021年9月28日*

## 主要功能

### 拾色器

此版本添加了一个新的[拾色器](../../interface/tools-and-widgets/color-picker.md)，其中包括吸管和对色板的支持。

需要选择颜色时就会显示拾色器。 它可以在屏幕上的任何位置移动。

![](../../assets/color-picker-raw.png){width="250px"}

### SVG支持

Sampler现在支持SVG文件。 可将它们导入到您的资源中，直接导入到图层堆叠中或导入到图层的图像输入中。

![](../../assets/svg-support.jpg){width="500px"}

### 在 Illustrator 中编辑

一项新的“在应用程序中编辑”功能为更新导入的图像带来了极大的灵活性。 如果要调整SVG文件，只需在Illustrator中直接编辑该文件即可。 Sampler将使用新SVG立即更新您的视觉效果。

### 全新裁剪UX/UI

Sampler现在拥有一个经过改版的适当裁切构件，可轻松定义裁切区域。 将非正方形图像裁剪为正方形纹理时，您也不会获得拉伸的结果。

![](../../assets/crop-9.jpg){width="500px"}

### 法线贴图格式

编辑首选项以设置工作流程所需的[正常格式](../../interface/preferences/normal-format.md)。 法线将按照您在首选项中选择的格式导入、显示和导出。

![](../../assets/7-normal-format-preferences.jpg){width="250px"}

### 以SBSAR格式导出材料属性

着色器设置的所有材料参数（正常缩放、Height缩放、Height级别……） 将导出到Sbsar 文件中，以便在Substance 3D Stager中读取，从而获得材料的完美匹配。

![](../../assets/material-consistency-sa-sg.jpg){width="500px"}

## 发行说明

### 3.1.0索科alt

*（2021年9月28日发布）*

**已添加：**

* [拾色器]新的拾色器UI
* [拾色器]并排预览当前和以前的颜色
* [拾色器]以十六进制输入颜色
* [拾色器]带有颜色预览的新吸管
* [拾色器]吸管可以选取Sampler之外的颜色
* [拾色器]在RGB或HSV色彩空间中微调颜色
* [拾色器]保存和管理色板
* [互操作性]在Illustrator中通过图像导入图层或图像参数编辑图像
* [互操作性]在Photoshop中通过图像导入图层或图像参数编辑图像
* [Widget]新的裁切构件
* [Widget]按Enter键验证裁剪
* [构件]裁切构件会读取图像大小以适合构件，并在调整大小时保持比例
* [UI]新的缩放滑块UI
* [应用程序]在首选项中添加法线格式选区
* [应用程序]图像导入图层中的法线格式遵循在首选项中设置的默认法线格式
* [Application]在2D 视图中，法线显示在首选项中设置的法线格式之后
* [应用程序]法线以首选项中设置的法线格式导出
* [导出]将普通格式参数添加到SBS和Sbsar 文件导出
* [导出]将着色器设置添加到SBS和Sbsar 文件导出中
* [导出]设置导出的图形的默认分辨率
* [复合滤镜]用7z打包SSA滤镜
* [复合滤镜]在复合滤镜中添加类别元数据
* [复合滤镜]复合滤镜可以嵌入缩略图
* [复合滤镜]将复合滤镜扩展名(.ssafilter)添加到“获取内容”的文件对话框
* [复合滤镜]在“资源”面板中导入复合滤镜(.ssafilter)
* [引擎]将Substance引擎更新到v8.2.0

**已修复：**

* [应用程序]连接的本地文件夹可能会挂起
* [应用程序]退出时崩溃
* [应用程序]启动两个Sampler实例时发生崩溃
* [内容]裁剪滤镜包含随机种子调整
* [Content]某些材料有时无法升级
* [导出]使用新添加的自定义预设导出时崩溃
* [导出]导出弹出窗口中缺少估计的包大小
* [导出]修复导出SBS和SBSAR文件时出现的内存泄漏问题
* [复合滤镜]复合滤镜可能具有重复的输入
* [复合过滤器]如果过滤器具有不符合的引用，则崩溃
* [复合滤镜]对包含复合滤镜的图层堆叠重新排序时崩溃
* [复合滤镜]渲染有时会挂起
* [图像导入]导入图像会触发多个渲染
* [图层]撤消/重做时崩溃
* [图层]添加基础材质时的崩溃
* [图层]使用无效图像作为环境光时出现崩溃
* [图层]修复插入具有多个图形的过滤器时重复导入的问题
* [图层]重新排序图层并非始终有效
* [Project]加载不完整的项目文件时出现崩溃
* [Project]打开损坏的项目时崩溃
* [项目]某些资源可能会从项目中消失
* [属性]修复缺失滤镜的预设
* [UI]无法设置角度参数
* [UI]筛选“资源”面板中的元数据显示
* [UI]按类别分组会隐藏过滤器
* [UI]“资源”面板中的滚动问题
* [UI]导出面板现在有一个滚动条
* [UI]在图像选择器中，某些图像格式不显示缩略图

**已知问题：**

* [实时引擎2021]繁重的计算可以崩溃应用程序
* [实时引擎2021]实时引擎2021将在装有AMD CPU和Nvidia GPU的Windows计算机上崩溃
* [拾色器]在第二个显示器上选取具有不同分辨率的颜色可能不起作用
