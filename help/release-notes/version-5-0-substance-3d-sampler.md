---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-5-0-substance-3d-sampler.html"
breadcrumb-title: ''
description: 查看Substance 3D Sampler版本5.0的发行说明，了解新的数字化工具、功能和工作流程改进。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本5.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# 版本5.0

![](../assets/welcome_digitization_tool.jpg)

<b>Substance 3D Sampler 5.0</b>引入了更简单的方法来使用更高质量的扫描和渲染进入材料的数字孪生。

主要新增功能包括：

## 快速操作

一键启动Sampler的所有主要工作流程，并准备好您的图层堆叠！

*[此处](../interface/panels/quick-actions-panel.md)*&#x200B;有详细信息。

![](../assets/quick_actions_1440x810.png)

## 全新的主屏幕布局

直接从主页查找所有项目和教程，开始您的工作。

*[此处](../interface/the-home-screen.md)*&#x200B;有详细信息。

![](../assets/new_home_screen_layout_1440x810.png)

## 新建渲染器

在实时路径跟踪和路径跟踪之间进行选择，以提高视觉一致性并支持新的材料属性。 直接从3D视图中保存您的工作快照。

*[此处](../interface/2d-and-3d-viewport.md)*&#x200B;有详细信息。

![](../assets/eclair_support_1440x810.png)

## HP Z Captis集成

借助HP Z Captis和Substance 3D Sampler，只需短短几分钟即可将真实的材料变为数字。

适用于企业、团队和教育帐户的功能。

*[此处](../pipeline-and-integrations/hp-z-captis-support/hp-z-captis-support.md)*&#x200B;有详细信息。

![](../assets/hp_z_captis_1440x810.png)

## V5.0发行说明

*（发布日期：2025年2月20日）*

<b>已添加</b>：



* [入门]新主页，可快速访问学习内容、示例项目、快速操作以及最近打开的项目。
* [入职]使用可以从主页和专用面板访问的新快速操作快速入门
* [用户引导] [Content]快速操作是预定义的工作流，会在图层堆叠中填充最常用的图层
* [入门]可以通过新的快速入门菜单、快速操作或自定义项目创建新项目
* [入门]可通过专用按钮直接从主页创建空项目
* [3D 视图]新的高级栅格器和路径跟踪器在Substance生态系统中带来了新的渲染功能（如涂层、光泽、translucency、次表面散射等属性）和视觉一致性
* [3D 视图]现在可以直接在3D视图中访问查看器设置
* [3D 视图]可以将渲染快照保存在剪贴板或文件中
* [3D 视图]显示网格以可视化场景来源
* [3D 视图]启用地面平面捕捉阴影和反射
* [3D 视图]控制您的地面平面如何反光和不透明
* [3D 捕捉]在地面上定位网格
* [应用程序]在应用程序启动时检查硬件兼容性
* [Application]崩溃报告窗口现在会在崩溃发生后立即打开
* [内容]打开示例项目以轻松开始
* [导出]将着色器导出到USD文件中
* [生成式AI]在“图像”中使用“图像”作为纹理工作流程的输入时，请勾选“不推断”标记
* [Project]缩览图存储在项目文件中，以便快速打开项目
* [项目]在首选项中进行设置，以使用不同模式（无缓存、轻缓存、完全缓存）在项目文件中存储缓存数据
* [脚本] [突破性更改]将Qt迁移至Qt6.15 — 现有插件的影响兼容性
* [脚本]默认增效工具和脚本文件夹现在位于“文档”文件夹中
* [脚本]增效工具的新UI，与主要Sampler面板在视觉上保持一致
* [脚本]访问2个增效工具示例以发现Sampler增效工具功能
* [脚本]新的open\_3d\_catpure()函数
* [脚本]插入图层时，控制是将其插入到目标位置的上方还是下方

<b>已修复：</b>

* [3D 捕捉]如果在macOS上无法启动对象捕获，则会崩溃
* [应用程序]退出时崩溃
* [应用程序]将资源添加到项目面板时，退出时挂起
* [应用程序]除非按Enter，否则无法重命名项目资源
* [应用程序]还原和重做菜单项应在以下情况下处于禁用状态
* [资源]无法从“资源”面板的“所有库”部分中删除资源
* [内容]贴图集创建者 — 使用现有不透明度图（如果存在）
* [Content] Color ID混合 — 修复基色拾色问题
* [图层]在使用生成器时避免无用的计算
* [图层]调整生成器可能会导致触发太多计算
* [性能]改进GPU内存管理
* [Performance]重新启动应用程序时可能不使用渲染缓存
* [资源]只读文件在“资源”面板中不可见
* [脚本]允许添加另一个图层后重用该图层
* [脚本]在一个脚本中多次更改图层堆叠结构可能会失败

<b>已删除：</b>

* [应用程序]删除对.dng和.nef图像文件的支持
