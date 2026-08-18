---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/release-notes/old-versions/version-0-7-0.html"
breadcrumb-title: ''
description: 查看Substance 3D Sampler版本0.7.0的发行说明，了解更新、改进和错误修复。
helpx_creative_field: ""
helpx_description: Sampler > Release Notes > Old Versions > Version 0.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 版本0.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# 版本0.7.0

发行日期：**2019/06/13**

已添加：

* [滤镜]通过按空格键可快速访问滤镜
* [Filters]新的专用面板用于管理、浏览和导入过滤器
* [元数据]右键单击材质以查看其元数据
* [元数据]右键单击某个材质以查看其在磁盘上的位置
* [滑块]按住Ctrl键并将滑块悬停在移动位置时为其制作动画
* [滑块]按P停止并重新开始滑块动画
* [导出] SBSAR导出遵循Substance Source准则
* [许可证]使用Substance Alchemist变量激活环境
* [UX] “文件”对话框记住最后一个选定的文件路径
* [UX] “文件夹”对话框记住最后一个选定的文件夹路径
* [UI]更新资源面板UI
* [UI]更新搜索栏UI
* [UI]“创建新材质”图标已更新
* [帮助] URL已更新为[substance3d.com](http://substance3d.com)域
* [网格]布料网格现已可用
* [内容]新的腐蚀过滤器
* [内容]新的氧化滤镜
* [内容]新的Moss滤镜
* [内容]新建Dust过滤器
* [内容]新建墙式图案滤镜
* [内容]新建石墙图案滤镜
* [Content]全新木饰面滤镜
* [内容]全新金属光洁度滤镜
* [内容]新建Snow过滤器
* [Content]新的随机化筛选器
* [内容]您现在可以直接在基础材质滤镜中导入纹理

已修复：

* 修复存储图层栈叠时出现的崩溃问题
* 可以在环境旋转滑块中添加一个大于1的值
* 在将混合图层从混合图层来回转换为素材图层时，不会丢失混合参数
* 多次生成同一图层栈叠的变体时修复重复项
* 重新打开材质时，Alchemist会记住滑块已修改的范围（最小和最大）

已知问题：

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* 不建议使用“愉悦”阶段的快速可见性切换
* 自定义环境导入可能会变成黑色
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可能会在MacOS上崩溃
