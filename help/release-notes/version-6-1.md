---
description: 查看Substance 3D Sampler版本6.1的发行说明，了解新增功能、改进和工作流程增强功能。
title: 版本6.1
hold: true
source-git-commit: 99bb504f8dd5c485bf0d208a85cc3825d186c55f
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 0%
---

# 版本6.1

**Kouign amann**（布列顿分层糕点）

![替代文本](../../help/assets/Sampler_splash_large.jpg)

此版本引入了性能模式，允许任何人关闭可能会减慢其工作流程的设置，并引入了自动稳定性改进，可在较轻的硬件上保护用户。

主要新增功能包括：

## 性能模式

在Sampler中获取更快、响应更快的体验。 新的&#x200B;**性能模式**&#x200B;汇集了所有可能减慢工作流程的设置：分辨率限制、阴影、位移质量和路径跟踪。 关闭您不需要的功能以提高性能和响应速度。

[*此处*](https://www.adobe.com/go/substance-3d-sampler-6.1-performance-mode_cn)的详细信息

![](../assets/v6.1/6_1-Performance_Mode.png)

## 改进了对最低规格计算机的支持

如果您的硬件低于[最低规格](../getting-started/system-requirements.md)，Sampler现在会自动调整以使情况保持稳定。 最有可能减慢速度或导致崩溃关闭的功能会自动关闭。

[*此处*](https://www.adobe.com/go/substance-3d-sampler-6.1-low-specs-mode_cn)的详细信息

![](../assets/v6.1/6_1-Checked.png)

## V6.1发行说明

*（发布日期：2026年11月19日）*

## 已添加

* &amp;lbrack；Application&amp;rbrack；报告最低硬件要求警告的新方法
* &amp;lbrack；Captis&amp;rbrack；添加一个可在4到8个偏振角之间进行选择的选项
* &amp;lbrack；Captis&amp;rbrack；新建字幕快速操作
* &amp;lbrack；Export&amp;rbrack；正确地向用户报告导出失败
* &amp;lbrack；Export&amp;rbrack；更新虚构引擎4导出预设（重命名为虚构引擎5）
* &amp;lbrack；Performance&amp;rbrack；从文件创建资源现在是异步的
* &amp;lbrack；Performance&amp;rbrack；将工作负载从主线程移动到工作线程
* &amp;lbrack；性能&amp;rbrack；新性能模式
* &amp;lbrack；Project&amp;rbrack；在项目保存失败时警告用户
* &amp;lbrack；Scripting&amp;rbrack；针对资源的新的generate_thumbnail方法和针对资源的新类型属性
* &amp;lbrack；脚本编写&amp;rbrack；从Python模块将3D视图快照渲染到文件
* &amp;lbrack；UI&amp;rbrack；单击放置区域上的任意位置可打开文件对话框
* &amp;lbrack；UI&amp;rbrack；左侧导览栏工具（色调均化、裁切、拼贴、变换、修复、颜色……）的快捷方式
* &amp;lbrack；UI&amp;rbrack；升级qt-spectrum以获取最新图标

## 固定

* &amp;lbrack；3D 视图&amp;rbrack；修复立即UV 偏移和旋转，移除OpenPBR的正常缩放
* &amp;lbrack；3D 视图&amp;rbrack；通过确保在删除崩溃时不进行阶段编辑来防止视口
* &amp;lbrack；3D 视图&amp;rbrack；在更改显示的资源时正确删除位移(Height)信息
* &amp;lbrack；3D 视图&amp;rbrack；在删除网格时正确更新文档
* &amp;lbrack；Application&amp;rbrack；确保在计算动态筛选器调试信息时曲面保持活动状态
* &amp;lbrack；Application&amp;rbrack；在场景中退出时修复崩溃
* &amp;lbrack；Application&amp;rbrack；修复在资产数据库服务关闭期间删除资产时可能发生的崩溃
* &amp;lbrack；Application&amp;rbrack；使缓存调试信息线程安全，以防止崩溃
* &amp;lbrack；Application&amp;rbrack；在访问崩溃之前，通过测试节点阻止节点不为空
* &amp;lbrack；Application&amp;rbrack；防止因访问空矢量的第一个元素而导致崩溃
* &amp;lbrack；Application&amp;rbrack；阻止invalidateVisibleIfs中的崩溃
* &amp;lbrack；Application&amp;rbrack；在数据库服务关闭时创建资源时阻止崩溃
* &amp;lbrack；Application&amp;rbrack；在退出时防止出现争用情况
* &amp;brack；Assets&amp;rbrack；确保资源在正确的锁后得到正确的保护
* &amp;lbrack；Captis&amp;rbrack；在手动模式下强度值有错误
* &amp;lbrack；Captis&amp;rbrack；防止用户选择大于后端允许的区域
* &amp;lbrack；通道设置&amp;rbrack；在ASM中双出现SpecularColor
* &amp;lbrack；通道设置&amp;rbrack；修复从字符串创建的使用的ID
* &amp;lbrack；Content&amp;rbrack；Atlas Scatter不透明度问题
* &amp;lbrack；Content&amp;rbrack；刺绣滤镜缺少金属功能
* &amp;lbrack；Content&amp;rbrack；修复穿孔过滤器
* &amp;lbrack；Content&amp;rbrack；修复风格化滤镜的类别和“资源”面板中的几项修复
* &amp;lbrack；Content&amp;rbrack；更新填充筛选器
* &amp;lbrack；Creative Cloud&amp;rbrack；修复Creative Cloud中3D资源的路径
* &amp;lbrack；引擎&amp;rbrack；在作业被取消的情况下访问引擎数据时阻止崩溃
* &amp;lbrack；Export&amp;rbrack；添加防御代码以检查结构的树不为空
* &amp;lbrack；Export&amp;rbrack；用于避免SBS生成中崩溃的防御代码
* &amp;lbrack；Export&amp;rbrack；允许输出自定义用法，即使引擎已知道这些用法
* &amp;lbrack；导出&amp;rbrack；修复导出预设
* &amp;lbrack；Export&amp;rbrack；法线图在USD中导出为Raw
* &amp;lbrack；Export&amp;rbrack；使用预设导出时，使用输出标签而不是用法
* &amp;lbrack；公开参数&amp;rbrack；修复动态筛选器上的公开参数
* &amp;lbrack；公开参数&amp;rbrack；修复公开参数名称更改时的更新
* &amp;lbrack；Filters&amp;rbrack；确保动态筛选器微调标识符在每个平台上的每次运行之间都相同
* &amp;lbrack；Filters&amp;rbrack；隐藏自动拼贴映射选择中不支持的用法
* &amp;lbrack；图层&amp;rbrack；更改图层可见性将始终重新创建结构
* 在某物上拼合仿制图章时崩溃(&amp;L)
* &amp;lbrack；Layers&amp;rbrack；直接在堆叠上插入生成器现在可正确设置调整和节点名称
* &amp;lbrack；Layers&amp;rbrack；插入带有“填充”的生成器可在拾色器中正确显示纹理
* &amp;lbrack；本地化&amp;rbrack；将中文字符集固定为GB18030
* 在仿制图章上绘画后存储时的&amp;lbrack；项目&amp;rbrack；崩溃
* &amp;lbrack；Project&amp;rbrack；确保会话和项目名称已实际保存
* &amp;lbrack；Project&amp;rbrack；保存树时防止崩溃
* &amp;lbrack；Project&amp;rbrack；从数据库还原损坏的项目时返回
* &amp;lbrack；快速操作&amp;rbrack；在堆叠中没有图像时显示图像选择弹出窗口
* &amp;lbrack；快速操作&amp;rbrack；修复快速操作问题；取消快速操作不再关闭快速启动
* &amp;lbrack；快速操作&amp;rbrack；导入纹理要求启用某些通道，但不应该启用
* &amp;lbrack；快速操作&amp;rbrack；在快速操作无法加载时防止崩溃
* &amp;lbrack；快速操作&amp;rbrack；更新快速操作内容
* &amp;lbrack；渲染&amp;rbrack；修复ASM材料的combineNormalAndHeight
* &amp;lbrack；渲染&amp;rbrack；修复带有Vulkan的可显示纹理的使用情况
* &amp;lbrack；正在渲染&amp;rbrack；当唯一用法输出发生更改时将树标记为已修改
* &amp;lbrack；渲染&amp;rbrack；使用正确的引用结构计算要计算的树节点
* &amp;lbrack；脚本编写&amp;rbrack；在导出过程中发生错误时不要停止
* &amp;lbrack；脚本&amp;rbrack；确保import_images()返回导入的图层
* &amp;lbrack；脚本编写&amp;rbrack；将图像微调设置为图像资源引用失败
* &amp;lbrack；脚本编写&amp;rbrack； get_filters()不返回动态筛选器
* &amp;lbrack；Thumbnail&amp;rbrack；生成缩略图时修复潜在崩溃
* &amp;lbrack；Thumbnail&amp;rbrack；在版面更改时重新创建缩略图生成器
* &amp;lbrack；UI&amp;rbrack；更改资源可能会将Height缩放设置为滑块最大值
* &amp;lbrack；UI&amp;rbrack；在纹理中绘制会实时更新纹理选择器
* &amp;lbrack；UI&amp;rbrack；进入全屏模式时未最大化，现在会填充整个窗口
* &amp;lbrack；UI&amp;rbrack；修复损坏的Substance杂志链接
* 打包；UI&amp;rbrack；修复导出弹出边距(&amp;L)
* 打包；UI&amp;rbrack；修复章节标题大小(&amp;L)
* &amp;lbrack；UI&amp;rbrack；修复字符串中的拼写错误
* &amp;lbrack；UI&amp;rbrack； Linux文件对话框现在使用GTK插件
* &amp;lbrack；UI&amp;rbrack；显示表情符号时防止崩溃
* &amp;lbrack；UI&amp;rbrack；将.ssa文件重命名为“Adobe Substance 3D Sampler archive”（无版本或Beta版）
* &amp;lbrack；UI&amp;rbrack；使用鼠标时恢复可闪烁的减速
* &amp;lbrack；UI&amp;rbrack； “创建新材料”对话框中的小修复
