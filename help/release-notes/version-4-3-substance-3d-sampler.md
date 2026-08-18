---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/version-4-3substance-3d-sampler.html"
breadcrumb-title: ''
description: 查看Substance 3D Sampler版本4.3的发行说明，了解新的纹理生成器、刺绣滤镜和透视裁剪工具。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本4.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6cc0519fb8c0f74fa805691ec4adb9e449a627d5
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---


# 版本4.3

<b>Substance 3D Sampler 4.3</b>引入了新的入门内容，包括<b>纹理生成器</b>、<b>刺绣</b>滤镜的新版本和<b>透视裁剪</b>工具。

*发行日期：2024年1月25日*

## 新的“入门资源”内容

![](../assets/NewStarterContent.png)

Sampler附带的材料已更新，以更好地满足<b>工业设计</b>工作流程、<b>时尚</b>工作流程以及媒体和娱乐行业的技术艺术家的需求，现在可以更好地控制创建纹理的技术方面。

## 纹理生成器

![](../assets/sa_whats-new-screen_v4-3-0_generators.png)

新的纹理生成器使用<b>参数噪声、图案</b>和<b>污渍</b>选项对素材创建进行了改进控制。  生成的图像可用于蒙版或渠道地图，让技术和创意团队可以比以往任何时候都更轻松地协作进行素材设计。

![](../assets/sampler4.3-texturegenerators-ezgif.com-video.gif)

使用新的筛选图标可仅解析纹理生成器。

![](../assets/parse-texgen.gif)

## 刺绣

![](../assets/Embroideryv3.png)

更新后的刺绣滤镜提高了拼接精度，最多支持8种颜色。 该材料的输入返回到图层栈栈中，从而能够将其他元材料插入到修补中。

## 透视裁切

![](../assets/PerspectiveCropTool.png)

使用新的透视裁剪工具，您可以通过四个控制点裁切扭曲的材质和扫描内容，以消除透视伪影并获取可平铺的资源。

![](../assets/sampler4.3-perspectivecrop-ezgif.com-video-gif.gif)

## 风格化

![](../assets/03-8.png)

“风格化”滤镜允许您设置任何素材的样式，以获得手绘外观。

## “填充”滤镜中的混合模式

![](../assets/Fill-Blend-mode.gif)

填充滤镜的升级引入了混合模式，允许您将“填充”的值、输入映射或纹理生成器与下方图层的通道结果相乘。

## 图像导入图层改进

![](../assets/Import-Layer-improvements.gif)

您可以在导入图像图层上添加多个图像，并从图像的Alpha通道生成不透明度映射。

## 发行说明

*（发布日期：2024年1月25日）*

<b>已添加</b>：

* [Assets]新的资源类型：纹理生成器
* [资源]入门资源中包含的新材料
* [资源]“属性”面板中图像参数的新资源选择器
* [资源]将纹理生成器从“资源”面板拖放到“属性”面板中的图像选择器中
* [资源]从操作系统文件资源管理器中拖放纹理生成器
* [资源]滤镜可以通过图像输入上的用户标记建议适合的生成器
* [资源]纹理生成器可以定义哪个过滤器应通过用户标记提供建议
* [内容]全新透视裁剪滤镜
* [内容]新的风格化滤镜
* [内容]填充滤镜上的混合模式
* [内容]已更新刺绣滤镜
* [内容]更新了绕图排画滤镜
* [内容]更新了所有滤镜以支持纹理生成器
* [图层]将纹理生成器添加到图层栈叠时，能够选择纹理生成器输出通道
* [图层]能够轻松地在纹理生成器上列出和应用预设
* [图层]在图像选择器中显示纹理生成器预览
* [图层]纹理生成器参数可以显示和导出
* [图层]使用纹理导入创建模板导入单个图像时，指定基色使用情况
* [图层]在“属性”面板中尝试在不兼容的文件拖放到图像选取器中时出现反馈
* [图层]从导入图像的Alpha通道生成不透明度通道
* [图层]更改图像到材质(AI)的类别时，计算速度更快
* [图层]使用创建模板后，选择最相关的图层
* [图层]位置构件现在可以使用“高级参数”组中的滑块进行调整
* [导出]在队列中显示百分比，而不是原始数字
* [互操作性]将不透明度通道现在在发送至Painter时识别为Alpha通道
* [应用程序]显示和保存硬件信息的新对话框
* [应用程序]更改每个项目的默认Height比例的新首选项
* [应用程序]改进过时资源的显示方式
* [脚本] New asset.documentResolution()和asset.setDocumentResolution()函数
* [脚本]新的select\_asset()函数
* [脚本]用于纹理生成器的Python API
* [Scripting] get\_project\_assets()现在可返回3D对象
* [UI]可在“资源”面板中更改资源缩览图大小
* [UI]更新了视口显示图标

<b>已修复：</b>

* [2D视图]使用鼠标滚轮缩放时在244%处被阻止
* [应用程序]初始化图形API时启动时崩溃
* [Application]如果项目名称包含#字符，则会崩溃
* [应用程序]打开旧项目时可能会崩溃
* [应用程序]重新打开当前项目可能会导致崩溃
* [应用程序]如果未保存，某些项目更改将不会注册，并且在关闭项目时毫无警告地丢失
* [导出]使用多个同名文件时出现.sbs/.sbsar导出问题
* [导出]导出的灰度图像.sbs/.sbsar文件的色彩空间不正确
* [滤镜]不透明度混合行为问题
* [图层] .svg文件有时无法以正确分辨率渲染
* [性能]不需要在磁盘上保存某些项目
* [Project]导入旧项目时无法加载关联的预设
* [脚本]无法获取第一个插入图层的参数
* [UI]将资源悬停在错误的位置或屏幕中时会显示预览弹出窗口
* [UI]在“欢迎”屏幕的顶部，未停靠的面板可见且可用
