---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/pipeline-and-integrations/hp-z-captis-support/faq-hp-z-captis-support-in-sampler.html"
breadcrumb-title: ''
description: 访问有关Substance 3D Sampler中HP Z Captis支持的常见问题以查找有关硬件集成和使用情况的答案。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 有关Sampler中的HP Z Captis支持的常见问题解答
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---


# 常见问题解答

## 素材示例

+++Captis涵盖哪些用例？
该解决方案涵盖跨行业的用例（汽车、服饰、产品设计、媒体和娱乐、体系结构……）。 Studio模式支持桌面拍摄（可重复、高效且简单），而Explorer模式支持移动拍摄“随时随地灵活，适应各种情况”。

+++

+++Captis可以扫描和捕获哪些类型的素材？
可以扫描和捕捉任何素材类型，但多个透明涂层图层除外（汽车颜料不属于Captis范围）。 某些特定素材可能需要在Sampler中进行额外处理才能优化效果。 请注意，处理算法将随时间不断优化。

+++

+++对材料样本大小或形状有何限制？样本是否需要平坦？
Captis可以扫描多种材料样本的大小或形状。 样品在样品盘上被送去磁铁，使样品变平。 使用Captis捕捉素材样本有几种模式：

* 工作室模式：在工作室、工作室或工厂中，Captis将采用长达30厘米x 30厘米的样本，并配有背光以保持不透明度。 样本托盘的深度为1.8厘米。

* 资源管理器模式：您可以在字段、设置时或独特的环境中使用资源管理器环，并为大于30cm x 30cm的样本启用灵活捕获。 当前限制：请注意，“资源管理器模式”仍是早期版本，尚未优化（截至2024年7月29日版本）。

+++

## 软件

+++HP Z Captis设备是否需要软件订阅或许可证才能使用？
Captis设备需要有效的Substance 3D Sampler企业版、团队版或大学许可证，这些许可证可在Substance 3D Collection中获得，使用的条件和使用条款与任何Substance 3D订阅相同。

设备(HP Z Captis)和许可证(Substance 3D Sampler)单独销售。

+++

+++与Adobe的Substance套件存在何种级别的集成？
HP Z Captis设备由Adobe Substance 3D Sampler完全控制和运行：您可以从Substance 3D Sampler预览和启动捕获，捕获完成后，它将自动将PBR通道加载为图层并创建3d素材。 您可以使用Sampler中提供的所有工具和滤镜继续处理您的材质。

在Substance 3D Sampler中捕获的材料后，可将其导出到Substance 3D套件的任何应用程序(Substance 3D Designer、Painter、Stager)和任何支持Substance的第三方应用程序，包括3DS Max、Maya、Blender、Unreal Engine、CLO、Browzwear、VRED、Rhino、Cinema4D等（在此处查看完整列表： <https://www.adobe.com/products/substance3d/plugins.html>）。

+++

+++使用Substance 3D Sampler和Captis的推荐规范有哪些？
可在[此处](system-requirements-to-use-hp-z-captis.md)获得Sampler硬件规范。

+++

+++HP Z Captis工作流程是否同时适用于Windows和Mac？
从2025年2月20日版起，带有HP Z Captis的Sampler工作流程仅在Windows上可用。

+++

+++在哪里可以找到带HP Z Captis工作流程的Substance 3D Sampler版本？
自2025年2月20日版本起，您可以从Creative Cloud桌面应用程序下载的Substance 3D Sampler常规版本中的部分，访问带有Captis的Adobe Substance 3D Sampler工作流程。 无需再从Adobe预发行版本下载它们。

+++

+++哪些内容尚不可用？
*截至2025年8月的限制（Sampler 5.1.0版本）：*

* Sampler with HP Z Captis工作流程目前仅在Windows上可用。

* 今天导出的五个地图是基色、粗糙度、正常、Height、不透明度。

* 资源管理器模式仍然是一个早期版本，尚未优化。

* 平铺是在Sampler图层栈栈中使用当前平铺滤镜执行的。

+++

+++哪些PBR渠道可用？
从2025年8月7日版本起，将导出的五张地图为基色、粗糙度、法线、Height、不透明度。 当前处理管道尚未处理金属量映射。

+++

+++拼贴是否自动完成？
平铺是在Sampler图层栈栈中使用当前平铺滤镜执行的。

