---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-4substance-3d-sampler.html"
breadcrumb-title: ''
description: 查看Substance 3D Sampler版本4.4的发行说明，了解生成式工作流程，包括文本到纹理和图像到纹理功能。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6cc0519fb8c0f74fa805691ec4adb9e449a627d5
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# 版本4.4

<b>Substance 3D Sampler 4.4</b>引入了三种新的生成式工作流程（Beta版）：文本到纹理、文本到图案和图像到纹理。

<b>生成式AI功能仅在Adobe版本</b>上可用，因为它需要Adobe帐户。 因此，这些功能<b>在Steam</b>上不可用。

*发行日期：2024年5月23日*

## 文本到纹理

![](../assets/textToTexture_whatNewPanel.png)

使用“文本到纹理”功能，您可以探索使用<b>文本提示</b>创建材料的新方法。 您可以根据详细的文本描述生成拼贴纹理，并通过图像到材料或任何Sampler滤镜在结果的基础上继续构建，使其成为您所独有的字体。

## 图像到纹理

![图像到纹理](../assets/imagetoText_whatNewPanel.png "图像到纹理")

使用“图像到纹理”，您可以从<b>您自己的参考图像</b>创建拼贴正方形纹理，无论它是非正方形图像还是非拼贴图像。 这样，您就可以接近所需的结果，而无需编写完美的提示。\
“图像到纹理”还可以根据已创建的Content创建变体，从而帮助您节省时间。

## 文本到图案

![文本到图案的插图图像](../assets/patterns_whatNewPanel.png)

文本到图案功能将使用您的<b>文本提示</b>生成方形拼贴图案。 然后，您可以将它用作base color和布料编织滤镜，以创建一个原始的布料材料，将它用作图案滤镜的输入等等！

## 发行说明

*（发布日期：2024年5月23日）*

<b>已添加</b>：

* [Application]3D 捕捉缓存现在存储在单独的子文件夹中
* [生成式AI]图像到纹理(Beta)
* [生成式AI]文本到图案(Beta)
* [生成式AI]文本到纹理(Beta)
* [脚本]资源现在具有“资源”属性
* [脚本]图层现在具有“output\_usages”属性

<b>已修复：</b>

* [Application]打开损坏的项目文件时出现崩溃
* [Application]项目包含损坏的资源时的崩溃
* [应用程序]在Windows上拔出监视器时崩溃
* [应用程序] Windows任务栏中的应用程序图标不正确
* [应用程序]主配置文件损坏会导致文件删除
* [应用程序]面板显示在弹出窗口前面
* [Content]纹理生成器的缩览图模糊
* [导出]导出.sbs/.sbsar文件时，从导入的图像生成的不透明度通道中断
* [滤镜]放大可以根据其输入图层崩溃
* [生成式AI]从服务收到意外结果时可能发生崩溃
* [脚本]从环境变量自动加载增效工具时出现崩溃
* [脚本]通过API分配输出使用情况时可能出现崩溃
