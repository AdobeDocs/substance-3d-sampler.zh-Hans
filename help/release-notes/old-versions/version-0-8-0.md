---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/release-notes/old-versions/version-0-8-0.html"
breadcrumb-title: ''
description: 查看Substance 3D Sampler版本0.8.0的发行说明，了解新增功能、更新和改进。
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 0.8.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本0.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---


# 版本0.8.0

**已添加：**

* [资源]在本地磁盘上连接和镜像您的材料文件夹
* [资源]浏览您的材料文件夹及其子文件夹
* [资源]将您的素材资源面板分离到一个单独的窗口中，以全屏查看您的资源
* [资源]新的“资源”面板布局支持文件夹和子文件夹导航
* [资源]使用Breadcrum浏览文件夹
* [资源]强制同步您的本地文件夹，使用通过右键单击访问的“同步”选项
* [资源]使用可通过右键单击访问的“断开连接”选项，断开本地文件夹的连接
* [管理]显示Substance文件的嵌入标签
* [管理]添加、编辑和删除材料的标签
* [管理]评价您的材质
* [图层]支持全景输出
* [图层]您可以在“图像导入”图层中删除图像输入
* [图层]自动选择新添加的图层
* [图层]删除图层后自动选择下方图层
* [UX]切换到其他实验室时，保持左侧面板可见
* [UX]在非空图层栈栈中导入图像时，不要创建基础图层或打开材质工作流程弹出窗口
* [UI]新建文本字段样式
* [UI]新的SearchBox样式
* [UI]新建面板标题样式
* [UI]新的忙碌指示器样式
* [UI]新建图层栈叠背景样式
* [UI]使用Adobe Clean字体
* [UI]移除颜色输入参数的吸管图标占位符
* [性能]忙碌指示器优化
* [内容]新的图案生成器滤镜
* [内容]新增模糊滤镜

**已修复：**

* [Inspire]修复使用10种以上颜色时崩溃的问题
* [2D视图]在2D视图的通道列表中修复滚动条
* [查看器]修复导入非2次幂的环境映射时崩溃的问题
* [内容]修复浮雕和穿孔滤镜自定义图案的PNG导入问题
* [导出]修复普通比特和Height比特（每通道16位）导出
* 在导入包含两个同名预设的素材时，修复无限循环
* 修复基础材质图层中显示的长文件路径

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* 不建议使用“愉悦”阶段的快速可见性切换
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可能会在MacOS上崩溃
* 在MacOS上退出时可能会随机崩溃