自动拼贴过滤器可用于自动拼贴具有定义的重复结构或小图案的材料，每个方向至少具有3个图案。 在文档[&#128279;](../../filters/tools/auto-tiling.md)的专用部分中了解有关此筛选器的更多信息。

+++

+++扫描素材可以导出为哪些格式？
HP Z Captis由Adobe Substance 3D Sampler本机运行。 HP Z Captis可捕捉64张原始图像（可从您的本地文件夹中检索）和PBR映射（可从捕捉的原始图像中进行处理并在Substance 3D Sampler中自动加载）。 Substance 3D Sampler将基于PBR通道创建3d素材，捕捉后自动加载到Sampler图层栈栈中。

从Adobe Substance 3D Sampler中，可以将数字素材导出为Substance 3D Sampler中可用的任何导出格式：Substance文件（.SBS和.SBSAR文件）或位图纹理（包括.PNG、.JPG、.TIFF..）（请参阅Sampler文档网页上的详细信息： [https://helpx.adobe.com/cn/substance-3d-sampler/getting-started/export.html](../../getting-started/export/export.md)）。

+++

+++拍摄期间，LDR和HDR有何区别？
在预览期间，您可以在LDR（低动态范围）和HDR(高动态范围)之间选择输出类型。\
即使选择LDR，也会捕获HDR地图并将其保存在您的设备上。\
建议您选择LDR，因为这将使项目的大小在Sampler以及任何将使用sbsar文件的第三方应用程序中更易于管理。

+++

## 正在处理

+++如果使用特定的文件格式、标准和规范或第三方应用程序，如何在当前的3D管道中使用Captis？
HP Z Captis由Adobe Substance 3D Sampler本机运行。 在Substance 3D Sampler中捕获素材样本并将其数字化后，您可以无缝导出数字素材：

在Substance 3D生态系统的任何应用程序中（包括支持各种导出格式的Substance 3D Designer或Substance 3D Painter： https://experienceleague.adobe.com/zh-hans/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats）。

在将Substance文件格式集成为3DS Max、Maya、Blender、C4D、Rhino、Browzwear、CLO...的任何应用程序中（请参阅下面的完整列表： <https://www.adobe.com/products/substance3d/plugins.html>）。 如果您使用的应用程序未列在此处，您始终可以导出PBR纹理图像，并在任何本机不支持Substance文件格式的应用程序中手动插入这些图像。

+++

+++正在拍摄多少张图片来创建地图？
[8个光板+ 1个背光] x [8个偏振态] x [8个HDR包围曝光] x [4个过曝以减少噪声] = 2048 + 256（背光）

+++

## 设备管理

在[HP网站](https://www.hp.com/us-en/workstations/z-captis.html "HP Z Captis")上详细了解设备及其规范。

+++能否更改设备的IP地址？
要更改设备的IP地址，您可以通过添加一行来修改Windows文件C:\Windows\System32\drivers\etc\hosts.txt ：

例如，您可以添加192.168.55.1 captis-device，然后在<b>Sampler的设置>存储和缓存>素材捕捉> captis地址</b>中，将IP替换为captis-device

+++

## 使用问题

+++Sampler无法检测到HP Z Captis。
确保HP Z Captis已连接到USB 3.0端口。

确保USB数据线连接到HP Z Captis的底座而不是圆锥体。

+++

+++在Sampler窗口中，我的预览完全为黑色。
确保已移除相机保护。

+++

+++将文件从HP Z Captis复制到我的计算机时速度较慢。
确保HP Z Captis已连接到USB 3.0端口。

如果您要求检索素材和测光图像，通常需要更多时间。

+++

+++Sampler未将图像复制到我的计算机。 是否必须重新启动扫描？
不，你没有。 您可以浏览设备的内容，并使用操作系统的文件资源管理器复制Adobe文件夹中找到的图像。

+++

+++菜单指示设备处于恢复模式。
按几秒钟的电源按钮将其关闭。 再次打开。

+++

+++我把圆锥体从底部移到了探险环，我无法再扫描了。
建议在将HP Z Captis从底座或探查器环上拔下之前，先将其关闭。

+++

+++以SBSAR格式导出素材的速度较慢。
确保图像在“属性”面板中不是32位浮点格式。

您还可以将压缩级别设置为“无”以加快导出速度。

+++

+++我想更改已捕捉素材和测光图像的存储路径。
现在，您可以在“编辑”>“首选项”>“存储和缓存”>“素材捕捉”中编辑捕捉的素材和测光图像的保存位置。

+++

+++窗户比我的屏幕大，我无法调整它的大小。
Captis窗口确实无法调整。 您可能正在使用未经处理的屏幕放大率。 Captis支持以下功能：

* 分辨率：1920x1080
  * 最大放大率：100%

* 最大放大率：100%

* 分辨率：2560x1440
  * 最大放大率：125%

* 最大放大率：125%

* 分辨率：3840x2160
  * 最大放大率：200%

* 最大放大率：200%

* 不支持低于1920x1080的分辨率。



+++
