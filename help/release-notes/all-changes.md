---
helpx_url: 'https://helpx.adobe.com/substance-3d-sampler/release-notes/all-changes.html'
breadcrumb-title: ''
description: 查看所有Substance 3D Sampler版本之间的更改和更新，以跟踪功能随时间的演变和改进。
helpx_description: Sampler > Release Notes > All Changes
title: 所有更改
user-guide-description: ''
user-guide-title: ''
source-git-commit: 275dc218870f111aa99533840a5aea4c3d22f0cf
workflow-type: tm+mt
source-wordcount: '24964'
ht-degree: 0%
---

# 所有更改

此页面将重新组合发生在Substance 3D Sampler上的所有更改，从新增功能到错误修复。

## 版本6

### **6.0.4**

*（发布日期：2026年9月24日）*

**已更改**
[引擎]将Substance 引擎更新到9.6.1

**固定**
将图像添加到浮雕蒙版时[图层]崩溃
[安全性]常规修复

### **6.0.3**

*（发布日期：2026年8月24日）*

**已修复：**

[渲染]恢复错误的NVIDIA驱动程序的临时解决方法

### **6.0.2**

*（发布日期：2026年6月25日）*

**已添加：**

* &amp;lbrack；Assets&amp;rbrack；检查sbsar版本，并警告引擎太旧而无法读取
* &amp;lbrack；Captis&amp;rbrack；添加返回选项以在首选项中保存captis测光法

**已修复：**

* 如果物理尺寸功能已禁用，则&amp;lbrack；2D 视图&amp;rbrack；不“以物理比例显示”
* &amp;lbrack；分析&amp;rbrack；缺少分析事件
* &amp;lbrack；Analytics&amp;rbrack；阻止使用崩溃面板报告vk设备上的崩溃
* &amp;lbrack；Application&amp;rbrack；不在退出时销毁vkdevices以避免nvidia驱动程序中的崩溃
* &amp;lbrack；应用程序&amp;rbrack；修复链接集合观察程序退出+通道管理器
* lbrack；Application&amp;rbrack；在退出时防止崩溃(&amp;L)
* &amp;lbrack；Content&amp;rbrack；“金属光洁度”滤镜不影响金属度
* &amp;lbrack；Content&amp;rbrack；将物理尺寸添加到动态滤镜中缺少的内容
* &amp;lbrack；Filters&amp;rbrack；从隐藏资源列表中移除内容识别填充
* &amp;lbrack；Layers&amp;rbrack；单击“重置所有设置”不会重置“应用于”下拉菜单
* 打包；图层&amp;打包；调整位置Widget的最小值和最大值(&amp;L)
* &amp;lbrack；图层&amp;rbrack；正确更新滤镜
* &amp;lbrack；物理尺寸&amp;rbrack；确保物理缩放适用于所有地方+使用动态滤镜确保物理大小正常
* &amp;lbrack；Project&amp;rbrack；确保创建新资源时的资源分辨率为默认分辨率(2k x 2k)
* &amp;lbrack；Project&amp;rbrack；重新打开用于打开先前版本的当前项目
* &amp;lbrack；Project&amp;rbrack； Sampler不再提供恢复损坏项目备份的功能
* &amp;lbrack；渲染&amp;rbrack；以最大2k分辨率渲染素材缩览图
* &amp;lbrack；UI&amp;rbrack；用于避免用户速度超过UI时崩溃的防御代码

### **6.0.1**

*（发布日期：2026年5月21日）*

**已添加：**

* &amp;lbrack；Application&amp;rbrack；在打开具有3D对象或环境光照的项目时警告用户
* &amp;lbrack；Captis&amp;rbrack；使UI适应小屏幕
* &amp;lbrack；Captis&amp;rbrack；更新标题UI
* &amp;lbrack；通道设置&amp;rbrack；在ASM中使用SSS通道时自动激活SSS
* &amp;lbrack；Engine&amp;rbrack；将Substance 引擎更新到版本9.4.3
* &amp;lbrack；预设&amp;rbrack；默认情况下会打开“应用预设缩略图值”
* &amp;lbrack；资源&amp;rbrack；默认情况下显示“所有库”，而不是在“资源”面板中显示“起始资源”
* &amp;lbrack；脚本编写&amp;rbrack；添加Python函数以管理图层的“应用对象”
* &amp;lbrack；UI&amp;rbrack；资源列表现在可响应：资源大小适应容器
* 默认情况下显示3D/2D视图(&amp;lbrack)；UI&amp;rbrack；
* 从资源管理器中删除素材时，&amp;lbrack；UI&amp;rbrack；显示素材优化弹出窗口
* &amp;lbrack；UI&amp;rbrack；启用设备栏按钮工具提示的翻转

**已修复：**

* &amp;lbrack；应用程序&amp;rbrack；修复色彩空间问题
* &amp;lbrack；应用程序&amp;rbrack；修复设置更新程序
* &amp;lbrack；Application&amp;rbrack；使扫描通道在设置为自动时处于活动状态
* &amp;lbrack；主屏幕中的“新建项目”按钮不再抹除以前同名的项目(&amp;R)
* &amp;lbrack；Application&amp;rbrack；防止在macOS上退出崩溃
* &amp;lbrack；Application&amp;rbrack；阻止访问无效资源引用的资源
* &amp;lbrack；Application&amp;rbrack；在微调中从VersionedImage访问表面时防止崩溃
* &amp;lbrack；Application&amp;rbrack；在阶段不存在时防止崩溃
* &amp;lbrack；Captis&amp;rbrack；确保在关闭Sampler之前断开Captis的连接
* &amp;lbrack；Captis&amp;rbrack；防止显示USB-2警告两次
* &amp;lbrack；声道设置&amp;rbrack；修复OpenPBR声道名称
* &amp;lbrack；通道设置&amp;rbrack；更新OpenPBR通道的长标签
* &amp;lbrack；Content&amp;rbrack；将SSS值的所有网格单位从米更新为厘米
* &amp;lbrack；Export&amp;rbrack；确保将默认值插入动态滤镜
* &amp;lbrack；Export&amp;rbrack；图像现在保存在工作线程中，以提高性能
* &amp;lbrack；滤镜&amp;rbrack；打开缩放功能时的内容识别填充崩溃
* &amp;lbrack；Filters&amp;rbrack；无法从资源面板打开动态筛选器的位置
* &amp;lbrack；滤镜&amp;rbrack；修复“自动拼贴”调整步骤中的全部重置
* &amp;lbrack；Filters&amp;rbrack；恢复禁用树结构创建中的使用处理
* &amp;lbrack；Filters&amp;rbrack；为upscale参数设置正确的默认值
* &amp;lbrack；Filters&amp;rbrack；更新生成器，即使它们位于填充图层中
* &amp;lbrack；图层&amp;rbrack；禁止重命名输入图层标题或占位符图层
* &amp;lbrack；图层&amp;rbrack；防止在图层插入期间由于指针悬停而崩溃
* &amp;lbrack；图层&amp;rbrack；拼合图层名称中的图像数量错误
* &amp;lbrack；本地化&amp;rbrack；确保在切换语言时更新预设名称
* &amp;lbrack；本地化&amp;rbrack；资源面板中的多个翻译问题
* &amp;lbrack；本地化&amp;rbrack；快速操作类别本地化问题
* 仅对打开的部分执行加载调整(&amp;L)
* &amp;lbrack；Preferences&amp;rbrack；清除首选项缓存路径会重置为以前的值
* 使用路径跟踪器时发生&amp;lbrack；渲染&amp;rbrack；内存泄漏
* &amp;lbrack；Rendering&amp;rbrack；防止删除纹理，但用户仍可通过Vulkan访问
* &amp;lbrack；渲染&amp;rbrack；纹理旋转未从0-1转换为0-360
* &amp;lbrack；脚本编写&amp;rbrack；从Python文档中删除不存在的类
* 如果没有选定资源，则&amp;lbrack；Scripting&amp;rbrack； selectedAsset返回None
* &amp;lbrack；Tools&amp;rbrack；重置纹理值现在会停止绘画并清除修补程序视图
* &amp;lbrack；UI&amp;rbrack；在调整内容时不要关闭“属性”面板中的部分
* &amp;lbrack；UI&amp;rbrack；悬停时公开颜色微调标签不可见
* &amp;lbrack；UI&amp;rbrack；修复资源列表响应行为
* &amp;lbrack；UI&amp;rbrack；在AssetItem工具提示中修复绑定循环
* &amp;lbrack；UI&amp;rbrack；修复在选定预设组上双击的问题
* 打包；UI&amp;rbrack；在图像演示器中修复放置区域(&amp;L)
* &amp;lbrack；UI&amp;rbrack；为所有语言修复带有按钮的标签
* &amp;lbrack；UI&amp;rbrack；在频道列表弹出窗口中修复日语的行Height
* &amp;lbrack；UI&amp;rbrack；修复长度字段的onAccepted信号
* &amp;lbrack；UI&amp;rbrack；用长左侧控件项修复弹出窗口宽度
* 打包；UI&amp;rbrack；修复资源项中的预览弹出窗口
* 打包；UI打包；修复粗糙/反射拾色器(&amp;R)
* &amp;lbrack；UI&amp;rbrack；修复字符串省略号
* &amp;lbrack；UI&amp;rbrack；修复字符串截断问题
* &amp;lbrack；UI&amp;rbrack；修复开关微调重置按钮
* &amp;lbrack；UI&amp;rbrack；选择自定义导出预设时隐藏材质模型下拉菜单
* &amp;lbrack；UI&amp;rbrack；在导出弹出窗口的通道列表中删除分辨率
* &amp;lbrack；UI&amp;rbrack；重置为默认布局会保留投影查看器设置
* &amp;lbrack；UI&amp;rbrack；恢复“在Photoshop中编辑”和“在Illustrator中编辑”菜单项

**已删除：**

* &amp;lbrack；UI&amp;rbrack；移除图像导入图层的“应用到”部分
* &amp;lbrack；UI&amp;rbrack；在首次启动时删除自动打开的快速操作工具提示

## 版本5

### **5.1.3大佛罗里达大区**

*（发布日期：2026年1月6日）*

**已添加：**

* &amp;lbrack；Captis&amp;rbrack；如果防火墙禁用了FTP协议，则显示警告

**已修复：**

* &amp;lbrack；Captis&amp;rbrack；在捕捉期间中止可能会导致错误
* &amp;lbrack；Captis&amp;rbrack；在捕捉结束时下载结果会使用大量RAM
* &amp;lbrack；Captis&amp;rbrack；在自动强度后立即执行自动对焦会导致错误
* &amp;lbrack；Captis&amp;rbrack；在“摘要”面板中显示HDR结果
* &amp;lbrack；UI&amp;rbrack；在某些情况下，MacOS上的文件夹对话框不会选择正确的文件夹

### **5.1.2大佛罗里达州**

*（发布日期：2025年11月20日）*

**已添加：**

* &amp;lbrack；Application&amp;rbrack；检测图形设备丢失，警告用户并正常退出
* &amp;lbrack；Layers&amp;rbrack；改进了拼合图层时的消息
* &amp;lbrack；图层&amp;rbrack；改进了图像导入和拼合图层的缩览图
* &amp;lbrack；入门&amp;rbrack；更新了主屏幕上的学习内容
* &amp;lbrack；Project&amp;rbrack；恢复崩溃前上次保存的会话状态
* 应用程序图标更新(&amp;L)&amp;L)

**已修复：**

* &amp;lbrack；Application&amp;rbrack；在图层栈栈中插入素材可能会导致macOS崩溃
* &amp;lbrack；Application&amp;rbrack；在macOS上重载时可能崩溃
* &amp;lbrack；Application&amp;rbrack；在视频内存已满的情况下添加图层时可能会崩溃
* &amp;lbrack；Application&amp;rbrack；打开项目时可能崩溃
* &amp;lbrack；Captis&amp;rbrack；在自动强度校准后不久运行自动对焦时失败
* &amp;lbrack；Captis&amp;rbrack；首次捕获后的可靠性和性能问题
* &amp;lbrack；Captis&amp;rbrack；在捕捉结束时复制文件时速度减慢并出错
* 查询Captis设备信息时发生&amp;lbrack；Captis&amp;rbrack；小内存泄漏
* &amp;lbrack；Export&amp;rbrack；多滑块公开参数生成损坏的.sbsar文件
* &amp;lbrack；Layers&amp;rbrack；切换资源时，自动拼贴图案重置为默认值
* &amp;lbrack；图层&amp;rbrack；默认自定基色显示为红色
* &amp;lbrack；Layers&amp;rbrack；可以对仿制图章子图层进行部分拼合，这会导致渲染问题
* &amp;lbrack；Layers&amp;rbrack；在渲染过程中微调图层栈栈时可能会崩溃
* 更改源声道时，自动拼贴目标区域步骤中出现意外错误(&amp;L)
* 创建新素材时，有时显示错误的缩览图(&amp;L)
* &amp;lbrack；快速操作&amp;rbrack；某些快速操作的输入计数错误
* &amp;lbrack；UI&amp;rbrack；动作组按钮具有不同的宽度
* 文本字段中的“清除”按钮有时会触发焦点丢失(&amp;L)
* &amp;lbrack；UI&amp;rbrack；组合框和文本字段过大
* &amp;lbrack；UI&amp;rbrack；图标和标签未对齐
* &amp;lbrack；UI&amp;rbrack；名称字段标签放置不正确
* &amp;lbrack；UI&amp;rbrack；快速操作按钮标签未对齐
* &amp;lbrack；UI&amp;rbrack；滑块显示任意尾随0太多

**已删除：**

* 生成式AI&amp;rbrack；生成式AI功能删除(&amp;L)。 *此功能已从应用程序中移除，服务将于3月5日停止在以前版本的Sampler中工作。*

### **5.1.1大佛罗里达州**

*（发布日期：2025年9月18日）*

**已添加：**

* &amp;lbrack；2D 视图&amp;rbrack；能够在2D 视图中缩小更多的高分辨率纹理
* &amp;lbrack；Captis&amp;rbrack；警告用户在复制文件时出现的问题
* &amp;lbrack；图层&amp;rbrack；复制图层时，请在新图层名称中使用增量编号

**已修复：**

* &amp;lbrack；2D 视图&amp;rbrack；在重置仿制图章的所有属性后绘制描边时，先前创建的描边会重新出现
* &amp;lbrack；Application&amp;rbrack； &quot;保存当前项目？&quot; 弹出窗口使用了错误的项目名称
* 退出时崩溃&amp;lbrack；应用程序&amp;rbrack；
* lbrack；应用程序&amp;rbrack；潜在崩溃
* &amp;lbrack；Application&amp;rbrack；有时，生成缩略图时使用的材料不正确
* &amp;lbrack；Captis&amp;rbrack；在某些设备上，以高分辨率执行扫描时，高度图为黑色
* &amp;lbrack；Captis&amp;rbrack；未设置捕捉名称和正在运行校准时，“开始捕捉”按钮不再禁用
* &amp;lbrack；Export&amp;rbrack；导出。sbsar 文件时，导出可能会失败，而不会通知用户
* 调整参数时，“自动拼贴”滤镜的&amp;lbrack；滤镜&amp;rbrack；高级参数屏幕有时会闪烁
* &amp;lbrack；滤镜&amp;rbrack；拼贴滤镜的默认参数在输出中生成灰色伪像
* &amp;lbrack；Filters&amp;rbrack；有时在高分辨率输入时，“自动拼贴”滤镜高级设置不会显示单个图案点
* &amp;lbrack；Filters&amp;rbrack；自定义大小自动拼贴参数的模式大小具有不正确的默认值
* &amp;lbrack；图层&amp;rbrack；自动拼贴滤镜偶尔出现的颜色问题通常在红色材料上可见
* Layers&amp;rbrack；有时添加图层会将一些微调重置为默认值(&amp;L)
* &amp;lbrack；物理尺寸&amp;rbrack；带有物理尺寸的资源缩略图的Height比例错误
* &amp;lbrack；UI&amp;rbrack；无法重命名公开参数
* &amp;lbrack；UI&amp;rbrack；通道激活按钮不是方形
* &amp;lbrack；UI&amp;rbrack；如果滑块标签太长，则无法访问重置按钮
* 按Return键或单击注销不会移除文本字段中的焦点(&amp;L)
* &amp;lbrack；UI&amp;rbrack；有时会在“物理尺寸”面板中显示不需要的工具提示
* &amp;lbrack；UI&amp;rbrack；创建空项目时，3D视图显示的网格不正确
* &amp;lbrack；UI&amp;rbrack；公开拾色器输入时，悬停时其标签消失
* &amp;lbrack；UI&amp;rbrack；公开参数时，有时彩色点位置不正确

### **5.1.0大佛罗里达大区**

*（发布日期：2025年8月7日）*

**已添加：**

* &amp;lbrack；2D视图&amp;rbrack；画笔大小现在可适应当前的纹理分辨率
* &amp;lbrack；3D视图&amp;rbrack；在首选项中切换3D渲染的原生显示比例
* &amp;lbrack；应用程序渲染引擎更新(&amp;r)
* &amp;lbrack；Captis&amp;rbrack；在预览期间添加“制作正方形”可能性
* &amp;lbrack；Captis&amp;rbrack；自动物理尺寸检测
* &amp;lbrack；捕捉新素材将创建新资源(&amp;R)
* &amp;lbrack；Captis&amp;rbrack；将下拉菜单中的分辨率选择更改为像素/英寸或厘米，而不是最大区域的像素分辨率
* &amp;lbrack；Captis&amp;rbrack；校准上下文帮助
* &amp;lbrack；Captis&amp;rbrack；生成粗糙度映射
* &amp;lbrack；Captis&amp;rbrack；在缺少默认校准文件时警告用户
* &amp;lbrack；过滤器&amp;rbrack；结构化素材和扫描的自动拼贴过滤器
* Lbrack；滤镜&amp;Rbrack；新褶皱移除器滤镜(&amp;L)
* 仿制图章滤镜中的新功能(&amp;L)&amp;R)
* &amp;lbrack；滤镜&amp;rbrack；均衡滤镜中的新功能
* Lbrack；Layers&amp;rbrack；拼合图层的功能
* 右键单击图层以重命名、复制、删除或拼合图层时，&amp;lbrack；图层的&amp;rbrack；上下文菜单
* &amp;lbrack；入门&amp;rbrack；更新欢迎和新增功能屏幕内容
* &amp;lbrack；Performance&amp;rbrack；使用“裁剪”滤镜时性能更好
* &amp;lbrack；Performance&amp;rbrack；改进3D 视图的内存使用
* &amp;lbrack；Performance&amp;rbrack；更新3D视图更快
* &amp;lbrack；物理尺寸&amp;rbrack；启用物理尺寸功能后，使用Substance过滤器时启用“以物理比例显示”
* &amp;lbrack；物理尺寸&amp;rbrack；在空堆叠中导入图像时，建议与图像比例更为一致的分辨率
* &amp;lbrack；快速操作&amp;rbrack； 3个用于扫描处理的新快速操作
* 用于拼合图层的脚本(&amp;L)&amp;R) API
* &amp;lbrack；脚本&amp;rbrack；获取图像导入图层的每个图像的文件名
* &amp;lbrack；脚本编写&amp;rbrack；用于激活/停用资源的给定通道的新功能
* &amp;lbrack；UI&amp;rbrack；重工“图层”面板中的图标和按钮以适应新功能
* &amp;lbrack；UI&amp;rbrack；警告环境光创作已弃用

**已修复：**

* 使用Substance过滤器时，选择“以物理比例显示”可能不起作用(&amp;l)；2D 视图(&amp;r)
* &amp;lbrack；3D 捕捉&amp;rbrack； Svg文件在文件选择器中列出，但不受支持
* 着色器设置中的&amp;lbrack；3D 视图&amp;rbrack；发射强度参数不起作用
* &amp;lbrack；3D 视图&amp;rbrack；有时创建新资源时网格位置不正确
* &amp;lbrack；3D 视图&amp;rbrack；切换到不受支持的硬件上的路径跟踪渲染崩溃
* 关闭手动测量弹出窗口而不设置大小时，&amp;lbrack；应用程序挂起(&amp;R)
* lbrack；应用程序&amp;rbrack；崩溃
* 显示桌面时（&amp;lbrack；Application&amp;rbrack；在Windows上冻结）（Windows键+ D键盘快捷键）
* 切换语言时可能崩溃的&amp;lbrack；Application&amp;rbrack；
* &amp;lbrack；预览数据无效时崩溃Captis&amp;rbrack；
* &amp;lbrack；Captis&amp;rbrack；放大后无法完全缩小
* &amp;lbrack；Captis&amp;rbrack；在某些向导步骤中缺少本地化
* &amp;lbrack；Captis&amp;rbrack；使用Captis时可能会在退出时崩溃
* 如果设备缺少校准文件，&amp;lbrack；Captis&amp;rbrack；扫描不起作用
* &amp;lbrack；滤镜&amp;rbrack；使用仿制图章滤镜时的画笔预览可能不正确，具体取决于纹理和画笔大小
* &amp;lbrack；Filters&amp;rbrack；使用“放大”滤镜后出现错误的输出大小
* &amp;lbrack；滤镜&amp;rbrack；缺少环境旋转和风格化滤镜的图标
* &amp;lbrack；Filters&amp;rbrack；更新某些滤镜可能会导致渲染错误
* 混合两种材质时，图层&amp;rbrack；首次渲染不正确(&amp;L)
* &amp;lbrack；Layers&amp;rbrack；更新图层的按钮显示“全部更新”，即使只有一个更新也是如此
* 在图层栈栈中导入图像时，&amp;lbrack；图层&amp;rbrack；不必要的计算
* &amp;lbrack；Performance&amp;rbrack；改进法线贴图格式处理以减少渲染时间
* &amp;lbrack；物理尺寸&amp;rbrack；手动测量弹出窗口仅在执行自动测量后起作用
* 启用物理尺寸时，&amp;lbrack；物理尺寸&amp;rbrack；在“导出”弹出窗口中的导出分辨率错误
* &amp;lbrack；快速操作&amp;rbrack；生成的资源名称缺少本地化
* 悬停时可能不会显示资源预览(&amp;L)；UI&amp;R；
* &amp;lbrack；UI&amp;rbrack；单击“重置为默认值”按钮可能会破坏某些控件
* 切换项目时未清除&amp;lbrack；UI&amp;rbrack；错误消息
* &amp;lbrack；UI&amp;rbrack；确保没有资源时，视口和属性面板中的材质名称为空
* &amp;lbrack；UI&amp;rbrack；重置为视点参数的默认值按钮不起作用
* &amp;lbrack；UI&amp;rbrack；重置为默认值按钮重叠
* &amp;lbrack；UI&amp;rbrack；取消停靠面板时，某些按钮无法单击
* &amp;lbrack；UI&amp;rbrack；纹理tilling V参数在查看器设置和3D 视图中部分隐藏

**已删除：**

* &amp;lbrack；3D 捕捉&amp;rbrack；删除3D 捕捉支持
* &amp;lbrack；Application&amp;rbrack；删除macOS x86支持

### **5.0.3榛子**

*（发布日期：2025年6月3日）*

**已添加：**

* &amp;lbrack；Captis&amp;rbrack；允许为现有材料指定相同的名称
* &amp;lbrack；Captis&amp;rbrack；将错误消息移动到弹出窗口而不是toasts
* &amp;lbrack；滤镜&amp;rbrack；更新刺绣
* &amp;lbrack；Preferences&amp;rbrack；在查看器设置和着色器设置中添加重置
* &amp;lbrack；UI&amp;rbrack；不在项目资源上显示“显示位置”菜单项

**已修复：**

* &amp;lbrack；3D 捕捉&amp;rbrack；网格后处理筛选器不输出预期映射
* 由于着色器缓存损坏，&amp;lbrack；3D 视图&amp;rbrack； 3D视图不起作用
* 当场景为Z-up时，&amp;lbrack；3D 视图&amp;rbrack；地面平面和网格是垂直的
* &amp;lbrack；3D 视图&amp;rbrack；网格有时消失
* &amp;lbrack；Application&amp;rbrack；启动时关闭登录窗口而不登录有时会崩溃应用程序
* &amp;lbrack；拒绝访问插件配置文件时的Application&amp;rbrack；崩溃
* &amp;lbrack；保存项目时取消选择当前材料(&amp;R)
* &amp;lbrack；Application&amp;rbrack；重置为默认布局会将分辨率设置为64x64
* 渲染图层堆叠时，&amp;lbrack；Application&amp;rbrack； Sampler有时会崩溃
* &amp;lbrack；Export&amp;rbrack；导出分辨率有时重置为64x64
* &amp;lbrack；Export&amp;rbrack；有时无法导出.sbs/.sbsar文件
* 当材料为空时，&amp;lbrack；图层&amp;rbrack；添加基础材质按钮不起作用
* 复制材料时&amp;lbrack；图层&amp;rbrack；纹理拼贴发生更改
* 如果在导入图像之前停靠了“物理尺寸”面板，则&amp;lbrack；物理尺寸&amp;rbrack；自动测量不起作用
* &amp;lbrack；脚本编写&amp;rbrack；自动保存插件已损坏
* &amp;lbrack；UI&amp;rbrack；导出对话框中的间距不正确
* &amp;lbrack；UI&amp;rbrack；滑块微调动画不再有效
* &amp;lbrack；UI&amp;rbrack；滑块在需要时不整数值
* &amp;lbrack；UI&amp;rbrack；某些下拉菜单被裁剪

### **5.0.2榛子**

*（发布日期：2025年4月22日）*

**已修复：**

* 主页上的&amp;lbrack；Application&amp;rbrack； Back按钮已损坏
* 如果磁盘上存在以前版本中的损坏数据，则&amp;lbrack；Application&amp;rbrack；Sampler有时无法启动
* &amp;lbrack；Application&amp;rbrack；导入的图像不出现在视口或图层堆叠中
* &amp;lbrack；Captis&amp;rbrack；即使在重新启动Sampler后，Captis IP地址字段仍为空
* &amp;lbrack；Captis&amp;rbrack；实时相机预览仅在应用程序语言设置为英语时有效
* &amp;lbrack；导出期间的导出&amp;rbrack；崩溃&amp;lbrack；图层&amp;rbrack；绘画有时在以前保存的项目中不起作用
* 仅更新一个频道时，&amp;lbrack；Layers&amp;rbrack； Sampler有时会更新所有纹理
* &amp;lbrack；Layers&amp;rbrack；升级到5.0.x后无法在图层堆叠中使用材料混合
* &amp;lbrack；Layers&amp;rbrack；使用图像到材质(AI)的旧版本更新项目会使材质变为全黑
* &amp;lbrack；Layers&amp;rbrack；尝试导入不受支持的图像时，Sampler会创建一个损坏的图层
* Python API的&amp;lbrack；脚本编写&amp;rbrack；部分不适用于空项目
* &amp;lbrack；UI&amp;rbrack；菜单项有时在“文件”菜单中溢出

### **5.0.1榛子**

*（发布日期：2025年3月20日）*

**已添加**

* &amp;lbrack；Application&amp;rbrack；更新的图形驱动程序兼容性列表
* &amp;lbrack；Captis&amp;rbrack；在操作系统策略阻止使用HP Z Captis时显示弹出窗口
* &amp;lbrack；快速操作&amp;rbrack；解释如何在工具提示中禁用快速操作
* &amp;lbrack；UI&amp;rbrack；崩溃报表窗口UI样式
* &amp;lbrack；UI&amp;rbrack；复制到剪贴板时，显示Toast说明操作已完成(&amp;R)

**已修复：**

* 球面投影关闭时，&amp;lbrack；2D 视图&amp;rbrack；曝光度滑块不起作用
* &amp;lbrack；在纹理外部绘画时，2D 视图&amp;rbrack；会创建已中断的描边
* &amp;lbrack；2D 视图&amp;rbrack； “曝光度”按钮没有工具提示。
* &amp;lbrack；2D 视图&amp;rbrack；缩放非正方形图像的侧边时不会跟随鼠标
* &amp;lbrack；3D 捕捉&amp;rbrack；3D 捕捉在Windows 11 24H2上不起作用
* 如果在崩溃重建步骤中退出Sampler，则&amp;lbrack；3D 捕捉&amp;rbrack；网格
* &amp;lbrack；3D视图&amp;rbrack；计算时间有时显示为0毫秒
* &amp;lbrack；3D 视图&amp;rbrack；将投影从正交更改为透视时，视口变为灰色
* 检查GPU功能时在启动时崩溃Application&amp;rbrack；(&amp;L)
* 安装过程中崩溃Application&amp;rbrack；(&amp;L)
* 右键单击元数据字段后&amp;lbrack；Application&amp;rbrack；退出时崩溃
* 从操作系统文件资源管理器打开SBSAR时，&amp;lbrack；Application&amp;rbrack；环境光缺失
* &amp;lbrack；Application&amp;rbrack；在Sampler运行时打开.sbsar会更改纹理拼贴设置
* &amp;lbrack；Captis&amp;rbrack；某些元数据可能不会在捕获步骤之间传输
* &amp;lbrack；Captis&amp;rbrack；所创建资源的名称不是在元数据字段中输入的名称
* &amp;lbrack；Content&amp;rbrack；示例项目提示更新过滤器，但已经是最新的
* &amp;lbrack；滤镜&amp;rbrack；正常/Height调整滤镜没有图标
* &amp;lbrack；Layers&amp;rbrack；无法更改图像导入图层中的图像
* 使用“放大”滤镜时&amp;lbrack；图层&amp;rbrack；崩溃
* &amp;lbrack；Layers&amp;rbrack；将包含旧图像的项目更新为素材可使素材变为全黑色
* &amp;lbrack；渲染&amp;rbrack；在创建资源后立即调整图层堆叠会中断渲染
* &amp;lbrack；Scripting&amp;rbrack；当项目中没有资源时，“自动保存”插件崩溃
* 画笔工具栏中缺少画笔大小值(&amp;L)
* &amp;lbrack；UI&amp;rbrack；更改应用程序语言不会更新主屏幕中的某些标签
* &amp;lbrack；UI&amp;rbrack；在滑块文本字段中按Esc或Enter将不会失去焦点
* &amp;lbrack；UI&amp;rbrack；在“属性”面板中，“全部重置”按钮与资源名称标签重叠
* 停放和取消停放面板时&amp;lbrack；UI&amp;rbrack；问题
* &amp;lbrack；UI&amp;rbrack；在叠加面板中滚动也将在底层窗口中滚动
* &amp;lbrack；UI&amp;rbrack；无法在“主屏幕”的“最近项目”部分切换到列表视图
* &amp;lbrack；UI&amp;rbrack；视口显示模式按钮图标始终显示2D/3D

### **5.0.0榛子**

*（发布日期：2025年2月20日）*

**已添加**

* &amp;lbrack；入门&amp;rbrack；新主页，可快速访问学习内容、示例项目、快速操作和最近项目。
* &amp;lbrack；入门&amp;rbrack；使用可从主页和专用面板访问的新快速操作快速入门
* &amp;lbrack；载入&amp;rbrack； &amp;lbrack；Content&amp;rbrack；快速操作是预定义的工作流，可在图层堆叠中填充最常用的图层
* &amp;lbrack；入门&amp;rbrack；可通过新的快速入门菜单、快速操作或自定义项目创建新项目
* &amp;lbrack；入门&amp;rbrack；可通过专用按钮直接从主页创建空项目
* &amp;lbrack；3D 视图&amp;rbrack；新的高级栅格化器和路径跟踪器在Substance生态系统中带来了新的渲染功能（如涂层、光泽、translucency、次表面散射等属性）和视觉一致性
* 现在可以直接在3D视图中访问&amp;lbrack；3D 视图&amp;rbrack；查看器设置
* &amp;lbrack；3D 视图&amp;rbrack；可将渲染快照保存在剪贴板或文件中
* &amp;lbrack；3D 视图&amp;rbrack；显示网格以可视化场景原点
* &amp;lbrack；3D视图&amp;rbrack；启用地平面以捕捉阴影和反射
* &amp;lbrack；3D 视图&amp;rbrack；控制地面平面反射和不透明的程度
* &amp;lbrack；3D 捕捉&amp;rbrack；在地面上定位网格
* &amp;lbrack；Application&amp;rbrack；检查应用程序启动时的硬件兼容性
* &amp;lbrack；Application&amp;rbrack；崩溃报告窗口现在会在崩溃发生后立即打开
* &amp;lbrack；Content&amp;rbrack；打开示例项目以轻松开始
* &amp;lbrack；导出&amp;rbrack；在USD文件中导出Adobe Standard Material着色器
* &amp;lbrack；生成式AI&amp;rbrack；在“图像”中使用“图像”作为纹理工作流程的输入时，请勾选“不推断”标记
* &amp;lbrack；Project&amp;rbrack；缩略图存储在项目文件中，以便快速打开项目
* &amp;lbrack；Project&amp;rbrack；首选项中用于在项目文件中使用不同模式（无缓存、轻缓存、完全缓存）存储缓存数据的设置
* &amp;lbrack；脚本&amp;rbrack； &amp;lbrack；中断change&amp;rbrack； Qt迁移到Qt6.15 — 影响现有插件的兼容性
* &amp;lbrack；Scripting&amp;rbrack；默认插件和脚本文件夹现在位于Documents文件夹中
* &amp;lbrack；脚本编写&amp;rbrack；增效工具的新UI，在视觉上与Sampler主面板保持一致
* &amp;lbrack；脚本编写&amp;rbrack； Access 2个插件示例，以发现Sampler插件功能
* &amp;lbrack；脚本&amp;rbrack； New open_3d_catpure()函数
* &amp;lbrack；脚本编写&amp;rbrack；插入图层时，控制是将其插入目标位置的上方还是下方

**已修复：**

* 无法在macOS上启动对象捕获时，3D 捕捉&amp;rbrack；崩溃
* &amp;lbrack；Application&amp;rbrack；退出时崩溃
* 将资源添加到“项目”面板时，&amp;lbrack；应用程序&amp;rbrack；在退出时挂起
* &amp;lbrack；除非按Enter，否则无法重命名项目资源(&amp;R)
* &amp;lbrack；Application&amp;rbrack；还原和重做菜单项在应该禁用时未禁用
* &amp;lbrack；资源无法从“资源”面板的“所有库”部分中删除资源
* &amp;lbrack；Content&amp;rbrack； Atlas creator — 使用现有不透明度映射（如果存在）
* &amp;lbrack；Content&amp;rbrack；颜色ID混合 — 修复基色拾色问题
* &amp;lbrack；Layers&amp;rbrack；在使用生成器时避免无用的计算
* &amp;lbrack；图层调整&amp;rbrack；调整生成器可能会导致触发太多计算
* &amp;lbrack；性能改进GPU内存管理(&amp;R)
* 重新启动应用程序时，可能无法使用&amp;lbrack；Performance&amp;rbrack；渲染缓存
* &amp;lbrack；资源&amp;rbrack；只读文件在“资源”面板中不可见
* &amp;lbrack；脚本编写&amp;rbrack；允许在添加另一个图层后重新使用图层
* &amp;lbrack；脚本编写&amp;rbrack；在一个脚本中多次更改图层堆叠结构可能会失败

**已删除：**

* &amp;lbrack；Application&amp;rbrack；删除对.dng和.nef图像文件的支持

## 版本4

### **4.5.2 GRUYERE**

*（发布日期：2024年11月7日）*

**已修复：**

* &amp;lbrack；Content&amp;rbrack；裁剪、刺绣和Height混合滤镜

### **4.5.1 GRUYERE**

*（发布日期：2024年7月30日）*

**已修复：**

* &amp;lbrack；图层&amp;rbrack；绘画灰度蒙版不起作用，影响仿制图章、绘画变形、内容识别填充等工具

### **4.5.0 GRUYERE**

*（发布日期：2024年7月18日）*

**已添加**

* &amp;lbrack；互操作性&amp;rbrack；将材料发送到UE5、Blender、Maya、3DsMax Unity
* &amp;lbrack；Content&amp;rbrack；新纹理生成器类别 — 渐变
* &amp;lbrack；Content&amp;rbrack；HDRI 工具 — 新的环境旋转过滤器

**已修复：**

* &amp;lbrack；公开参数&amp;rbrack；公开.sbsar输入值不起作用
* &amp;lbrack；图层&amp;rbrack；Base color在灰度图像上变为红色
* 颜色通道中使用的&amp;lbrack；渲染&amp;rbrack；灰度图像具有错误的色彩空间
* &amp;lbrack；脚本编写&amp;rbrack；使用导出预设有时无法导出预期的通道
* &amp;lbrack；Content&amp;rbrack；Dirt — 在图像上应用Dirt筛选器以材料生成黑色法线
* &amp;lbrack；Content&amp;rbrack；浮雕 — 图案在浮雕滤镜中的缩放比例在0和1之间不是线性的
* &amp;lbrack；Content&amp;rbrack；使其平铺 — 改进了正常和Height一致性

### **4.4.1字体**

*（发布日期：2024年6月6日）*

**已修复：**

* 缺少&amp;lbrack；Content&amp;rbrack；Dirt筛选器
* 使用“图像”纹理时，有时会出现&amp;lbrack；生成式AI&amp;rbrack；网络错误

### **4.4.0字体**

*（发布日期：2024年5月23日）*

**已添加：**

* &amp;lbrack；Application&amp;rbrack；3D 捕捉缓存现在存储在单独的子文件夹中
* 生成式AI&amp;rbrack；图像到纹理(Beta)(&amp;L)
* 生成式AI&amp;rbrack；文本到图案(Beta)(&amp;L)
* 生成式AI&amp;rbrack；纹理化文本(Beta)(&amp;L)
* &amp;lbrack；脚本编写&amp;rbrack；资源现在具有“resource”属性
* &amp;lbrack；脚本编写&amp;rbrack；图层现在具有“output_usages”属性

**已修复：**

* 打开损坏的项目文件时崩溃(&amp;lbrack；Application&amp;rbrack；)
* &amp;lbrack；项目包含损坏资源时的Application&amp;rbrack；崩溃
* 在Windows上拔下监视器时崩溃Application&amp;rbrack；
* Windows任务栏中的&amp;lbrack；Application&amp;rbrack；错误应用程序图标
* &amp;lbrack；应用程序&amp;rbrack；主配置文件损坏会导致文件删除
* 应用程序&amp;brack；面板显示在弹出窗口前面(&amp;L)
* &amp;lbrack；Content&amp;rbrack；纹理生成器的缩览图模糊
* 导出.sbs/.sbsar文件时，从导入的图像生成的不透明度通道中断(&amp;l)
* &amp;lbrack；Filters&amp;rbrack； Upscale可以根据其输入图层崩溃
* &amp;lbrack；生成式AI&amp;rbrack；从服务收到意外结果时可能发生崩溃
* &amp;lbrack；脚本编写&amp;rbrack；从环境变量自动加载插件时崩溃
* &amp;lbrack；脚本编写&amp;rbrack；在API中分配输出使用时可能会崩溃

### **4.3.3 EMPANADA**

*（发布日期：2024年3月26日）*

**已添加：**

* &amp;lbrack；3D 捕捉&amp;rbrack；后期处理过程中新增高级自动UV参数
* &amp;lbrack；滤镜&amp;rbrack；穿孔滤镜：能够反转和更改自定义图案的大小

**已修复：**

* macOS上的&amp;lbrack；3D 捕捉&amp;rbrack；基色可能不正确
* &amp;lbrack；3D 捕捉&amp;rbrack；处理新版本时崩溃
* &amp;lbrack；3D 捕捉&amp;rbrack；后处理步骤可能会在macOS上崩溃
* &amp;lbrack；3D 捕捉&amp;rbrack；网格变换图层可能会导致渲染错误
* &amp;lbrack；Application&amp;rbrack；在前一个实例仍在导出时启动Sampler时崩溃
* 首次启动时，&amp;lbrack；Application&amp;rbrack； Sampler暂时无响应
* &amp;lbrack；Export&amp;rbrack；各向异性角度映射不会导出
* &amp;lbrack；滤镜&amp;rbrack；向图层栈叠中添加布料编织可能导致崩溃
* &amp;lbrack；Filters&amp;rbrack；向图层栈栈添加浮雕可能会导致崩溃
* &amp;lbrack；滤镜&amp;rbrack；内容识别填充在使用32位图像时崩溃
* &amp;lbrack；滤镜&amp;rbrack；浮雕：不能完全覆盖下方图层的不透明度
* &amp;lbrack；滤镜&amp;rbrack；填充：混合模式在Designer和Painter中不起作用
* &amp;lbrack；滤镜&amp;rbrack；刺绣：自动颜色选择损坏
* &amp;lbrack；Preferences&amp;rbrack；防止为3D 捕捉缓存设置不受支持的路径
* &amp;lbrack；Preferences&amp;rbrack； “正常格式”首选项不起作用
* &amp;lbrack；Scripting&amp;rbrack； Asset.export_material的通道参数区分大小写

### **4.3.2 EMPANADA**

*（发布日期：2024年2月22日）*

**已修复：**

* &amp;lbrack；在Windows的网络共享上保存项目会损坏项目文件(&amp;R)

### **4.3.1 EMPANADA**

*（发布日期：2024年2月15日）*

**已修复：**

* 批量生成蒙版时无法访问图像文件时的崩溃(&amp;lbrack；3D 捕捉)&amp;rbrack；
* &amp;lbrack；Export&amp;rbrack；导出带有“裁剪”或相对于输入材料层的策略会产生无效结果
* &amp;lbrack；Layers&amp;rbrack；渲染图层栈栈时发生罕见崩溃
* &amp;lbrack；Filters&amp;rbrack；刺绣 — 修复在MacOS上使用素材输入时出现的问题
* &amp;lbrack；滤镜&amp;rbrack；风格化 — 支持纹理生成器
* &amp;lbrack；滤镜&amp;rbrack；模式 — 修复参数命名
* &amp;lbrack；Localization&amp;rbrack； “另存为……” 在硬件信息窗口中，“帮助”菜单下的菜单未本地化

### **4.3.0 EMPANADA**

*（发布日期：2024年1月25日）*

**已添加**

* &amp;lbrack；资源&amp;rbrack；新资源类型：纹理生成器
* &amp;lbrack；资源&amp;rbrack；入门资源中包含的新材料
* &amp;lbrack；资源&amp;rbrack；在“属性”面板中为图像参数新建资源选择器
* &amp;lbrack；资源&amp;rbrack；将纹理生成器从“资源”面板拖放到“属性”面板中的图像选择器中
* &amp;lbrack；资源&amp;rbrack；从操作系统文件资源管理器拖放纹理生成器
* &amp;lbrack；Assets&amp;rbrack；滤镜可以通过图像输入上的用户标记建议适合生成器
* &amp;lbrack；资源&amp;rbrack；纹理生成器可以定义哪个筛选器应通过用户标记提供建议
* &amp;lbrack；Content&amp;rbrack；新透视裁剪滤镜
* &amp;lbrack；Content&amp;rbrack；新风格化滤镜
* 填充滤镜上的混合模式(&amp;L)&amp;R)
* &amp;lbrack；Content&amp;rbrack；更新的刺绣滤镜
* &amp;lbrack；Content&amp;rbrack；更新了绘画环绕滤镜
* &amp;lbrack；Content&amp;rbrack；更新了所有筛选器以支持纹理生成器
* &amp;lbrack；Layers&amp;rbrack；将生成器输出声道添加到图层堆叠时能够选择纹理生成器输出声道
* &amp;lbrack；Layers&amp;rbrack；能够在纹理生成器上轻松列出和应用预设
* &amp;lbrack；图层&amp;rbrack；在图像选择器中显示纹理生成器预览
* 可以公开和导出&amp;lbrack；图层&amp;rbrack；纹理生成器参数
* &amp;lbrack；Layers&amp;rbrack；在使用Base color导入创建模板导入单个图像时分配纹理使用情况
* 尝试在“属性”面板的图像拾色器中拖放不兼容文件时&amp;lbrack；图层&amp;rbrack；反馈
* &amp;lbrack；Layers&amp;rbrack；从导入图像的Alpha 通道生成不透明度通道
* 更改图像到材料(AI)的类别时，&amp;lbrack；图层&amp;rbrack；的计算速度更快
* &amp;lbrack；图层&amp;rbrack；使用创建模板后选择最相关的图层
* &amp;lbrack；Layers&amp;rbrack；现在可以使用“高级参数”组中的滑块调整位置构件
* &amp;lbrack；Export&amp;rbrack；在队列中显示百分比，而不是原始数字
* &amp;lbrack；互操作性&amp;rbrack；在发送到Painter时，不透明度通道现在被识别为Alpha通道
* &amp;lbrack；用于显示和保存硬件信息的Application&amp;rbrack；新建对话框
* &amp;lbrack；Application&amp;rbrack；用于更改每个项目的默认Height比例的新首选项
* &amp;lbrack；Application&amp;rbrack；改进过时资源的显示方式
* &amp;lbrack；Scripting&amp;rbrack；新asset.documentResolution()和asset.setDocumentResolution()函数
* &amp;lbrack；脚本&amp;rbrack；新select_asset()函数
* 用于纹理生成器的&amp;lbrack；脚本编写&amp;rbrack； Python API
* &amp;lbrack；Scripting&amp;rbrack； get_project_assets()现在可返回3D对象
* &amp;lbrack；可在“资源”面板中更改资源缩略图大小(&amp;R)
* &amp;lbrack；UI&amp;rbrack；更新的视口显示图标

**已修复：**

* &amp;lbrack；2D视图&amp;rbrack；鼠标滚轮缩放在244%处被阻止
* 初始化图形API时在启动时崩溃&amp;lbrack；Application&amp;rbrack；
* 如果项目名称包含#字符，&amp;lbrack；Application&amp;rbrack；崩溃
* 打开旧项目时可能崩溃的&amp;lbrack；Application&amp;rbrack；
* &amp;lbrack；Application&amp;rbrack；重新打开当前项目会导致崩溃
* &amp;lbrack；Application&amp;rbrack；某些项目更改未注册，如果未保存，在关闭项目时将会丢失且不发出警告
* &amp;lbrack；使用多个同名文件时出现Export&amp;rbrack； .sbs/.sbsar导出问题
* &amp;lbrack；导出&amp;rbrack；导出的灰度图像.sbs/.sbsar 文件的色彩空间不正确
* &amp;lbrack；滤镜&amp;rbrack；不透明度混合行为问题
* 有时无法以正确的分辨率渲染&amp;lbrack；图层&amp;rbrack； .svg文件
* &amp;lbrack；Performance&amp;rbrack；不必在磁盘上保存某些项目
* &amp;lbrack；Project&amp;rbrack；导入旧项目时不会加载关联的预设
* &amp;lbrack；脚本编写&amp;rbrack；无法获取第一个插入图层的参数
* &amp;lbrack；UI&amp;rbrack；将资源悬停在错误的位置或屏幕中时可弹出预览
* &amp;lbrack；UI&amp;rbrack；取消停靠的面板在“欢迎”屏幕顶部可见且可用

### **4.2.2多拉亚基**

*（发布日期：2023年12月5日）*

**已添加：**

* &amp;lbrack；3D 捕捉&amp;rbrack；3D 捕捉在Windows上的速度现在提高了5%到10%
* &amp;lbrack；3D 捕捉&amp;rbrack；在抽取前改善网格清理
* &amp;lbrack；引擎&amp;rbrack；将Substance 引擎更新到9.0.3版
* &amp;lbrack；Layers&amp;rbrack；内容识别填充：上游更新、各种用例修复和Linux支持

**已修复：**

* &amp;lbrack；3D 捕捉&amp;rbrack；在对齐后单击“返回”再单击“下一步”不会更新点云
* &amp;lbrack；3D 捕捉&amp;rbrack；添加到项目后显示有孔的网格
* 在3D 捕捉后退出全屏模式时&amp;lbrack；Application&amp;rbrack；崩溃
* &amp;lbrack；应用程序&amp;rbrack；使用精心编制的图像文件时崩溃
* &amp;lbrack；Application&amp;rbrack；如果退出Sampler时位于“所有库”中，则“资源”面板在重新启动时将为空
* 导出材料时出现&amp;lbrack；Application&amp;rbrack；内存泄漏
* &amp;lbrack；Application&amp;rbrack；打开使用以前Sampler版本保存的项目可能会导致崩溃
* &amp;lbrack；Application&amp;rbrack；无法转换3D网格时的潜在崩溃
* &amp;lbrack；在Sampler运行时打开.sbsar时的Application&amp;rbrack；静音崩溃
* 导出具有自定义用途的.sbs/.sbsar 文件时，导出&amp;rbrack；崩溃
* &amp;lbrack；Export&amp;rbrack；导出的正常映射始终DirectX，无论用户如何设置
* &amp;lbrack；Export&amp;rbrack；在macos上将3D对象导出为FBX文件不起作用
* &amp;lbrack；Export&amp;rbrack；将带有刺绣滤镜的图层堆叠导出为.sbs/.sbsar 文件时出现不一致
* &amp;lbrack；Export&amp;rbrack；有时无法导出.sbs/.sbsar文件
* &amp;lbrack；Export&amp;rbrack；导出.sbs/.sbsar文件图像时，有时没有正确的位深度
* &amp;lbrack；Layers&amp;rbrack；使“飞溅”图层不可见会改为渲染其第一个子图层
* 在亮度/对比度图层中加载蒙版时，图层&amp;rbrack；崩溃(&amp;L)
* 删除图层后显示误导性错误消息(&amp;L)
* Lbrack；Layers&amp;rbrack；降级资源时可能会崩溃(&amp;L)
* &amp;lbrack；Layers&amp;rbrack；某些输出未连接到输入，除非在“通道设置”面板中强制使用
* &amp;lbrack；物理尺寸&amp;rbrack；参考图层下拉菜单可能会错误地重置
* &amp;lbrack；UI&amp;rbrack；导入模板信息图标需要更新
* &amp;lbrack；UI&amp;rbrack；视口快捷键提示每次视口布局更改时都会出现

### **4.2.1多拉亚基**

*（发布日期：2023年9月21日）*

**已添加：**

* 将&amp;lbrack；Content&amp;rbrack；图像转换为材料 — 改进法线图中微细节的生成
* &amp;lbrack；Content&amp;rbrack；图像到材料 — 新的愉悦强度参数
* 可以在图像导入图层中添加图像(&amp;L)&amp;R)
* 可以在“图像导入”图层中删除&amp;lbrack；图层&amp;rbrack；图像
* 现在可以删除无效的图层(&amp;L)
* 按Shift+C组合键循环切换声道(&amp;L)；2D 视图(&amp;R)；快捷键(&amp;R)
* &amp;lbrack；3D 捕捉&amp;rbrack；当用户导入的图像数少于20个时显示警告toast
* &amp;lbrack；Application&amp;rbrack；用于设置默认纹理拼贴值的新首选项
* &amp;lbrack；上线&amp;rbrack；更新了图像到材料(AI)和升级的教程UI
* &amp;lbrack；脚本&amp;rbrack；3D 捕捉API：将Capture3dState设置为对齐时，DatasetInfo包含更多数据
* &amp;lbrack；脚本编写&amp;rbrack；将select_asset参数新增到create_asset()。 新函数：wait_for_recover()和clear_render_cache()计算

**已修复：**

* &amp;lbrack；裁剪区域非常小时的图层&amp;rbrack；崩溃
* 添加或调整“裁剪”滤镜时的&amp;lbrack；图层&amp;rbrack；崩溃
* &amp;lbrack；图层&amp;rbrack；使裁剪区域变成方形会导致材料输出分辨率不正确
* 禁用多个图层时，&amp;lbrack；图层和rbrack；输出有时会消失
* &amp;lbrack；Layers&amp;rbrack；渲染缓存可能无法通过“要材料的图像(AI)”和“放大”滤镜正确失效
* &amp;lbrack；Layers&amp;rbrack；在警告弹出窗口中选择“不再显示此消息”时，无法添加“放大”滤镜
* &amp;lbrack；图层&amp;rbrack；修改后，无法恢复刺绣滤镜中的图像
* &amp;lbrack；Export&amp;rbrack；更改标准法线图时，导出的格式分辨率发生变化
* &amp;lbrack；导出&amp;rbrack；导出环境时删除“\_environment”文件名后缀
* &amp;lbrack；Export&amp;rbrack；图层堆叠中存在变形变换图层时无法导出。sbsar 文件
* 分辨率更改时，&amp;lbrack；2D 视图&amp;rbrack；“适合屏幕”不起作用
* &amp;lbrack；Application&amp;rbrack；在计算时关闭应用程序窗口后，应用程序进程仍可能正在运行
* 退出时崩溃&amp;lbrack；应用程序&amp;rbrack；
* &amp;lbrack；切换GPU加速神经网络时，Application&amp;rbrack；使渲染缓存失效
* &amp;lbrack；脚本编写&amp;rbrack；将插件命名为现有面板名称会导致意外行为
* &amp;lbrack；UI&amp;rbrack；单击带有工具提示的项目会导致工具提示消失直到重新启动
* 切换资源时，&amp;lbrack；UI&amp;rbrack；Height缩放值可能会更改
* 组合框中的&amp;lbrack；UI&amp;rbrack；边距不正确

### **4.2道拉亚基**

*（发布日期：2023年9月5日）*

**已添加：**

* &amp;lbrack；Content&amp;rbrack；极大地改进了“图像到材料”(AI)和Delighter滤镜
* &amp;lbrack；Content&amp;rbrack；新建放大滤镜
* &amp;lbrack；Content&amp;rbrack； “裁剪”滤镜现在具有动态输出分辨率。
* &amp;lbrack；材料创建模板&amp;rbrack；添加文档大小设置。
* &amp;lbrack；材料创建模板&amp;rbrack；新的“添加裁剪”切换按钮。
* &amp;lbrack；材料创建模板&amp;rbrack；新的“放大材料”切换
* &amp;lbrack；材料创建模板&amp;rbrack；显示导入的图像大小
* &amp;lbrack；材料创建模板&amp;rbrack；在某些导入的图像无法使用时提供反馈
* &amp;lbrack；材料创建模板&amp;rbrack；图像大小不一致时发出警告
* &amp;lbrack；材质创建模板&amp;rbrack；新警告和工具提示
* &amp;lbrack；图层&amp;rbrack；显示图层栈栈中图层的分辨率
* &amp;lbrack；图层&amp;rbrack；图层计算分辨率现在可以设置为“文档大小”或“输入大小”
* layers&amp;rbrack；在图层栈栈中显示图层分辨率(&amp;L)
* &amp;lbrack；Layers&amp;rbrack；在适用时将图层分辨率策略切换为“文档”或“图层输入”
* &amp;lbrack；Layers&amp;rbrack；手动添加“放大”滤镜时警告用户并提供一些文档
* &amp;lbrack；Layers&amp;rbrack；在线性放大时警告用户，并建议改用“放大”滤镜
* &amp;lbrack；图层&amp;rbrack；现在可以更快地取消计算图像到材质(AI)图层，以便缩短调整图层栈栈时的渲染时间
* &amp;lbrack；Layers&amp;rbrack；现在可以更快地取消计算放大图层，以缩短调整图层栈栈时的渲染时间
* &amp;lbrack；Export&amp;rbrack；允许覆盖导出纹理的分辨率
* &amp;lbrack；Export&amp;rbrack；导出列表的通道现在已排序
* &amp;lbrack；Export&amp;rbrack；在要导出的通道列表中显示通道分辨率
* &amp;lbrack；Application&amp;rbrack；用于启用或禁用GPU加速神经网络的新首选项
* &amp;lbrack；UI&amp;rbrack；改进的分辨率下拉菜单
* &amp;lbrack；UI&amp;rbrack；用于网格变换、网格后期处理和编织滤镜的新图标
* &amp;lbrack；UI&amp;rbrack；将“共享”面板重命名为“导出”
* &amp;lbrack；脚本编写&amp;rbrack；将图层输出分辨率支持添加到导出API
* &amp;lbrack；Scripting&amp;rbrack；为图像导入API添加了裁剪、放大和文档大小
* 加载；上线&amp;加载；新教程(&amp;L)
* &amp;lbrack；入门&amp;rbrack；更新欢迎和新增功能屏幕内容
* &amp;lbrack；Engine&amp;rbrack；将Substance 引擎更新到版本9.0.1

**已修复：**

* &amp;lbrack；3D 捕捉&amp;rbrack；改进对齐方式设置参数中的精度选项命名
* &amp;lbrack；Application&amp;rbrack；导入16维度的非倍数图像可能会导致崩溃
* 在“项目”面板中复制资源时&amp;lbrack；Application&amp;rbrack；崩溃
* 在“项目”面板中切换资源时&amp;lbrack；Application&amp;rbrack；崩溃
* 为Snow滤镜绘制自定义蒙版时&amp;lbrack；Content&amp;rbrack；无法正常工作
* &amp;lbrack；公开的参数&amp;rbrack；在切换材质时公开的参数更改可能会丢失
* &amp;lbrack；互操作性&amp;rbrack；从“导出”面板发送材料可能会导致崩溃
* 从单个图像输入切换到材质输入时，&amp;lbrack；图层&amp;rbrack；内容识别填充停止计算
* &amp;lbrack；图层&amp;rbrack；复制包含素材的环境光后崩溃
* 如果重命名了图像文件，&amp;lbrack；图层&amp;rbrack；图像导入图层在“属性”面板中显示错误的图像名称
* &amp;lbrack；Layers&amp;rbrack；有时会在非活动图层上显示旋转器
* &amp;lbrack；Layers&amp;rbrack；有时在图像导入图层中更改图像的输出使用方式不起作用
* &amp;lbrack；Layers&amp;rbrack；创建模板窗口中的拼写错误
* &amp;lbrack；UI&amp;rbrack； 3D视口入门工具提示有焦点问题
* 如果文件名太长，&amp;lbrack；UI&amp;rbrack；图像名称可能会溢出
* 使用橡皮擦时出现的&amp;lbrack；UI&amp;rbrack；次要画笔工具栏布局问题
* 在“查看器设置”面板中，某些语言的&amp;lbrack；UI&amp;rbrack；字符串被截断
* &amp;lbrack；UI&amp;rbrack；在显示视口工具提示弹出窗口时，按“空格”键可创建新项目

### **4.1.2坎诺利**

*（发布日期：2023年6月20日）*

**已修复：**

* 调整材料和过滤器时内存泄漏(&amp;lbrack；Layers&amp;rbrack；)，导致崩溃

### **4.1.1坎诺利**

*（发布日期：2023年6月6日）*

**已添加**

* &amp;lbrack；引擎&amp;rbrack；将Substance 引擎更新到版本9.0
* &amp;lbrack；互操作性&amp;rbrack；将3D对象发送到Stager和Painter

**已修复：**

* 3D 捕捉渲染器失败时崩溃的&amp;lbrack；3D 捕捉&amp;rbrack；
* &amp;lbrack；无法加载图像时的3D 捕捉&amp;rbrack；崩溃
* 达到网格重构步骤时崩溃3D 捕捉(&amp;lbrack；R)
* 调整定界框大小时的崩溃(&amp;l)；3D 捕捉(&amp;r)
* &amp;lbrack；按照约定导入蒙版时，无法正确分配蒙版(&amp;R)；3D 捕捉&amp;R
* &amp;lbrack；调整定界框时3D 捕捉&amp;rbrack；渲染出错
* &amp;lbrack；3D 捕捉&amp;rbrack；在3D 捕捉后期处理期间在版本之间切换和切换渲染选项时速度缓慢
* 在3D 捕捉后处理步骤期间在版本之间切换有时会中断(&amp;lbrack；3D 捕捉(&amp;rbrack)
* Lbrack；Application&amp;rbrack；启动时崩溃
* 复制重命名的材质时&amp;lbrack；Application&amp;rbrack；崩溃
* &amp;lbrack；Application&amp;rbrack；打开旧版.alch项目（不带其依赖项文件夹）时崩溃
* &amp;lbrack；Application&amp;rbrack；在插入/拔出屏幕、计算机进入睡眠状态或远程访问时崩溃
* &amp;lbrack；应用程序崩溃&amp;rbrack；与非持久性资产管理相关的崩溃和内存泄漏
* &amp;lbrack；Export&amp;rbrack；应禁用为嵌入或引用纹理的3D对象文件类型选择材质格式
* &amp;lbrack；导出&amp;rbrack；在3D对象导出期间发生错误时崩溃
* 导出.sbs/.sbsar文件时&amp;lbrack；Export&amp;rbrack；崩溃
* &amp;lbrack；Export&amp;rbrack；在导入具有相同标签但文件名不同的自定义预设时崩溃
* &amp;lbrack；Export&amp;rbrack；将环境光导出到.sbs/.sbsar文件有时不起作用
* &amp;lbrack；Export&amp;rbrack； Gltf/Glb导出为base64中的纹理编码
* 重新聚焦时，&amp;lbrack；Export&amp;rbrack；名称文本字段不起作用
* 将图像导出到材料（AI驱动）图层到.sbs/.sbsar 文件时，&amp;lbrack；Export&amp;rbrack；保留拼贴不起作用
* &amp;lbrack；Export&amp;rbrack；导出gltf并替换文件时，要替换的文件列表不正确
* &amp;lbrack；公开的参数&amp;rbrack；随机植入在导出的.sbs/.sbsar文件中不起作用
* &amp;lbrack；Layers&amp;rbrack；内容识别填充有时会在第二次添加时崩溃
* &amp;lbrack；Layers&amp;rbrack；计算图层栈栈时崩溃
* &amp;lbrack；图层&amp;rbrack；图像到材质(AI)磁盘缓存不起作用
* &amp;lbrack；图层&amp;rbrack；调整图层时可能崩溃
* 回栈；性能&amp;回栈；内存泄漏(&amp;L)
* &amp;lbrack；保存项目时项目&amp;rbrack；崩溃
* &amp;lbrack；Project&amp;rbrack；在一行中导入同一项目两次会复制资源
* &amp;lbrack；UI&amp;rbrack；仅带图标的圆角按钮无法正确渲染

### 4.1.0坎诺利

*（发布日期：2023年3月28日）*

**已添加：**

* 标记；内容标记；新建刺绣滤镜(&amp;R)
* 标记；内容标记；新建绘画变形滤镜(&amp;R)
* &amp;lbrack；UI&amp;rbrack；在“文件”菜单中添加导出选项
* 现在可在对齐步骤中使用&amp;lbrack；3D 捕捉&amp;rbrack；后退按钮
* &amp;lbrack；3D 捕捉&amp;rbrack；图像处理JPEGEXIF方向
* &amp;lbrack；3D 捕捉&amp;rbrack；脚本 — 新dataset_info.camera属性
* &amp;lbrack；3D 捕捉&amp;rbrack；添加Linux支持（请参阅文档）
* &amp;lbrack；3D 捕捉&amp;rbrack；验证导入图像的读取权限
* 教程&amp;lbrack；上线&amp;rbrack；学习 — 2个新教程（“刺绣”和“绘画变形”）
* &amp;lbrack；载入&amp;rbrack；更新了新增内容

**已修复：**

* &amp;lbrack；3D 捕捉&amp;rbrack；更改版本时保持相机位置
* &amp;lbrack；3D 捕捉&amp;rbrack；将对象的所有组合并为一个组
* &amp;lbrack；3D 捕捉&amp;rbrack；重命名的生成网格到原始网格中
* &amp;lbrack；Application&amp;rbrack；尝试生成不存在的图像的缩略图时崩溃
* 资源回收箱图标在资源面板中不执行任何操作(&amp;L)
* &amp;lbrack；Content&amp;rbrack；更新带有材质槽的过滤器无法按预期工作
* &amp;lbrack；Export&amp;rbrack；导出具有特定滤镜的资源时可能会崩溃
* &amp;lbrack；导出&amp;rbrack； SBS/SBSAR导出 — 图像导入图层优先于图像参数
* &amp;lbrack；Export&amp;rbrack； UE4 Export预设不适用于PNG
* &amp;lbrack；Layers&amp;rbrack；从OS资源管理器中同时删除素材和滤镜时崩溃
* &amp;lbrack；Layers&amp;rbrack；在使用任何图像文件拖动任何SBSAR文件时崩溃
* &amp;lbrack；图层&amp;rbrack；刺绣不透明度通道可以是全白色
* 在Linux上，默认显示中文语言(&amp;L)
* &amp;lbrack；Performance&amp;rbrack；修复了从资源中删除图层时的内存问题
* &amp;lbrack；保存时可能崩溃的项目&amp;rbrack；
* &amp;lbrack；UI&amp;rbrack；在“版本”菜单按钮上添加缺失间距
* 无法正确显示&amp;lbrack；UI&amp;rbrack；取消按钮
* &amp;lbrack；UI&amp;rbrack；禁用3D 捕捉后处理参数的滑块动画
* &amp;lbrack；UI&amp;rbrack；在外部单击时，“材料创建模板”窗口不会自行关闭
* &amp;lbrack；UI&amp;rbrack；在外部单击时，筛选器快速访问器会自行关闭

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

### 4.0.2香蕉

*（发布日期：2023年3月9日）*

**已添加：**

* &amp;lbrack；3D 捕捉&amp;rbrack；磁盘使用情况显示使用的数量
* &amp;lbrack；3D 捕捉&amp;rbrack；导入照片是异步操作，而且速度更快
* &amp;lbrack；脚本编写&amp;rbrack；用于编写3D 捕捉功能脚本的新类和函数
* &amp;lbrack；脚本&amp;rbrack；在导出完成、失败或取消时执行操作的新ExportController类
* &amp;lbrack；脚本编写&amp;rbrack；传递参数python脚本与 — run-script一起运行
* 在图层面板上拖动资源时&amp;lbrack；UI&amp;rbrack； UI反馈
* &amp;lbrack；Content&amp;rbrack；色温滤镜现在可以在材料上工作
* &amp;lbrack；Content&amp;rbrack；正常使用Height滤镜时有一个保留拼贴的新选项

**已修复：**

* &amp;lbrack；3D 捕捉&amp;rbrack；数据集对齐步骤中校正的图像大小
* &amp;lbrack；3D 捕捉&amp;rbrack；在UV展开后删除重复顶点
* &amp;lbrack；3D 捕捉&amp;rbrack； MacOS — 如果3D 捕捉可用，可更好地检测
* 导入图像时关闭3D 捕捉窗口时&amp;lbrack；3D 捕捉&amp;rbrack；崩溃
* 生成新版本时崩溃&amp;lbrack；3D 捕捉&amp;rbrack；
* 尝试在查看器中加载3D对象时崩溃&amp;lbrack；3D 捕捉&amp;rbrack；
* 使用含有非UTF8字符的3D 捕捉时出现&amp;lbrack；崩溃(&amp;r)
* &amp;lbrack；3D 捕捉&amp;rbrack；命中与提示拼写错误
* &amp;lbrack；3D 捕捉&amp;rbrack；网格不再进行缩放以适应单位多维数据集
* &amp;lbrack；3D 捕捉&amp;rbrack；在渲染时关闭3D 捕捉时防止崩溃
* &amp;lbrack；3D 捕捉&amp;rbrack；移除蒙版会使图像消失
* 同时导入两次资源时的崩溃(&amp;L)
* &amp;lbrack；Application&amp;rbrack；在打开项目时备份以前版本的资源（如果从未备份过）
* &amp;lbrack；Application&amp;rbrack；在未烘焙所有映射时正确缓存已烘焙贴图
* 显示3D对象时，&amp;lbrack；Application&amp;rbrack；全屏崩溃。
* &amp;lbrack；保存项目时复制上一个材料(&amp;R)
* &amp;lbrack；Application&amp;rbrack；在烘焙步骤中取消网格后处理计算时防止崩溃
* &amp;lbrack；Application&amp;rbrack；重新打开当前项目不会放弃更改
* &amp;lbrack；应用程序&amp;rbrack；停止生成3D对象的缩览图
* 使用画笔崩溃时2D 视图(&amp;l)
* &amp;lbrack；内容识别填充 — 计算可能会卡住
* &amp;lbrack；Content&amp;rbrack； Atlas Creator滤镜正在缩小不透明度通道
* &amp;lbrack；导出&amp;rbrack；修复清除失败的导出队列
* &amp;lbrack；Export&amp;rbrack； OBJ导出创建的对象比预期小100倍
* 导入为灰度通道的彩色图像现在被视为灰度(&amp;L)
* 无法在第三方应用程序中导入&amp;lbrack；Export&amp;rbrack； FBX文件
* USD文件中的&amp;lbrack；Export&amp;rbrack；着色器输出名称不正确
* 在操作系统资源管理器上更改图像名称时，不会更新图像名称(&amp;L)
* &amp;lbrack；脚本编写&amp;rbrack；重新加载无效脚本时显示错误消息
* &amp;lbrack；UI&amp;rbrack；基础材质按钮在不可用时禁用
* 访问“材料创建模板”窗口上的“文件”对话框时崩溃(&amp;lbrack；UI&amp;rbrack；)
* 即使关闭“图层”面板，也可以访问&amp;lbrack；UI&amp;rbrack；快速访问器
* &amp;lbrack；UI&amp;rbrack；发送至图标未对齐
* &amp;lbrack；UI&amp;rbrack；单击混合图标时，图层图标会发生变化

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* 发送给Stager的位移的&amp;lbrack；互操作性&amp;rbrack；材料将失去位移控制

### 4.0.1香蕉

*（发布日期：2023年2月7日）*

**已修复：**

* &amp;lbrack；3D 捕捉&amp;rbrack；使用蒙版时，纹理投影可能已损坏
* 对象上可能会出现&amp;lbrack；3D 捕捉&amp;rbrack；伪像
* &amp;lbrack；3D 捕捉&amp;rbrack；导出的网格可能非常小

**已知问题：**

* &amp;lbrack；3D 捕捉&amp;rbrack； FBX和OBJ导出会缩小结果
* 即使您的硬件不兼容，&amp;lbrack；3D 捕捉&amp;rbrack；3D 捕捉在MacOS上也可用。 请查看文档。
* &amp;lbrack；3D 捕捉&amp;rbrack；完成网格重建时崩溃。
* 如果微调下方的图层，&amp;lbrack；图层&amp;rbrack；内容识别填充可能会卡住
* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

### 4.0.0香蕉

*（发布日期：2023年1月31日）*

**已添加：**

* &amp;lbrack；3D 捕捉&amp;rbrack；从图像创建3D对象
* &amp;lbrack；3D 捕捉&amp;rbrack；专用3D 捕捉向导
* &amp;lbrack；3D 捕捉&amp;rbrack；在数据集上导入或生成黑白色蒙版
* &amp;lbrack；3D 捕捉&amp;rbrack；对齐结果 — 将所有匹配功能作为点云查看
* &amp;lbrack；3D 捕捉&amp;rbrack；对齐结果 — 查看每个对齐照片关联的相机并与之交互
* &amp;lbrack；3D 捕捉&amp;rbrack；使用定界框构件定义重建区域
* &amp;lbrack；3D 捕捉&amp;rbrack；在所有轴上缩放、平移和旋转定界框构件(&amp;l)
* &amp;lbrack；3D 捕捉&amp;rbrack；定义重构网格的几何精度
* &amp;lbrack；3D 捕捉&amp;rbrack；通过创建新版本来优化网格和纹理
* &amp;lbrack；3D 捕捉&amp;rbrack；每个版本都会自动缩减为设定的目标脸部号
* &amp;lbrack；3D 捕捉&amp;rbrack；后处理步骤自动展开并重新投影纹理，然后烘焙高多边形网格中的正常Height和AO信息
* &amp;lbrack；3D 捕捉&amp;rbrack；将原始结果或版本添加到Sampler项目
* &amp;lbrack；3D 捕捉&amp;rbrack；新建网格后期处理图层以自动清理、展开、重新投影纹理并烘焙底层网格图层的详细信息
* &amp;lbrack；3D 捕捉&amp;rbrack；新建网格变换图层以缩放、旋转或平移底层网格图层
* &amp;lbrack；Export&amp;rbrack；新建导出窗口
* &amp;lbrack；导出&amp;rbrack；专用设置和UI，具体取决于资源类型(材料、环境光、网格)
* &amp;lbrack；导出&amp;rbrack；将网格导出为USD、USDA、USDZ、glTF、glb、obj、fbx、stl
* &amp;lbrack；Export&amp;rbrack；在导出材料文件时定义Substance类型(SBSAR、SBS)
* &amp;lbrack；UI&amp;rbrack；在“首选项”弹出窗口中将缓存设置移动到新选项卡
* 现在可以对2D和3D视口进行垂直调整、交换和栈叠(&amp;lbrack)
* &amp;lbrack；Application&amp;rbrack；用于添加额外入门资源的新SAMPLER_RESOURCES_PATH环境变量
* &amp;lbrack；Scripting&amp;rbrack；添加了SAMPLER_PLUGIN_PATH和SAMPLER_SCRIPT_PATH环境变量，以便在启动时导入增效工具和脚本
* &amp;lbrack；脚本编写&amp;rbrack；添加了材料、环境光和3d对象的导出功能
* &amp;lbrack；脚本编写&amp;rbrack；向参数添加了标识符、默认值、最小值和最大值、标签以及枚举值
* &amp;lbrack；Scripting&amp;rbrack；添加了import_informations函数，可在导入图像时输入自定义用法纹理

**已修复：**

* 打开最近的项目并在确认对话框中保存时崩溃&amp;lbrack；Application&amp;rbrack；
* Application&amp;rbrack；的“文件”对话框阻止打开.ssa文件(&amp;L)
* &amp;lbrack；Application&amp;rbrack；文件对话框可以在macOS的后台窗口中显示
* 打开3.2项目时的潜在崩溃(&amp;lbrack；Application&amp;rbrack；)
* &amp;lbrack；Application&amp;rbrack；选择文件会在显示警告之前关闭“文件”对话框
* &amp;lbrack；公开参数&amp;rbrack；导出参数环境光不起作用
* 图层堆叠中的&amp;lbrack；Layers&amp;rbrack；“单击此处浏览”链接不再有效
* 有时无法在同一图层中绘制多个图像(&amp;L)
* &amp;lbrack；图层&amp;rbrack；在图层属性中设置图像不会更新图像选择器缩览图
* &amp;lbrack；Layers&amp;rbrack；微调添加为图层的Sampler资源不起作用
* 打开项目时&amp;lbrack；Project&amp;rbrack；不需要的资源更新
* &amp;lbrack；脚本编写&amp;rbrack；在Windows上，浏览到插件文件夹有时会失败
* 在Python脚本中使用&#39;open_project()&#39;时执行&amp;lbrack；脚本&amp;rbrack；崩溃
* API中缺少&amp;lbrack；脚本编写&amp;rbrack；JPEG导出
* &amp;lbrack；脚本&amp;rbrack； “日志”面板不是只读的
* &amp;lbrack；脚本编写&amp;rbrack； image_picker参数值不起作用
* &amp;lbrack；UI&amp;rbrack；在“项目”面板中缺少环境光的资源图标
* 首选项弹出窗口中的&amp;lbrack；UI&amp;rbrack；发送到Designer格式下拉菜单可以为空
* &amp;lbrack；UI&amp;rbrack；某些按钮的样式不正确
* &amp;lbrack；UI&amp;rbrack；标签与按钮组小组件中的按钮重叠
* &amp;lbrack；UI&amp;rbrack；工具提示位置对于“设置物理尺寸”菜单中的“工具”是错的
* &amp;lbrack；UI&amp;rbrack；更改语言时，“文件”菜单未对齐

**已知问题：**

* &amp;lbrack；3D 捕捉&amp;rbrack；使用蒙版时，纹理投影可能会损坏
* 如果变换中的缩放比例太小，则对象上可能会出现小的伪影(&amp;lbrack；3D 捕捉)(&amp;r)
* &amp;lbrack；3D 捕捉&amp;rbrack；导出的网格可能非常小。 重置网格变换的比例并重新导出
* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

## 版本3

### 3.4.1阿兰奇尼

*（发布日期：2022年10月6日）*

**已添加：**

* &amp;brack；载入&amp;brack；新欢迎屏幕和新增功能
* &amp;lbrack；上线&amp;rbrack；更新的主屏幕UI
* 主屏幕中的&amp;lbrack；用户引导&amp;rbrack；新学习内容
* &amp;lbrack；脚本编写&amp;rbrack；在无法识别方法时，在“日志”面板中记录错误
* &amp;lbrack；脚本编写&amp;rbrack；新建ssa.助手模块以启用打印到“日志”面板
* &amp;lbrack；Application&amp;rbrack；支持Substance 3D Designer中新增的并排按钮Widget

**已修复：**

* 导出.lbrack；引用缺失图像的。sbsar 文件时导出&amp;rbrack；崩溃
* 导出引用损坏图像文件的资源时，导出&amp;rbrack；崩溃
* &amp;lbrack；导出&amp;rbrack；导出带有刺绣图层的.sbsar文件时生成灰色素材
* &amp;lbrack；导出&amp;rbrack；将素材导出为.sbs/sbsar文件可以生成完全透明的素材
* &amp;lbrack；Export&amp;rbrack； Normal Format参数未在.sbs/.sbsar文件中正确显示
* &amp;lbrack；导出&amp;rbrack；引用.svg文件的图层栈栈的Sbs/sbsar导出被破坏
* &amp;lbrack；导出&amp;rbrack；变换图层未正确导出/已更新的Enscape — 重新导出预设
* &amp;lbrack；公开的参数&amp;rbrack；删除包含公开的参数的图层时崩溃
* &amp;lbrack；公开参数&amp;rbrack；更新图层栈栈中的过时图层可能会导致公开参数的列表损坏
* 仍应导出不应导出的公开参数(&amp;L)
* &amp;lbrack；公开参数&amp;rbrack；删除图层时删除混合滤镜不会取消公开其参数
* &amp;lbrack；公开参数&amp;rbrack；文本参数中断.sbs/.sbsar导出
* 将图层栈栈放到另一个图层栈栈中时&amp;lbrack；图层崩溃(&amp;R)
* &amp;lbrack；Layers&amp;rbrack；无法加载筛选器时崩溃
* 重置图像字段时&amp;lbrack；Layers&amp;rbrack；无法重新加载上一个图像
* &amp;lbrack；图层&amp;rbrack；无法撤消/重做变换工具更改
* 单击“复位所有设置”后&amp;lbrack；图层仿制图章图层卡住(&amp;R)
* &amp;lbrack；Layers&amp;rbrack；使用任何重置按钮都会防止在“图像”字段中绘制
* &amp;lbrack；Layers&amp;rbrack； “重置”按钮不清除“图像”字段中的绘图蒙版
* &amp;lbrack；Layers&amp;rbrack； “图像”字段中的“重置”按钮在用户已绘制某些内容的情况下不起作用
* 使用画笔工具时，&amp;lbrack；图层渲染缓存不起作用(&amp;R)
* 已删除的图层仍可在“属性”面板中显示(&amp;L)
* 在项目资源之间切换时，&amp;lbrack；图层&amp;rbrack；图层计算可能会停滞
* &amp;lbrack；Project&amp;rbrack；有时，Sampler无法从磁盘打开项目
* &amp;lbrack；2D视图&amp;rbrack；2D视图始终默认为材质输出

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

### 3.4.0阿兰奇尼

*（发布日期：2022年9月6日）*

**已添加：**

* &amp;lbrack；公开参数&amp;rbrack；新公开参数面板
* &amp;lbrack；公开参数&amp;rbrack；参数悬停时的新建按钮可在“属性”面板中公开和取消公开参数
* &amp;lbrack；公开参数&amp;rbrack；新增右键单击参数上下文菜单，以从“属性”面板公开和取消公开参数
* 公开参数面板中列出了&amp;lbrack；公开参数&amp;rbrack；公开参数
* &amp;lbrack；公开参数&amp;rbrack；色点和色盘添加到多个位置以轻松识别公开参数
* 可以在公开参数面板中编辑&amp;lbrack；公开参数&amp;rbrack；参数标签
* &amp;lbrack；公开参数&amp;rbrack；显示不可导出参数的警告
* &amp;lbrack；公开参数&amp;rbrack；如果将带有公开混合参数的图层移动到隐藏位置，则会显示警告
* &amp;lbrack；公开参数&amp;rbrack；公开参数以SBS和SBSAR格式导出
* &amp;lbrack；元数据&amp;rbrack；支持自定义元数据模板
* &amp;lbrack；元数据&amp;rbrack；新建CLO物理属性元数据模板
* &amp;lbrack；元数据&amp;rbrack；在悬停时添加图标以添加/删除自定义元数据
* &amp;lbrack；Python API&amp;rbrack；新Python API
* &amp;lbrack；用于创作资源的Python API&amp;rbrack； API
* &amp;lbrack；用于图层管理的Python API&amp;rbrack； API
* &amp;lbrack；用于参数管理的Python API&amp;rbrack； API
* &amp;lbrack；用于项目管理的Python API&amp;rbrack； API
* &amp;lbrack；Python API&amp;rbrack；插件可以启用和禁用
* &amp;lbrack；Python API&amp;rbrack； Python API文档可在“帮助”菜单中访问
* &amp;lbrack；脚本&amp;rbrack；“首选项”弹出窗口中的“新建插件和脚本”部分
* &amp;lbrack；脚本编写&amp;rbrack；创建和导入插件以自定义Sampler界面和您自己的面板
* &amp;lbrack；Scripting&amp;rbrack；增效工具将成为Sampler界面的一部分，可以像标准Sampler面板一样停放和移动
* &amp;lbrack；脚本&amp;rbrack；Sampler右侧工具栏上插件的专用按钮栏
* &amp;lbrack；脚本编写&amp;rbrack；创建并导入脚本以执行给定任务的列表
* &amp;lbrack；脚本&amp;rbrack；通过脚本菜单启动Python脚本
* &amp;lbrack；脚本编写&amp;rbrack；插件和脚本可以从“首选项”窗口删除、重新排序和重新加载
* &amp;lbrack；脚本编写&amp;rbrack；已添加 — run-script命令行参数
* &amp;lbrack；日志&amp;rbrack；新建日志面板
* &amp;lbrack；日志&amp;rbrack；从“首选项”窗口启用“日志”面板
* &amp;lbrack；日志&amp;rbrack；用于清除、复制/粘贴、导出日志的新操作栏
* &amp;lbrack；属性&amp;rbrack；参数悬停时的新建按钮可重置参数值
* &amp;lbrack；属性&amp;rbrack；对参数新增右键单击上下文菜单以重置参数值
* &amp;lbrack；Content&amp;rbrack；图像到材料（AI支持）现在可在MacOS上使用
* &amp;lbrack；引擎&amp;rbrack；将Substance引擎更新到8.6.0版

**已修复：**

* &amp;lbrack；Application&amp;rbrack；在生成缩略图时，应用程序可能会在退出时崩溃
* 退出时使用“另存为”时，应用程序可能崩溃(&amp;L)
* 在MacOS上关闭时，应用程序可能挂起(&amp;L)
* &amp;lbrack；Application&amp;rbrack；在打开颜色对话框的情况下保存不会保存其更改
* &amp;lbrack；导出时，Export&amp;rbrack；使用命名约定不正确
* &amp;lbrack；Layers&amp;rbrack；将素材放到滤镜之上可能会崩溃
* &amp;lbrack；图层&amp;rbrack；更新过时的图层栈栈可能会更新不相关的图层栈栈
* &amp;lbrack；导出元数据&amp;rbrack；空字段
* &amp;lbrack；Metadata&amp;rbrack；当只有一个元数据项时，用户界面允许您尝试对其重新排序
* &amp;lbrack；Project&amp;rbrack；计算在复制材质后永不结束
* &amp;lbrack；初始项目保存后复制项目资源(&amp;R)
* &amp;lbrack；切换资源时，项目和rbrack；不必要的计算
* &amp;lbrack；渲染&amp;rbrack；某些图层堆叠在删除图层后无法正确渲染
* &amp;lbrack；安全&amp;rbrack；修复CVE-2015-20107
* &amp;lbrack；UI&amp;rbrack； 2D输出可能会变得模糊，具体取决于窗口大小
* &amp;lbrack；UI&amp;rbrack；资源预览在应用程序失去焦点时可保持打开状态
* &amp;lbrack；UI&amp;rbrack；初始屏幕圆角具有方形不透明背景

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

### 3.3.2祖基尼

*（发布日期：2022年6月28日）*

**已修复：**

* &amp;lbrack；Application&amp;rbrack；在打开项目时修复潜在崩溃
* &amp;lbrack；Export&amp;rbrack；重新启动Sampler会中断导入的自定义导出预设列表
* &amp;lbrack；互操作性&amp;rbrack；修复从Designer发送的材料被删除，然后从Designer重新发送时的崩溃
* &amp;lbrack；Project&amp;rbrack；无法删除项目中的最后一个材料或环境光（如果它是最后一个资源）
* &amp;lbrack；Project&amp;rbrack；右键单击环境光时，将显示“未保存的修改”星号

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

### 3.3.1祖基尼

*（发布日期：2022年6月7日）*

**已添加：**

* 支持&amp;lbrack；Application&amp;rbrack；本机Apple silicon (M1)
* &amp;lbrack；UI&amp;rbrack；新快捷键“C”键可在2D视图中循环切换通道
* 用于在画笔工具栏中编辑灰度颜色值的数字字段(&amp;L)&amp;R)

**已修复：**

* &amp;lbrack；工具&amp;rbrack；在UI比例缩放(150%)的Windows上使用画笔工具时偏移描边
* &amp;lbrack；Performance&amp;rbrack；提高内存消耗
* 启用该功能时可能缺少&amp;lbrack；物理尺寸&amp;rbrack；物理尺寸信息
* 按Alt键时，&amp;lbrack；UI&amp;rbrack；鼠标滚动有时无法按预期工作
* 打开保存的项目时，&amp;lbrack；Application&amp;rbrack；应用程序可能会崩溃
* &amp;lbrack；Application&amp;rbrack；在拖放多个图像并在“材质创建模板”窗口中使用“纹理导入”时崩溃
* 保存包含自定义筛选器的项目时&amp;lbrack；Application&amp;rbrack；可能发生崩溃
* &amp;lbrack；Application&amp;rbrack；切换应用程序时， Control键状态有时会丢失
* 重命名本地文件夹时资源崩溃(&amp;L)

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

### 3.3.0祖基尼

*（发布日期：2022年5月17日）*

**已添加：**

* &amp;lbrack；Content&amp;rbrack；新内容识别填充滤镜（Windows和Mac）
* &amp;lbrack；内容识别填充处理图像、PBR素材和环境光照
* &amp;lbrack；Content&amp;rbrack；将“保留拼贴”参数添加到图像到材质（AI驱动）
* &amp;lbrack；Content&amp;rbrack；“透视变换”滤镜可以在其四个点之间显示网格
* &amp;lbrack；互操作性&amp;rbrack；将材料发送到Adobe Substance 3D Stager
* &amp;lbrack；工具&amp;rbrack；调整变换或裁剪工具大小时按Ctrl键使变换居中
* 调整变换或裁剪工具大小时，按住Shift键锁定与正方形的比例(&amp;L)
* &amp;lbrack；工具&amp;rbrack；仿制图章光标可预览要盖印的内容
* &amp;lbrack；工具&amp;rbrack；使用仿制图章时预览橡皮擦光标中的原始内容
* 按住Ctrl键并单击&amp;lbrack；工具&amp;rbrack；可在仿制图章图层中创建新的图章
* &amp;lbrack；工具&amp;rbrack；连续仿制图章现在分组到单个图层中
* 画笔；工具&amp;Rbrack；画笔工具栏UI改进(&amp;L)
* &amp;lbrack；工具&amp;rbrack；画笔工具栏位置在会话期间保持不变
* 按轴新建画笔拼贴选项(&amp;L)；工具(&amp;R)
* &amp;lbrack；工具&amp;rbrack；在绘画时隐藏/显示2D视图上的叠加
* &amp;lbrack；工具&amp;rbrack；新快捷键“X”键，用于在画笔和橡皮擦之间切换
* &amp;lbrack；工具&amp;rbrack；新建快捷键“&amp;lbrack；”“&amp;rbrack；”以更改画笔大小
* &amp;lbrack；工具&amp;rbrack；新快捷键“E”键用于切换橡皮擦
* 创建环境光时新建球面投影模式(&amp;lbrack；2D 视图(&amp;r)
* 球面投影模式支持&amp;lbrack；2D视图&amp;rbrack；画笔工具
* 球面投影模式支持&amp;lbrack；2D视图&amp;rbrack；位置工具
* 球面投影模式支持&amp;lbrack；2D视图&amp;rbrack；撤消/重做
* &amp;lbrack；2D视图&amp;rbrack；在球面投影中，设置默认位置以查看环境中心
* &amp;lbrack；2D视图&amp;rbrack；新的曝光控制
* &amp;lbrack；UI&amp;rbrack；在“属性”面板中，图像微调显示内容源（图像或来自图层）
* &amp;lbrack；UI&amp;rbrack；改进了图层/素材输出下拉背景
* &amp;lbrack；UI&amp;rbrack；分辨率信息在2D视图中的新位置
* &amp;lbrack；UI&amp;rbrack；包含3D视图导航控件快捷键的新工具提示
* &amp;lbrack；UI&amp;rbrack；带有画笔控件的新工具提示
* &amp;lbrack；UI&amp;rbrack；带有投影导航控件快捷键的新工具提示
* &amp;lbrack；复合滤镜&amp;rbrack；复合滤镜处理变化以处理图像、PBR素材和环境光
* &amp;lbrack；复合滤镜&amp;rbrack；调整顺序与复合滤镜中的节点列表顺序匹配
* &amp;lbrack；复合滤镜&amp;rbrack；具有相同组的不同节点的微调将合并到“属性”面板中的一个组中
* &amp;lbrack；Application&amp;rbrack；每个资源类型都有专用的查看器设置

**已修复：**

* &amp;lbrack；应用程序在切换到2D视图时可能会崩溃
* &amp;lbrack；Application&amp;rbrack；修复多次导出时可能出现的死锁或崩溃问题
* &amp;lbrack；Application&amp;rbrack；使声道的默认值与Substance 3D Designer一致
* &amp;lbrack；应用程序加载项目不会触发材质重新计算
* &amp;lbrack；Application&amp;rbrack；更新了URL以纹理化导入文档
* &amp;lbrack；Content&amp;rbrack；使用复合滤镜时，它要求在不应更新时进行更新（重新加载时）
* 使用“不透明度混合”时，&amp;lbrack；Height映射中的细节消失(&amp;R)
* &amp;lbrack；UI&amp;rbrack；在“颜色”对话框中，使用滑块的文本字段可能会超出范围
* &amp;lbrack；UI&amp;rbrack；用法列表有一个无用的垂直滚动条

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)
* &amp;lbrack；Content&amp;rbrack；形状光Widget无法在球面投影模式下工作
* &amp;lbrack；互操作性&amp;rbrack；发送给Stager的位移的素材将失去位移控制

### 3.2.1八角德

*（发布日期：2022年3月8日）*

**已添加：**

* &amp;lbrack；导出&amp;rbrack；将dpi元数据导出到图像文件中
* &amp;lbrack；物理尺寸&amp;rbrack；在编辑物理尺寸时保持与非正方形纹理的比率
* &amp;lbrack；物理尺寸&amp;rbrack；物理尺寸元数据在物理尺寸更改时立即应用
* &amp;lbrack；UI&amp;rbrack；调整Height缩放最大滑块，以便在启用物理尺寸时影响任何类型的材料
* &amp;lbrack；UI&amp;rbrack；资源面板中有关搜索过滤器的新工具提示
* &amp;lbrack；UI&amp;rbrack；使用工具提示说明何时在“资源”面板中禁用按钮
* &amp;lbrack；Content&amp;rbrack；亮度对比度滤镜更新

**已修复：**

* “裁剪”和“变换”工具中的&amp;lbrack；2D 视图&amp;rbrack； 90度旋转按钮无法按预期工作
* &amp;lbrack；2D 视图&amp;rbrack；裁切构件有时会丢失
* &amp;lbrack；Application&amp;rbrack；清除图像参数不会重新连接基础层
* 保存项目后退出时崩溃&amp;lbrack；Application&amp;rbrack；
* 将当前材料拖放到“资源”面板集合时&amp;lbrack；Application&amp;rbrack；崩溃
* &amp;lbrack；Application&amp;rbrack；在视口中拖放资源时可能崩溃
* &amp;lbrack；Content&amp;rbrack；普通混合具有随机种子调整
* &amp;lbrack；Content&amp;rbrack；Snow滤镜的正常输出不正确，具体取决于新鲜和融化的雪参数值
* &amp;lbrack；Content&amp;rbrack；镶板滤镜：修复了意外的接缝
* &amp;lbrack；Content&amp;rbrack；刺绣滤镜：删除金属映射中的线程
* &amp;lbrack；Content&amp;rbrack；Floor拼贴过滤器：修复x和y拼贴计数
* &amp;lbrack；Content&amp;rbrack；砖块壁滤镜：将法线和Height输出到16位
* &amp;lbrack；Export&amp;rbrack；导出弹出窗口中的默认文件名不是当前材料名
* &amp;lbrack；导出&amp;rbrack；使用导出预设的物理比率导出时，会提供错误的尺寸
* CLO导出预设中缺少&amp;lbrack；Export&amp;rbrack；金属
* &amp;lbrack；Export&amp;rbrack；替换导出自定义预设时，显示名称不会更新
* &amp;lbrack；图层&amp;rbrack；未发现第一个插入图层的自定义通道
* 更改隐藏图层的微调时，重新评估&amp;lbrack；图层&amp;rbrack；素材
* &amp;lbrack；Localization&amp;rbrack；工具提示在“导出”面板中未本地化
* &amp;lbrack；物理尺寸&amp;rbrack；禁用资源物理尺寸不会移除物理规模
* &amp;lbrack；物理尺寸&amp;rbrack；Height缩放值不能首次设置为滑块边界之外
* &amp;lbrack；物理尺寸&amp;rbrack；导入没有物理尺寸的图像会阻止打开项目
* &amp;lbrack；物理尺寸&amp;rbrack；物理尺寸在缺失时错误地设置为零
* &amp;lbrack；物理尺寸&amp;rbrack；物理尺寸物理缩放复选框状态在首次显示时不更新
* &amp;lbrack；UI&amp;rbrack；基础材质和“正常到Height”没有类别
* 绘制图像时，&amp;lbrack；UI&amp;rbrack；光标有时不可见
* &amp;lbrack；UI&amp;rbrack；禁用文本字段编辑菜单中的“全部复制”和“全部剪切”选项（如果文本字段为空）
* &amp;lbrack；UI&amp;rbrack；筛选器名称包含错误的字符
* &amp;lbrack；UI&amp;rbrack；物理尺寸锁定按钮的样式不正确
* &amp;lbrack；UI&amp;rbrack；“资源”面板搜索栏中的“关闭”按钮不清除搜索字符串

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)

### 3.2.0八角德

*（发布日期：2022年1月25日）*

**已添加：**

* &amp;lbrack；物理尺寸&amp;rbrack；新建物理尺寸面板
* &amp;lbrack；物理尺寸&amp;rbrack；将物理尺寸选项添加到“材料创建模板”窗口
* &amp;lbrack；物理尺寸&amp;rbrack；添加物理尺寸测量工具
* &amp;lbrack；物理尺寸&amp;rbrack；添加物理尺寸自动测量工具
* &amp;lbrack；物理尺寸&amp;rbrack；添加物理尺寸诊断工具
* &amp;lbrack；物理尺寸&amp;rbrack；允许设置物理尺寸的z值
* 用于设置2D 视图缩放级别的下拉构件(&amp;lbrack；物理尺寸&amp;rbrack；)
* &amp;lbrack；物理尺寸&amp;rbrack；在缩放级别下拉列表中新增了“以物理比例显示”选项
* &amp;lbrack；物理尺寸&amp;rbrack；缩放级别下拉列表中新增了“适合物理尺寸”选项
* &amp;lbrack；物理尺寸&amp;rbrack；在2D 视图中显示物理尺寸
* &amp;lbrack；物理尺寸&amp;rbrack；以3D视口显示物理尺寸
* &amp;lbrack；物理尺寸&amp;rbrack；在图像导入对话框中，如果存在导入的物理尺寸，则显示高度图深度
* &amp;lbrack；物理尺寸&amp;rbrack；在资源上下文菜单中显示物理尺寸
* &amp;lbrack；物理尺寸&amp;rbrack；在首选项中设置长度单位
* &amp;lbrack；物理尺寸&amp;rbrack；导出纹理并保留物理比率
* &amp;lbrack；元数据&amp;rbrack；可将自定义元数据添加到用户创作的资源中
* &amp;lbrack；导出&amp;rbrack；将自定义元数据导出到.sbs(ar)文件
* &amp;lbrack；Export&amp;rbrack；将描述、类别、作者和标记元数据导出到.sbs(ar)文件
* &amp;lbrack；导出&amp;rbrack；将物理尺寸导出为.sbs(ar)文件
* &amp;lbrack；导出&amp;rbrack；设置。sbsar 文件压缩设置
* &amp;lbrack；导出&amp;rbrack；将资源缩览图导出为.sbs(ar)文件
* &amp;lbrack；导出&amp;rbrack；在导出.sbs(ar)文件时设置图形类型
* &amp;lbrack；Application&amp;rbrack；实时引擎2021不再可用
* &amp;lbrack；Application&amp;rbrack；还原/重做现在支持拼贴(U，V)和Height缩放滑块更改
* &amp;lbrack；渲染&amp;rbrack；保存创作资源时生成磁盘缓存
* &amp;lbrack；资源&amp;rbrack；按住Ctrl键并单击可在“资源”面板中启用多个资源类型过滤器
* &amp;lbrack；UI&amp;rbrack；锁定拼贴(U，V)滑块的功能
* &amp;lbrack；UI&amp;rbrack；在文本字段中添加具有“复制”、“剪切”、“粘贴”、“全部复制”和“剪切全部”的上下文菜单
* &amp;lbrack；UI&amp;rbrack；长度单位（米、英寸、秒差距……） 标签和文本字段中的支持
* &amp;lbrack；UI&amp;rbrack；用户可以设置用于显示数字的小数精度
* &amp;lbrack；UI&amp;rbrack；在所有相关的测量弹出窗口中使用单位(&amp;R)
* &amp;lbrack；本地化&amp;rbrack；默认新资源名称现已本地化
* &amp;brack；Content&amp;rbrack；新布料编织生成器
* &amp;lbrack；Content&amp;rbrack；新通道开关过滤器
* &amp;lbrack；Content&amp;rbrack；所有相关的滤镜现在都可以识别物理尺寸
* 用于“木工光洁度”的&amp;lbrack；Content&amp;rbrack；新图标
* &amp;lbrack；Content&amp;rbrack；所有滤镜现在都与Adobe Standard Material(ASM)通道兼容
* &amp;lbrack；Content&amp;rbrack；滤镜现在可以有“环境”变化

**已修复：**

* &amp;lbrack；2D视图&amp;rbrack；通道在移除后保留在列表中
* &amp;lbrack；Application&amp;rbrack；无法复制从操作系统文件资源管理器加载的资源
* &amp;lbrack；Application&amp;rbrack；退出时崩溃
* 在“资源”面板中单击“入门资源”时，有时会崩溃&amp;lbrack；Application&amp;rbrack；
* 删除材料时崩溃Application&amp;rbrack；(&amp;L)
* &amp;lbrack；Application&amp;rbrack；环境变量“SUBSTANCE_DISABLE_SPECIFIC_FEATURES”在设置为“0”或“”时仍处于活动状态。
* &amp;lbrack；应用程序&amp;rbrack；在保存包含多个材料的项目时冻结
* &amp;lbrack；Application&amp;rbrack；导入图像可能会导致崩溃
* &amp;lbrack；应用程序&amp;rbrack；在首次启动时缺少某些入门级资源
* &amp;lbrack；Export&amp;rbrack；导出资源有时会导致崩溃
* &amp;lbrack；Layers&amp;rbrack；当“图层”面板关闭或不可见时无法导入图像
* &amp;lbrack；Layers&amp;rbrack；更改语言会导致重新计算当前资源
* &amp;lbrack；图层&amp;rbrack；更改导入图像的用法不会更新要使用的滤镜变化
* 调整图层下面的图层时，&amp;lbrack；图层&amp;rbrack；图像到材料(AI)有时会不进行计算
* &amp;lbrack；Layers&amp;rbrack；图像到材料(AI)有时会在不需要时重新计算
* &amp;lbrack；Layers&amp;rbrack；在磁盘上更新自定义筛选器时，建议不要更新
* Layers&amp;rbrack；正常通道有时具有错误的像素格式(&amp;L)
* &amp;lbrack；Layers&amp;rbrack；某些图层即使不可见也仍会计算
* &amp;lbrack；Layers&amp;rbrack；切换图层可见性时，2D 视图工具可能会损坏
* &amp;lbrack；Layers&amp;rbrack；使用“图像到材料”(AI)时，UI冻结
* &amp;lbrack；Layers&amp;rbrack；切换变换滤镜图层的可见性会破坏2D 视图工具，并且可能导致崩溃
* 从图层堆叠中删除图层时&amp;lbrack；Layers&amp;rbrack；重新计算过多
* &amp;lbrack；Layers&amp;rbrack；当复合滤镜包含异常或自定义输入/输出时，Sampler不对其进行计算
* &amp;lbrack；Performance&amp;rbrack；资源面板打开缓慢
* &amp;lbrack；Performance&amp;rbrack；避免对图层堆叠进行一些不必要的重新计算
* &amp;lbrack；Performance&amp;rbrack；加载项目资源花费的时间过多
* 不能使用磁盘上的渲染缓存(&amp;L)
* &amp;lbrack；Performance&amp;rbrack；在图层之间切换缓慢
* &amp;lbrack；性能调整材料或滤镜速度缓慢
* &amp;lbrack；Project&amp;rbrack；退出时保存项目可能会导致崩溃
* &amp;lbrack；渲染&amp;rbrack；删除图像可能会删除所有输出
* &amp;lbrack；Rendering&amp;rbrack；调整时，视口中显示的渲染时间错误
* &amp;lbrack；UI&amp;rbrack；在需要时在导出弹出窗口中无法垂直滚动
* &amp;lbrack；UI&amp;rbrack；可以在没有要导出的内容时打开导出弹出窗口
* &amp;lbrack；UI&amp;rbrack；某些弹出窗口在内容溢出时不会滚动
* 单击文本字段或打开菜单时，未选择&amp;lbrack；UI&amp;rbrack；文本字段
* &amp;lbrack；UI&amp;rbrack；属性面板中混合模式的名称有时不正确
* &amp;lbrack；UI&amp;rbrack； “文件”菜单中的“存储”选项有时显示为灰色
* &amp;lbrack；UI&amp;rbrack；重命名两个材料后，文本字段不会消失
* 首选项弹出窗口中的&amp;lbrack；UI&amp;rbrack；拼写错误

**已知问题：**

* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)

### 3.1.2索科特尔

*（发布日期：2021年12月14日）*

**已修复：**

* &amp;lbrack；互操作性&amp;rbrack；在Windows上使用Bridge中的Substance 3D Sampler打开.sbsar文件可能会失败
* &amp;lbrack；Layers&amp;rbrack；将唯一图层移动到它下面时崩溃
* 更改语言时，&amp;lbrack；UI&amp;rbrack；通道设置按钮消失
* &amp;lbrack；UI&amp;rbrack；保存项目后，“属性”面板中的材质名称消失
* 单击“所有库”会导致崩溃(&amp;L)

**已知问题：**

* &amp;lbrack；实时引擎2021&amp;rbrack；计算繁重可能会使应用程序崩溃
* &amp;lbrack；实时引擎2021&amp;rbrack；实时引擎2021将在装有AMD CPU和Nvidia GPU的Windows计算机上崩溃
* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)

### 3.1.1索科特尔

*（发布日期：2021年11月24日）*

**已添加：**

* &amp;lbrack；互操作性&amp;rbrack；将资源（SBS或SBSAR）发送到Substance 3D Designer
* &amp;lbrack；互操作性&amp;rbrack；在首选项中设置与Substance 3D Designer互操作性的默认格式
* &amp;lbrack；互操作性&amp;rbrack；从Adobe Bridge接收多个资源
* &amp;lbrack；UI&amp;rbrack；新建随机种子Widget
* &amp;lbrack；UI&amp;rbrack；上下文菜单更新
* 资源将图像从资源面板拖放到属性面板(&amp;L)
* &amp;lbrack；Project&amp;rbrack；资源名称经过整理以避免出现某些特定字符
* SBSAR文件的&amp;lbrack；品牌化&amp;rbrack；更新文件图标
* &amp;lbrack；Engine&amp;rbrack；更新Substance 引擎版本8.3.0

**已修复：**

* &amp;lbrack；Content&amp;rbrack；裁剪 — 裁剪非方形图像时保留比例
* &amp;lbrack；Content&amp;rbrack；变换 — 使用构件时不会反转水平变换
* 碎石；内容&amp;rbrack；砾石 — 修复所有通道上的自定义蒙版绘画
* &amp;lbrack；Content&amp;rbrack；地板拼贴 — 修复图案拼贴和重复的问题
* 如果未安装，&amp;lbrack；资源&amp;rbrack；灰显Adobe Bridge选项
* &amp;lbrack；拾色器&amp;rbrack；转义键可关闭拾色器
* 使用灰度输入时，渲染&amp;brack；固定散射距离缩放(&amp;L)
* &amp;lbrack；Share&amp;rbrack；发送至选项仅适用于Adobe许可证
* &amp;lbrack；Project&amp;rbrack；修复内存性能问题

**已知问题：**

* &amp;lbrack；实时引擎2021&amp;rbrack；计算繁重可能会使应用程序崩溃
* &amp;lbrack；实时引擎2021&amp;rbrack；实时引擎2021将在装有AMD CPU和Nvidia GPU的Windows计算机上崩溃
* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)

### 3.1.0索科特尔

*（发布日期：2021年9月28日）*

**已添加：**

* 颜色选择器&amp;R；新建颜色选择器UI(&amp;L)
* 颜色选择器&amp;brack；并排预览当前和以前的颜色
* &amp;lbrack；拾色器&amp;rbrack；以十六进制输入颜色
* 颜色选择器&amp;brack；带颜色预览的新吸管(&amp;L)
* &amp;lbrack；拾色器&amp;rbrack；吸管可以在Sampler之外选取颜色
* 颜色选择器&amp;Rbrack；在RGB或HSV色彩空间中微调颜色(&amp;L)
* 颜色选择器&amp;brack；存储和管理色板(&amp;L)
* &amp;lbrack；互操作性&amp;rbrack；通过图像导入图层或图像参数在Illustrator中编辑图像
* &amp;lbrack；互操作性&amp;rbrack；通过图像导入图层或图像参数在Photoshop中编辑图像
* 标记；构件&amp;标记；新建裁切构件(&amp;R)
* &amp;lbrack；Widget&amp;rbrack；按Enter验证裁切
* &amp;lbrack；Widget&amp;rbrack；裁切构件会读取图像大小以适合构件，并在调整大小时保持比例
* &amp;lbrack；UI&amp;rbrack；新进度滑块UI
* &amp;lbrack；Application&amp;rbrack；在首选项中添加常规格式选择
* &amp;lbrack；Application&amp;rbrack；图像导入图层中的普通格式遵循在首选项中设置的默认普通格式
* &amp;lbrack；Application&amp;rbrack；在2D 视图中，正常格式显示在首选项中设置的正常格式之后
* &amp;lbrack；Application&amp;rbrack；以首选项中设置的常规格式导出常规格式
* &amp;lbrack；Export&amp;rbrack；将普通格式参数添加到SBS和Sbsar 文件导出
* &amp;lbrack；导出&amp;rbrack；将着色器设置添加到SBS和Sbsar 文件导出
* &amp;lbrack；Export&amp;rbrack；设置导出的图形的默认分辨率
* &amp;lbrack；复合滤镜&amp;rbrack；打包SSA滤镜(7z)
* &amp;lbrack；复合滤镜&amp;rbrack；在复合滤镜中添加类别元数据
* 复合滤镜&amp;brack；复合滤镜&amp;brack；复合滤镜可以有嵌入的缩略图
* &amp;lbrack；复合滤镜&amp;rbrack；将复合滤镜扩展名(.ssafilter)添加到“获取内容”的文件对话框中
* 资源面板中的导入复合滤镜(.ssafilter)（&amp;lbrack；复合滤镜&amp;rbrack；）
* &amp;lbrack；引擎&amp;rbrack；将substance引擎更新到v8.2.0

**已修复：**

* &amp;lbrack；Application&amp;rbrack；连接的本地文件夹可能会挂起
* 退出时崩溃&amp;lbrack；应用程序&amp;rbrack；
* 启动两个Sampler实例时的Application&amp;rbrack；崩溃(&amp;L)
* &amp;lbrack；Content&amp;rbrack；裁剪滤镜具有随机种子调整
* &amp;lbrack；Content&amp;rbrack；某些Substance素材有时无法升级
* &amp;lbrack；Export&amp;rbrack；使用新添加的自定义预设导出时崩溃
* &amp;lbrack；Export&amp;rbrack；导出弹出窗口中缺少包的估计大小
* &amp;lbrack；导出&amp;rbrack；修复导出SBS和SBSAR文件时出现的内存泄漏问题
* 复合滤镜&amp;brack；复合滤镜&amp;brack；复合滤镜可能有重复输入
* 如果滤镜具有不符合的引用，&amp;lbrack；复合滤镜&amp;rbrack；崩溃
* &amp;lbrack；使用复合滤镜重新排序图层堆叠时的复合滤镜&amp;rbrack；崩溃
* &amp;lbrack；复合滤镜&amp;rbrack；渲染有时会挂起
* &amp;lbrack；图像导入&amp;rbrack；导入图像会触发多个渲染
* 撤消/重做时崩溃图层(&amp;L)
* 添加基础材质时崩溃Layers&amp;rbrack；
* 将无效图像用作崩溃时环境光(&amp;L)
* &amp;lbrack；Layers&amp;rbrack；修复插入带有多个图形的过滤器时重复导入的问题
* &amp;lbrack；Layers&amp;rbrack；重新排序图层并非始终有效
* 加载不完整的项目文件时出现&amp;lbrack；项目&amp;rbrack；崩溃
* 打开损坏的项目时崩溃&amp;lbrack；项目&amp;rbrack；
* &amp;lbrack；Project&amp;rbrack；一些资源可能会从项目中消失
* &amp;lbrack；属性&amp;rbrack；修复缺失滤镜的预设
* 无法设置&amp;lbrack；UI&amp;rbrack；角度参数
* &amp;lbrack；UI&amp;rbrack；筛选器元数据显示在“资源”面板中
* &amp;lbrack；UI&amp;rbrack；按类别分组隐藏筛选器
* 资源面板中的滚动问题(&amp;L)
* &amp;lbrack；UI&amp;rbrack；导出面板现在有一个滚动条
* &amp;lbrack；UI&amp;rbrack；在图像选择器中不显示某些图像格式的缩览图

**已知问题：**

* &amp;lbrack；实时引擎2021&amp;rbrack；重型计算可以崩溃应用程序
* &amp;lbrack；实时引擎2021&amp;rbrack；实时引擎2021将在安装了AMD CPU和Nvidia GPU的Windows计算机上崩溃
* 拾色器可能无法在具有不同分辨率的第二台显示器上选取颜色(&amp;L)

### 3.0.1华夫饼

*（发布日期：2021年7月27日）*

**已添加：**

* &amp;lbrack；画笔&amp;rbrack；在画笔工具中启用颜色（如果图像输入支持）
* 按住Shift键在画笔工具中绘制直线(&amp;L)
* 在画笔工具中按住Shift键时显示线条预览(&amp;L)
* 画笔工具现在支持撤消和重做(&amp;L)
* &amp;lbrack；2D 视图&amp;rbrack；绘画时使用图像输入默认颜色
* &amp;lbrack；图层&amp;rbrack；读取SBSAR文件中的Substance输入默认值
* &amp;lbrack；渲染&amp;rbrack；允许将Height与普通图像组合
* 支持&amp;lbrack；渲染&amp;rbrack；子表面散射（在MacOS上不可用）
* &amp;lbrack；Assets&amp;rbrack；使用SBSAR图形类型确定资源类型
* 资源面板&amp;lbrack；资源为搜索和资源可发现性提供更好的性能
* &amp;lbrack；Assets&amp;rbrack；在“资源”面板中添加了一个“所有库”条目，其中显示了所有库的所有资源
* &amp;lbrack；Assets&amp;rbrack；用户现在可以选择按类别或类型对资源进行分组
* &amp;lbrack；导入&amp;rbrack；导入时自动检测各向异性、毛皮、光泽和Specular edge color纹理
* &amp;lbrack；UI&amp;rbrack；用图标替换面板标题
* &amp;lbrack；UI&amp;rbrack；文本字段样式更新
* &amp;lbrack；UI&amp;rbrack；在“创建环境光模板”窗口中新建说明文本
* &amp;lbrack；Application&amp;rbrack；在发送到外部应用程序时，以当前分辨率导出资源
* &amp;lbrack；应用程序&amp;rbrack；材料默认分辨率现在为2048\*2048（在macos上为1024\*1024）
* floor拼贴滤镜中的新图案(&amp;L)
* 颜色替换滤镜中的&amp;lbrack；Content&amp;rbrack；新双色模式

**已修复：**

* 画笔工具中的第一个笔触有时损坏(&amp;l)；2D 视图(&amp;r)
* 画笔工具不可见时&amp;lbrack；2D 视图&amp;rbrack；释放资源
* &amp;lbrack；2D 视图&amp;rbrack；在变换构件中使用右侧的调整大小光标
* 如果用户之前已在2D 视图中平移，&amp;lbrack；2D 视图&amp;rbrack；构件不会显示
* &amp;lbrack；打开具有损坏工作流程的项目时崩溃Application&amp;rbrack；
* &amp;lbrack；Application&amp;rbrack；修复应用程序关闭问题，防止日志被无用的错误淹没
* &amp;lbrack；Application&amp;rbrack；重做、删除和保存键盘快捷键在某些操作系统上不起作用
* &amp;lbrack；Application&amp;rbrack；撤消/重做更改导入图层中的图像使用情况已损坏
* Lbrack；Export&amp;rbrack；Emission color导出的图像的名称错误(&amp;L)
* 使用SBSAR导出时，&amp;lbrack；Export&amp;rbrack；环境为8位
* &amp;lbrack；Export&amp;rbrack；删除导出的图像文件名中的额外空格
* &amp;lbrack；导出&amp;rbrack；替换或删除自定义导出预设崩溃
* &amp;lbrack；图层&amp;rbrack；避免在输入计数不匹配时进行崩溃
* 插入基础材质图层时崩溃&amp;lbrack；图层&amp;rbrack；
* &amp;lbrack；图层&amp;rbrack；筛选器输入计数上限为默认值
* &amp;lbrack；图层&amp;rbrack；重做操作会将混合类型错误地更改为Height混合
* &amp;lbrack；图层&amp;rbrack；删除输入标头上方的放置区域
* 在输入标头周围错误的位置插入图层(&amp;L)
* &amp;lbrack；Layers&amp;rbrack； Reset all settings按钮不会重置下拉构件值
* &amp;lbrack；图层&amp;rbrack；在图像导入图层上更改图像时撤消/重做将项目标记为已修改并保存
* 混合图层可以停止使用(&amp;L)&amp;R；
* 加载缺少依赖项的旧项目文件夹时崩溃(&amp;L)
* 保存后使用还原/重做时&amp;lbrack；项目&amp;rbrack；崩溃
* &amp;lbrack；Project&amp;rbrack；打开包含环境光的Sbsar 文件时会创建材料资源
* &amp;lbrack；项目&amp;rbrack；重命名素材可触发缩略图生成
* &amp;lbrack；重命名材质后保存&amp;rbrack；将项目标记为未修改
* &amp;lbrack；Project&amp;rbrack；重命名材质后未保存某些更改
* &amp;lbrack；渲染&amp;rbrack；亮点在具有2020实时引擎的环境中可见
* &amp;lbrack；渲染使用2021实时引擎调整大小时崩溃
* &amp;lbrack；渲染&amp;rbrack；在Height级别更改时重新计算阴影
* &amp;lbrack；Assets&amp;rbrack；连接的文件夹在添加无效文件时停止为新资源编制索引
* 将本地文件夹与多种材质连接时&amp;lbrack；资源崩溃(&amp;R)
* &amp;lbrack；UI&amp;rbrack； 2D/3D视图按钮缺少工具提示
* &amp;lbrack；UI&amp;rbrack；启动时，“资源”面板中的所有资源都会高亮显示
* 导入材质时，&amp;lbrack；UI&amp;rbrack；痕迹有时会在“资源”面板中消失
* &amp;lbrack；UI&amp;rbrack；更改语言不影响“项目”面板
* &amp;lbrack；UI&amp;rbrack；通道设置面板显示旧版工作流程信息
* &amp;lbrack；UI&amp;rbrack；在“属性”面板中未做微调的滤镜中正确对齐“此项目没有设置”文本
* &amp;lbrack；UI&amp;rbrack；元素在欢迎屏幕和首选项弹出窗口中未对齐
* &amp;lbrack；UI&amp;rbrack；面板标题的宽度不正确
* &amp;lbrack；UI&amp;rbrack；滚动有时在“属性”面板中损坏
* &amp;lbrack；UI&amp;rbrack；启动画面比例不正确且模糊
* &amp;lbrack；UI&amp;rbrack；全屏模式不是全屏模式
* &amp;lbrack；UI&amp;rbrack；取消停靠的面板始终位于顶部，即使该应用程序在MacOS上未处于活动状态
* &amp;lbrack；UI&amp;rbrack；更新欢迎屏幕横幅图像
* &amp;lbrack；Content&amp;rbrack；拼贴滤镜不处理环境遮蔽声道
* 焊缝组件接缝选择和菱形图案导致&amp;lbrack；内容&amp;rbrack；面组缝合问题
* &amp;lbrack；Content&amp;rbrack；浮雕滤镜以256 x 256像素工作
* &amp;lbrack；Content&amp;rbrack；修复当偏移大于0时地板拼贴的拼贴问题

**已知问题：**

* &amp;lbrack；实时引擎2021&amp;rbrack；计算繁重，应用程序崩溃
* &amp;lbrack；实时引擎2021&amp;rbrack；实时引擎2021将在同时具有AMD CPU和Nvidia GPU的Windows计算机上崩溃

### 3.0.0华夫饼

*（发布日期：2021年6月23日）*

**已添加：**

* &amp;lbrack；品牌&amp;rbrack；Substance Alchemist将变为Adobe Substance 3D Sampler
* brack；品牌推广&amp;rbrack；新建应用程序图标(&amp;L)
* &amp;lbrack；UI&amp;rbrack；新用户体验和用户界面
* &amp;lbrack；UI&amp;rbrack；新闪屏(&amp;R)
* &amp;lbrack；UI&amp;rbrack；面板在界面中不可停靠和停靠
* &amp;lbrack；UI&amp;rbrack；最多可在同一列中停放3个面板
* &amp;lbrack；UI&amp;rbrack；可在同一面板中最多停放3个面板（选项卡）
* &amp;lbrack；UI&amp;rbrack；取消停靠面板可在同一屏幕或不同屏幕中创建单独的窗口
* 单击已关闭面板的图标时，&amp;lbrack；UI&amp;rbrack；已关闭面板弹出窗口
* &amp;lbrack；UI&amp;rbrack；通过移动面板图标重新排列左右栏
* &amp;lbrack；UI&amp;rbrack；用于直接访问特定滤镜（裁切、变换、透视变换、仿制图章）的新工具栏
* &amp;lbrack；UI&amp;rbrack；左侧栏中新增“获取内容”按钮
* &amp;lbrack；UI&amp;rbrack；使用“获取内容”按钮直接将文件导入到您的资源中
* &amp;lbrack；UI&amp;rbrack；使用“获取内容”按钮将文件直接导入到您的图层
* &amp;lbrack；UI&amp;rbrack；使用“获取内容”按钮直接Substance 3D Assets网站
* 现在可直接在视口中访问&amp;lbrack；UI&amp;rbrack；分辨率构件
* &amp;lbrack；UI&amp;rbrack；现在所有UI元素都是动态加载的
* &amp;lbrack；UI&amp;rbrack；快捷键 — 使用“2”可切换2D 视图的可见性
* &amp;lbrack；UI&amp;rbrack；快捷键 — 使用“3”可切换3D视图的可见性
* &amp;lbrack；欢迎屏幕&amp;rbrack；使用“新建”按钮单击即可创建项目
* &amp;lbrack；欢迎屏幕&amp;rbrack；新图稿横幅
* &amp;lbrack；Project&amp;rbrack；所有项目现在都与一个唯一的文件相关联
* &amp;lbrack；项目&amp;rbrack；新建项目文件扩展名.ssa
* &amp;lbrack；项目&amp;rbrack；另存为项目将要求您选择保存项目的位置
* &amp;lbrack；Project&amp;rbrack；关闭Sampler将要求您保存项目（如果未保存）
* &amp;lbrack；Project&amp;rbrack；关闭Sampler后，如果自上次保存后进行了修改，则将要求您保存项目
* &amp;lbrack；Project&amp;rbrack；项目名称显示在视口上方
* &amp;lbrack；Project&amp;rbrack；如果项目名称未保存或包含自上次保存以来所做的修改，则项目名称将采用带星号的斜体
* &amp;lbrack；Project&amp;rbrack；直接从操作系统资源管理器打开.ssa项目文件
* &amp;lbrack；Project&amp;rbrack；从操作系统资源管理器中打开.sbsar将启动Sampler，同时显示一个可以使用此.sbsar文件的新项目
* &amp;lbrack；Project&amp;rbrack；从操作系统资源管理器中打开.alch（旧版Substance Alchemist文件）
* &amp;lbrack；项目面板&amp;rbrack；包含项目中创建的所有资源的新面板
* &amp;lbrack；项目面板&amp;rbrack；使用+图标创建资源（材质或环境光照）
* &amp;lbrack；项目面板&amp;rbrack；右键单击资源可打开上下文菜单
* &amp;lbrack；项目面板&amp;rbrack；从右键单击上下文菜单中，可以删除资源
* &amp;lbrack；项目面板&amp;rbrack；在右键单击上下文菜单中，您可以复制资源
* &amp;lbrack；项目面板&amp;rbrack；在右键单击上下文菜单中，可以重命名资源
* &amp;lbrack；项目面板&amp;rbrack；在资源之间切换不会丢失修改
* &amp;lbrack；Resolution&amp;rbrack；您现在可以为所有资源设置非方形分辨率
* &amp;lbrack；Resolution&amp;rbrack；分辨率值由项目中的资源保存
* 环境光在Substance 3D Sampler中创建环境光(&amp;L)
* 环境光创建环境光时，拖放图像将显示“环境光创建模板”窗口(&amp;L)
* &amp;lbrack；环境光&amp;rbrack；在环境光创建模板中，选择环境导入以将图像在3D视图中分配给环境
* &amp;lbrack；环境光&amp;rbrack；在环境光创建模板中，选择HDR合并，以便从多个具有不同曝光度的360度图像中创建环境光
* &amp;lbrack；环境光&amp;rbrack；在环境光创建模板中，选择“用作位图”以在创建环境光之前编辑图像
* &amp;lbrack；环境光照&amp;rbrack；在图像导入图层中指定环境使用情况，以便在3D视图中直接将图像分配给环境
* &amp;lbrack；环境光&amp;rbrack；在环境通道的2D视图中，有一个自动颜色校正使渲染显示与3D视图中的显示相同
* 环境光照&amp;brack；用于创建环境光的新专用内容(&amp;L)
* 资源面板(&amp;L)&amp;R；资源面板和筛选器面板合并到新的资源面板中
* &amp;lbrack；资源面板&amp;rbrack；资源面板现在支持以下资源类型：材料、筛选器和图像
* &amp;lbrack；资源面板&amp;rbrack；所有入门资源都可在“入门资源”部分中访问
* 资源面板&amp;rbrack；入门资源部分为只读(&amp;l)
* 资源面板(&amp;L)&amp;R；新增的“您的资源”部分
* &amp;lbrack；资源面板&amp;rbrack；“您的资源”部分是您可以导入所有资源的位置
* &amp;lbrack；资源面板&amp;rbrack； “您的资源”中的所有资源都添加到文档中的特定文件夹中
* &amp;lbrack；资源面板&amp;rbrack；连接资源面板中的本地文件夹以添加新部分
* &amp;lbrack；资源面板&amp;rbrack；搜索将在当前文件夹及其子文件夹中搜索
* &amp;lbrack；资源面板&amp;rbrack；在具有痕迹的文件夹和子文件夹之间导航
* 资源面板&amp;lbrack；按材料、按筛选器或按图像筛选当前文件夹
* &amp;lbrack；资源面板&amp;rbrack；组合多个滤镜以仅获取材料和图像
* &amp;lbrack；资源面板&amp;rbrack；通过在网格或列表之间切换来更改显示
* 资源面板&amp;brack；滤镜用它们的图标表示(&amp;L)
* 资源面板&amp;brack；图像用预览表示(&amp;L)
* &amp;lbrack；资源面板&amp;rbrack；增加宽度将更改特定视图的面板布局，以便在文件夹之间导航
* &amp;lbrack；资源面板&amp;rbrack；在非只读部分中，通过将资源拖放到素材箱图标来删除资源
* 资源面板&amp;brack；右键单击资源可打开上下文菜单(&amp;l)
* &amp;lbrack；资源面板&amp;rbrack；从右键单击上下文菜单中访问资源元数据（名称、类别、位置）
* &amp;lbrack；资源面板&amp;rbrack；从右键单击上下文菜单中，删除资源（仅适用于非只读部分）
* &amp;lbrack；资源面板&amp;rbrack；从右键单击上下文菜单中，浏览Adobe Bridge中的资源
* &amp;lbrack；图层面板&amp;rbrack；新建图标用于在图层上直接添加基础材质
* &amp;lbrack；图层面板&amp;rbrack；快捷键- Shift + B组合键将在图层上添加基础材质
* 图层面板&amp;lbrack；图层现在具有缩略图预览（材料缩略图、滤镜图标或图像预览）
* &amp;lbrack；属性面板&amp;rbrack；带有资源名称和资源缩略图的“属性”面板标题的新设计
* &amp;lbrack；属性面板&amp;rbrack；滤镜图层现在支持预设
* &amp;lbrack；属性面板&amp;rbrack；在图像导入图层上，右键单击图像预览以在Photoshop中编辑图像
* &amp;lbrack；Adobe Bridge&amp;rbrack；在Adobe Bridge中浏览您的资源时，将在资源位置启动Bridge
* &amp;lbrack；Adobe Photoshop&amp;rbrack；在Adobe Photoshop中编辑将在Photoshop中打开准备编辑的图像
* &amp;lbrack；Adobe Photoshop&amp;rbrack；在Adobe Photoshop中每次保存时，编辑的图像都会在Sampler中重新加载
* 从Adobe Substance 3D Designer发送的&amp;lbrack；Substance 3D Designer&amp;rbrack；资源将直接到达资源面板的“您的资源”部分
* &amp;lbrack；Export&amp;rbrack；将资源直接发送到Adobe Substance 3D Painter和Adobe Substance 3D Stager
* &amp;lbrack；导出&amp;rbrack；将材料和环境光发送到Adobe Substance 3D Painter
* &amp;lbrack；导出&amp;rbrack；将环境光发送到Adobe Substance 3D Stager
* &amp;lbrack；现在支持新的材料属性，并以3D形式渲染&amp;rbrack；
* &amp;lbrack；渲染&amp;rbrack；添加光泽支持（光泽颜色、光泽不透明度和光泽粗糙度）
* &amp;lbrack；渲染&amp;rbrack；添加涂层支持（Coat color、Coat roughness、Coat normal、Coat specular level和涂层IOR）
* &amp;lbrack；渲染&amp;rbrack；添加各向异性支持（Anisotropy level和Anisotropy angle）
* &amp;lbrack；渲染&amp;rbrack；添加Specular edge color支持
* &amp;lbrack；渲染&amp;rbrack；在“通道设置”面板中激活这些新属性
* &amp;lbrack；渲染&amp;rbrack；引入新的实时引擎(2021)渲染器（测试版）
* &amp;lbrack；渲染&amp;rbrack；在“查看器设置”面板中的两个渲染器版本之间切换
* &amp;lbrack；Rendering&amp;rbrack；实时引擎(2021)渲染器支持translucency、吸收和散布材料属性
* &amp;lbrack；Rendering&amp;rbrack；实时引擎(2021)渲染器引入了一种从环境光计算阴影的新方法
* &amp;lbrack；Rendering&amp;rbrack；实时引擎(2021)渲染器实时计算环境光的辐照度
* &amp;lbrack；着色器设置面板&amp;rbrack；新着色器设置面板可调整特定材料着色器参数
* &amp;lbrack；着色器设置面板&amp;rbrack；新参数（正常比例、Height比例、Height级别、发射强度、IOR、Coat normal强度和涂层IOR）
* &amp;lbrack；着色器设置面板&amp;rbrack；实时引擎2021的特定参数（次表面散射、散射距离、红移和瑞利散射）
* &amp;lbrack；着色器设置面板&amp;rbrack；设置值按资源存储
* &amp;lbrack；查看器设置面板&amp;rbrack；添加了默认环境光的预览
* &amp;lbrack；查看器设置面板&amp;rbrack；添加了默认网格的预览
* &amp;lbrack；查看器设置面板&amp;rbrack；新环境不透明度参数
* &amp;lbrack；查看器设置面板&amp;rbrack；新环境模糊参数（特定于实时引擎2021渲染器）
* &amp;lbrack；本地化&amp;rbrack；德语和法语的新翻译
* &amp;lbrack；Content&amp;rbrack；新的默认入门材料
* brack；Content&amp;rbrack；新的默认环境光照(&amp;L)
* &amp;lbrack；Content&amp;rbrack；所有过滤器均已更新、清除和优化
* &amp;lbrack；Content&amp;rbrack；调整滤镜已拆分为多个滤镜
* &amp;lbrack；Content&amp;rbrack；新建亮度/对比度滤镜
* 标记；内容标记；新建色相/饱和度滤镜(&amp;R)
* 标记；内容标记；新建自然饱和度滤镜(&amp;R)
* 标记；内容标记；新建锐化滤镜(&amp;R)
* &amp;lbrack；Content&amp;rbrack；新常规/Height调整
* &amp;lbrack；Content&amp;rbrack；新建面板过滤器
* 标记；内容标记；新建涂抹滤镜(&amp;R)
* &amp;lbrack；Content&amp;rbrack；新建编织过滤器
* &amp;lbrack；Content&amp;rbrack；新变形变换滤镜
* &amp;lbrack；Content&amp;rbrack；AO过滤器的新Height
* &amp;lbrack；Content&amp;rbrack；正常过滤器的新Height
* &amp;lbrack；Content&amp;rbrack；颜色替换 — 在新的受支持通道（光泽、涂层、各向异性...）中进行替换
* &amp;lbrack；Content&amp;rbrack；颜色变化 — 手动模式可精确选择要更改的颜色
* &amp;lbrack；Content&amp;rbrack；拼贴 — 用于可视化裁剪接缝的选项
* &amp;lbrack；Content&amp;rbrack；拼贴 — 用于绘制裁剪的接缝以实现完美拼贴的选项
* &amp;lbrack；Content&amp;rbrack；匹配 — 添加材质以匹配其颜色和粗糙度的选项
* &amp;lbrack；Content&amp;rbrack；匹配 — 现在可以在图像上工作，以匹配另一图像的颜色
* &amp;lbrack；Content&amp;rbrack；环境光 — 新色温滤镜
* &amp;lbrack；Content&amp;rbrack；环境光 — 新曝光度滤镜
* &amp;lbrack；Content&amp;rbrack；环境光 — 新的曝光度预览滤镜
* &amp;lbrack；Content&amp;rbrack；环境光照 — 新建Nadir Patch滤镜
* &amp;lbrack；Content&amp;rbrack；环境光照 — 新建Nadir Extract滤镜
* &amp;lbrack；Content&amp;rbrack；环境光照 — 新光照滤镜（球体、直线、形状、平面）
* &amp;lbrack；Content&amp;rbrack；环境光照 — 新全景修补滤镜
* &amp;lbrack；Content&amp;rbrack；环境光照 — 新的水平拉直滤镜
* &amp;lbrack；Content&amp;rbrack；环境光照 — 新的HDR合并筛选器

**已知问题：**

* &amp;lbrack；实时引擎2021&amp;rbrack；更改布局，使应用程序崩溃
* &amp;lbrack；实时引擎2021&amp;rbrack；计算繁重，应用程序崩溃
* &amp;lbrack；面板&amp;rbrack； MacOS — 未停靠的面板位于所有应用程序之前
* &amp;lbrack；构件&amp;rbrack；变换和位置构件可能会消失。 隐藏和取消隐藏图层以使其显示。
* &amp;lbrack；导出&amp;rbrack；环境光的SBSAR导出会失去32位深度精度
* 打开文件夹时，&amp;lbrack；资源面板&amp;rbrack；资源可以突出显示
* &amp;lbrack；属性面板&amp;rbrack；重置参数不会重置组合框UI
* &amp;lbrack；本地化&amp;rbrack；更改语言不会影响项目面板，直到重新创建项目面板为止

## 版本2

### 2.3.2 (2020.3.2)粉丝

*（发布日期：2021年2月23日）*

**已添加：**

* 支持&amp;lbrack；本地化&amp;rbrack；日语

**已修复：**

* &amp;lbrack；图层&amp;rbrack；在刺绣滤镜中微调材质时会丢失刺绣图像

**已知问题：**

* 高分辨率图像上“图像到材质”（AI驱动）的使用可能较慢
* “内容识别填充”滤镜在高分辨率下速度较慢
* 在滑块中键入特定值时，可以忽略昏迷或点
* 无法将完全相同的素材图层栈叠存储两次

### 2.3.1 (2020.3.1)粉丝

*（发布日期：2020年12月17日）*

**已添加：**

* &amp;lbrack；引擎&amp;rbrack；Substance 引擎更新
* &amp;lbrack；用于禁用特定功能的应用程序和rbrack；环境变量
* &amp;lbrack；Content&amp;rbrack；替换颜色 — 新的高级分段选项
* &amp;lbrack；Content&amp;rbrack；Floor磁贴 — 可用的新图案和选项
* &amp;lbrack；Content&amp;rbrack；刺绣 — 滤镜的完全改良
* &amp;lbrack；Content&amp;rbrack；调整 — 新的金属参数+不透明度安全变换校正

**已修复：**

* &amp;lbrack；Layers&amp;rbrack；不能导入两次相同的自定义滤镜
* &amp;lbrack；Layers&amp;rbrack；无法使用画笔工具的图像输入
* &amp;lbrack；Export&amp;rbrack；导出.jpg而不是.jpeg
* &amp;lbrack；UI&amp;rbrack；更新欢迎屏幕图像积分
* &amp;lbrack；UI&amp;rbrack；修复菜单中的不可见分隔符
* &amp;lbrack；UI&amp;rbrack；单选按钮在截断时显示工具提示
* &amp;lbrack；UI&amp;rbrack；拼写错误：初学者材质
* 资源名称中的&amp;lbrack；Application&amp;rbrack； UTF-8字符不起作用
* &amp;lbrack；本地化&amp;rbrack；禁用中文区域设置的斜体字体样式
* &amp;lbrack；本地化&amp;rbrack；本地化字符串拆分为两行
* &amp;lbrack；Localization&amp;rbrack；调整文件夹名称，如果名称太长，则使用省略号替换
* &amp;lbrack；Localization&amp;rbrack；格式化带千位分隔符的数字
* &amp;lbrack；本地化&amp;rbrack；本地化日期和时间显示
* &amp;lbrack；本地化&amp;rbrack；在Windows上本地化拾色器
* &amp;lbrack；Content&amp;rbrack；变换 — 激活安全变换后，正常轴每45°可正确旋转一次
* &amp;lbrack；Content&amp;rbrack；表面浮雕 — 使用perlin分形噪声修复拼贴问题（高级噪声）
* &amp;lbrack；Content&amp;rbrack；墙式图案 — 16位Height输入
* &amp;lbrack；Content&amp;rbrack；材料图标渲染 — Specular反射问题
* &amp;lbrack；Content&amp;rbrack；颜色变化 — 颜色输入和结果之间无颜色变化
* &amp;lbrack；Content&amp;rbrack；颜色变化 — 性能更新

**已知问题：**

* 高分辨率图像上“图像到材料”（AI驱动）的使用可能会很慢
* “内容识别填充”滤镜在高分辨率下速度较慢
* 在滑块中键入特定值时，可以忽略昏迷或点
* 无法存储两倍于相同图层堆叠的存储

### 2.3.0 (2020.3.0)粉丝

*（发布日期：2020年10月26日）*

**已添加：**

* &amp;lbrack；图像到材料&amp;rbrack；支持NVIDIA RTX 3000系列
* &amp;lbrack；图像到材料&amp;rbrack；用于控制几何细节的新参数
* &amp;lbrack；要材料的图像&amp;rbrack；用于控制粗糙度的新参数
* &amp;lbrack；要材料的图像&amp;rbrack；用于控制愉悦强度的新参数
* &amp;lbrack；缩略图&amp;rbrack；基于Substance DesignerPBR渲染器的新缩略图生成器
* &amp;lbrack；缩略图&amp;rbrack；更新基础材质和地图集以嵌入缩略图
* &amp;lbrack；缩略图&amp;rbrack；从。sbsar 文件中检索缩略图（如果存在）
* &amp;lbrack；缩览图&amp;rbrack；在“首选项”中更改缩览图品质
* &amp;lbrack；引擎&amp;rbrack；更新为Substance 引擎版本8
* &amp;lbrack；本地化&amp;rbrack；中文本地化
* &amp;lbrack；UI&amp;rbrack；实验性专色拾色器
* &amp;lbrack；Content&amp;rbrack；新环境图- Studio 06
* &amp;lbrack；Content&amp;rbrack；添加Atlas生成器过滤器
* &amp;lbrack；Content&amp;rbrack；添加Atlas Splitter过滤器
* &amp;lbrack；Content&amp;rbrack；添加丢弃的Gums滤镜
* &amp;lbrack；Content&amp;rbrack；添加指纹过滤器
* &amp;lbrack；Content&amp;rbrack；添加Scratches过滤器
* &amp;lbrack；Content&amp;rbrack；添加表面浮雕滤镜（替换Height调制滤镜）
* 打包；内容打包；添加变形滤镜(&amp;R)
* &amp;lbrack；Content&amp;rbrack；添加反转滤镜
* &amp;lbrack；Content&amp;rbrack；添加着色滤镜
* &amp;lbrack；Content&amp;rbrack；添加替换颜色筛选器
* &amp;lbrack；Content&amp;rbrack；变换 — 添加停用特定通道上的转换的可能性
* &amp;lbrack；Content&amp;rbrack；变换 — 激活安全变换时添加旋转
* &amp;lbrack；Content&amp;rbrack；颜色变化 — 添加分段选项以选择如何分布颜色

**已修复：**

* &amp;lbrack；Layers&amp;rbrack；执行多个还原/重做操作时正确更新UI
* &amp;lbrack；图层&amp;rbrack；执行多个撤消/重做操作时防止崩溃
* 使用图像进行材料（AI驱动）时崩溃(&amp;lbrack；Layers&amp;rbrack；)，并记录：设备序号无效
* &amp;lbrack；Filters&amp;rbrack；改进NVIDIA显卡检测以实现NVidia的特定功能
* 关闭应用程序时崩溃&amp;lbrack；应用程序&amp;rbrack；
* &amp;lbrack；Application&amp;rbrack；修复MacOS上的VRAM数量检测
* &amp;lbrack；Export&amp;rbrack；某些导出预设有时缺失
* &amp;lbrack；Content&amp;rbrack；油画绘画效果 — 使用高位移振幅固定Height范围
* &amp;lbrack；Content&amp;rbrack；使其成为高级拼贴 — 在导出时不刷掉基色
* &amp;lbrack；Content&amp;rbrack；使其成为高级拼贴 — 当AO太强时基色上的白色蒙版
* &amp;lbrack；Content&amp;rbrack；调整 — 现在可用于图像(scan1、...)

**已知问题：**

* 高分辨率图像上“图像到材质”（AI驱动）的使用可能较慢
* “内容识别填充”滤镜在高分辨率下速度较慢
* 在滑块中键入特定值时，可以忽略昏迷或点
* 无法将完全相同的素材图层栈叠存储两次

### 2.2.1 (2020.2.1)乌敦

*（发布日期：2020年7月21日）*

**已添加：**

* 当“图像到材料”（AI驱动）内存不足时，出现&amp;lbrack；Layers&amp;rbrack；应用程序内错误消息

**已修复：**

* &amp;lbrack；Layers&amp;rbrack；图像到材料（AI支持）不适用于Specular/光泽度工作流程
* &amp;lbrack；Layers&amp;rbrack；在使用“图像到材质”（AI驱动）时视频内存不足时崩溃
* &amp;lbrack；Layers&amp;rbrack；打开堆叠时不使用磁盘缓存进行显示
* Nvidia RTX 8000的&amp;lbrack；图层和rbrack；检测
* Layers&amp;rbrack；Layers&amp;rbrack；有时不可能将图层移到“飞溅”输入之外(&amp;L)
* 在堆叠中插入堆叠时未使用&amp;lbrack；图层&amp;rbrack；磁盘缓存
* &amp;lbrack；Layers&amp;rbrack；虽然未使用某些通道用法，但会计算这些用法
* 导入图像时，有时会创建空白输出(&amp;l)
* &amp;lbrack；2D 视图&amp;rbrack；切换到绘图模式下的另一个图层活动块平移和缩放
* &amp;lbrack；Content&amp;rbrack；Snow-法线图上的8位问题
* &amp;lbrack；Content&amp;rbrack；路面图案 — 法线图上的8位问题
* &amp;lbrack；Content&amp;rbrack；均衡器 — 法线图上的8位问题
* &amp;lbrack；Content&amp;rbrack；砾石生成器 — 法线图上的8位问题
* &amp;lbrack；Content&amp;rbrack；Floor平铺 — 处理不透明度和Specular level
* &amp;lbrack；Content&amp;rbrack；混合器循环需要导出预设 — 反转法线图
* &amp;lbrack；Content&amp;rbrack；使用“图像到材料”功能校正大型图像的问题（AI支持）
* &amp;lbrack；在出现数据库错误时选择“备份并重新启动”时Application&amp;rbrack；崩溃
* 快速单击同一资源时崩溃&amp;lbrack；Application&amp;rbrack；
* &amp;lbrack；退出时Application&amp;rbrack；稀有崩溃
* 将文件拖放到欢迎屏幕时崩溃(&amp;lbrack；Application&amp;rbrack；)
* 加载损坏的崩溃文件时的&amp;lbrack；Application&amp;rbrack；环境
* &amp;lbrack；Application&amp;rbrack；快速切换渲染的资源时发生罕见崩溃
* &amp;lbrack；应用程序在资源计算时退出时冻结(&amp;R)
* &amp;lbrack；Application&amp;rbrack；在macos上极少启动崩溃
* 启动后立即关闭应用程序时发生&amp;lbrack；Application&amp;rbrack；死锁
* &amp;lbrack；渲染&amp;rbrack； 3D视图有时闪烁
* &amp;lbrack；UI&amp;rbrack；拾色器和随机种子构件未与其余调整对齐
* &amp;lbrack；渲染&amp;rbrack；显示错误的计算时间
* &amp;lbrack；Export&amp;rbrack；某些导出预设有时缺失

**已知问题：**

* 高分辨率图像上“图像到材料”（AI驱动）的使用可能会很慢
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* “内容识别填充”滤镜在高分辨率下速度较慢
* 在滑块中键入特定值时，可以忽略昏迷或点
* 无法存储两倍于相同图层堆叠的存储

### 2.2.0 (2020.2.0)乌敦

*（发布日期：2020年6月15日）*

**已添加：**

* Windows和Linux上提供的&amp;lbrack；Create&amp;rbrack；New Image to 材料（AI驱动）滤镜
* &amp;lbrack；Create&amp;rbrack；将位图重命名为材料到图像到材料(B2M)
* &amp;lbrack；图像导入&amp;rbrack；新建材料创建模板弹出窗口
* &amp;lbrack；图像导入&amp;rbrack；新的“添加基础材质”选项
* &amp;lbrack；图像导入&amp;rbrack；能够在材料创建模板中拖放其他图像
* &amp;lbrack；图像导入&amp;rbrack；能够删除材料创建模板中的图像
* &amp;lbrack；图像导入&amp;rbrack；根据导入位图的文件名自动为其分配通道
* &amp;lbrack；图像导入&amp;rbrack；能够反转法线图
* &amp;lbrack；2D 视图&amp;rbrack；绘画模式简介
* &amp;lbrack；2D 视图&amp;rbrack；绘画拼贴
* &amp;lbrack；2D 视图&amp;rbrack；设置画笔颜色的灰度值
* &amp;lbrack；2D 视图&amp;rbrack；绘画时平移和缩放
* &amp;lbrack；2D 视图&amp;rbrack； X快捷键可反转画笔灰度值
* 用于更改画笔大小的快捷键&amp;lbrack；2D 视图&amp;rbrack；&amp;lbrack；和&amp;rbrack；
* &amp;lbrack；2D 视图&amp;rbrack； Ctrl（或Cmd） +鼠标滚轮更改画笔大小
* &amp;lbrack；2D 视图&amp;rbrack；现在可以在使用仿制修补时修改源位置
* 拖放；图层&amp;R；按住Shift并拖放可自动散点地图集(&amp;L)
* &amp;lbrack；图层&amp;rbrack； Alt +拖放操作可插入材料作为贴花
* &amp;lbrack；Layers&amp;rbrack；从Substance Designer轻松公开转换矩阵
* &amp;lbrack；Layers&amp;rbrack；将纹理放到非空栈栈中会自动分配给正确的通道
* &amp;lbrack；图层&amp;rbrack；新图层类型：复合滤镜
* &amp;lbrack；参数&amp;rbrack；支持Substance字符串输入
* &amp;lbrack；UI&amp;rbrack；为弹出窗口和菜单添加了投影
* &amp;lbrack；UI&amp;rbrack；带右键单击选项的新颜色构件（清除、复制、粘贴）
* 带绘画工具选项的&amp;lbrack；UI&amp;rbrack；新建图像构件
* &amp;lbrack；UI&amp;rbrack；能够在图像小组件中导入的图像上绘画
* &amp;lbrack；渲染&amp;rbrack；新默认相机位置
* 为Substance Designer2020.1.2 (10.1.2)导出&amp;lbrack；导出&amp;rbrack；Substance文件
* Lbrack；Performance&amp;rbrack；更好的应用程序启动时间(&amp;L)
* &amp;lbrack；Performance&amp;rbrack；改进异步任务处理
* &amp;lbrack；Performance&amp;rbrack；在添加、删除或移动图层时提高图层栈栈性能
* &amp;lbrack；性能&amp;rbrack；图像到材料（AI驱动）在RTX GPU上运行速度更快
* &amp;lbrack；Content&amp;rbrack；新网格：女性T恤、男性T恤、鞋
* &amp;lbrack；Content&amp;rbrack；新混合模式 — 每通道混合
* &amp;lbrack；Content&amp;rbrack；使用2个新参数（Height位置和Height比例）进行不透明度混合Height校正
* &amp;lbrack；Content&amp;rbrack；在混合模式下添加Height调整
* &amp;lbrack；Content&amp;rbrack；使用“自定义蒙版”混合中的Height信息选项
* &amp;lbrack；Content&amp;rbrack；新透视校正工具
* &amp;lbrack；Content&amp;rbrack；图案生成器 — 添加参数以反转图案
* &amp;lbrack；Content&amp;rbrack；模式生成器 — 添加新的参数覆盖材料详细信息
* 标记；内容标记；新建贴花滤镜(&amp;R)
* &amp;lbrack；Content&amp;rbrack；新Moss筛选器
* &amp;lbrack；Content&amp;rbrack；新裂缝过滤器
* &amp;lbrack；Content&amp;rbrack；新建PBR 验证过滤器
* &amp;lbrack；Content&amp;rbrack；新建Floor拼贴过滤器
* &amp;lbrack；Content&amp;rbrack；新建面组贴图滤镜
* &amp;lbrack；Content&amp;rbrack；Atlas Scatter — 添加自定义蒙版输入以启用绘画选项
* &amp;lbrack；Content&amp;rbrack；Dirt — 添加自定义蒙版输入以启用绘画选项
* 打包；内容打包；克隆导出预设(&amp;R)
* &amp;lbrack；Content&amp;rbrack； VStitcher导出预设
* &amp;lbrack；Content&amp;rbrack； Unity HDRP预设导出detailMap

**已修复：**

* 加载导入的图像太多次(&amp;L)
* 在堆叠底部创建仿制修补程序时崩溃&amp;lbrack；图层&amp;rbrack；
* &amp;lbrack；Layers&amp;rbrack；在堆叠底部添加材料会使其不稳定
* 导入图像后，Layers&amp;Rbrack；滤镜工作不正常(&amp;L)
* 在使用自定义筛选器的项目之间切换工作流时，&amp;lbrack；Layers&amp;rbrack； workflow_type值不会更新
* &amp;lbrack；Layers&amp;rbrack；未选中任何图层时禁用“移除图层”按钮
* 加载包含仿制修补程序的资源时崩溃(&amp;lbrack；Layers&amp;rbrack；)
* &amp;lbrack；图层&amp;rbrack；正常到Height滤镜在MacOs上崩溃
* 在来回加载环境图时&amp;lbrack；Application&amp;rbrack；崩溃
* 安装某些图形输入板驱动程序时出现应用程序和Rbrack；性能问题(&amp;L)
* &amp;lbrack；Application&amp;rbrack； EXR 32位文件导入为黑色
* 加载和卸载资源时的Application&amp;rbrack；崩溃(&amp;L)
* 从浏览切换到创建时崩溃&amp;lbrack；应用程序&amp;rbrack；
* 保存素材时目标集合不是来自当前项目的(&amp;L)
* &amp;lbrack；应用程序&amp;rbrack；修复备份并重新启动
* &amp;lbrack；图像导入&amp;rbrack；正确导入灰度图像
* &amp;lbrack；Content&amp;rbrack；用于新矩阵处理的新筛选器
* 导入的自定义滤镜在快速访问栏中可见(&amp;L)
* &amp;lbrack；Content&amp;rbrack；使用Make it tile高级滤镜修复色偏
* &amp;lbrack；Performance&amp;rbrack；打开颜色对话框时速度较慢并重新计算当前图层
* 键盘快捷键有时不起作用(&amp;L)
* &amp;lbrack；2D视图&amp;rbrack；内容识别填充需要无用的首次单击才能使用
* 删除本地磁盘中的文件夹后，仍会监视这些文件夹是否有更新(&amp;L)
* &amp;lbrack；资源&amp;rbrack；从文件系统中删除链接文件夹不会将其删除
* 不导出自定义导出预设中的自定义用途(&amp;L)
* &amp;lbrack；导出&amp;rbrack；导出路径中包含特殊字符的.sbsar文件失败

**已知问题：**

* 重复计算“图像到材质”（AI驱动）可能会触发崩溃（内存不足）
* 反复重新计算Delighter可能会触发崩溃（内存不足）
* 高分辨率图像上“图像到材质”（AI驱动）的使用可能较慢
* 在低VRAM的GPU上使用图像到材质（AI驱动）可能会触发崩溃（内存不足）
* “图像到材质”（AI驱动）在PBRSpecular/光泽度上不可用
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* “内容识别填充”滤镜在高分辨率下速度较慢
* 在滑块中键入特定值时，可以忽略昏迷或点
* 无法将完全相同的素材图层栈叠存储两次

### 2.1.1 (2020.1.1)提拉米苏

*（发布日期：2020年4月1日）*

**已添加：**

* &amp;lbrack；Project&amp;rbrack；导出和导入元数据
* &amp;lbrack；Application&amp;rbrack；Ctrl+S现在可在Explore中保存预设
* &amp;lbrack；Performance&amp;rbrack；使用渲染缓存，而不是重新计算保存的材质，分辨率最高可达2k

**已修复：**

* &amp;lbrack；UI&amp;rbrack；视口中的固定计算指示器
* &amp;lbrack；UI&amp;rbrack；在滑块中输入负值是固定的
* &amp;lbrack；UI&amp;rbrack；组合框：键盘箭头和滚动条现在可以使用
* &amp;lbrack；UI&amp;rbrack；在2D 视图中的“材料输出”和“图层输入”之间切换时，保留选定的通道
* &amp;lbrack；图层&amp;rbrack；修复了在基础材质中添加自定义声道时崩溃的问题
* &amp;lbrack；处理图层时的图层&amp;rbrack；崩溃
* &amp;lbrack；Layers&amp;rbrack；自定通道不与保存的材质一起显示
* &amp;lbrack；Application&amp;rbrack；修复了导入资源时出现的罕见崩溃
* &amp;lbrack；Application&amp;rbrack；退出时崩溃
* 切换预设时，&amp;lbrack；Application&amp;rbrack；组合框现在会显示正确的值
* &amp;lbrack；Export&amp;rbrack；已将Enscape预设重命名为Enscape Revit
* &amp;lbrack；Export&amp;rbrack；删除导出预设后可导入它
* &amp;lbrack；导出时导出&amp;rbrack；崩溃
* &amp;lbrack；渲染&amp;rbrack；固定base color为16位半浮点格式时的渲染
* &amp;lbrack；Project&amp;rbrack；在导入损坏的包时不崩溃
* &amp;lbrack；Project&amp;rbrack；从未打开创建时处理2019.1.4到2.x.x的迁移
* &amp;lbrack；Project&amp;rbrack；在两次导入同一项目时修复崩溃
* &amp;lbrack；Project&amp;rbrack；导入项目时修复崩溃
* &amp;lbrack；资源在早期版本中导入的自定义筛选器有效(&amp;R)
* &amp;lbrack；具有相同名称的资源&amp;rbrack；材料不再相互擦除
* 链接本地文件夹时资源崩溃(&amp;L)
* &amp;lbrack；资源和rbrack；初学者材质用户创建的文件夹在重新启动后不再被删除
* &amp;lbrack；Inspire&amp;rbrack；修复材料/收藏夹放置区域，并在使用未保存的材料时添加警告消息

**已知问题：**

* “内容识别填充”滤镜在高分辨率下速度较慢
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 在滑块中键入特定值时，可以忽略昏迷或点

### 2.1.0 (2020.1.0)提拉米苏

*（发布日期：2020年3月12日）*

**已添加：**

* &amp;lbrack；导出&amp;rbrack；导出预设选项，为渲染器和游戏引擎打包纹理
* &amp;lbrack；导出&amp;rbrack；将预设导出为虚构引擎4
* &amp;lbrack；导出&amp;rbrack；将预设导出为Unity Standard
* &amp;lbrack；导出&amp;rbrack；将预设导出到Unity HDRP
* &amp;lbrack；导出&amp;rbrack；将预设导出到混合器循环/循环
* &amp;lbrack；导出&amp;rbrack；将预设导出到Arnold 5
* &amp;lbrack；导出&amp;rbrack；将预设导出到电晕渲染器
* &amp;lbrack；导出&amp;rbrack；将预设导出到Encape
* &amp;lbrack；导出&amp;rbrack；将预设导出到Keyshot 9
* &amp;lbrack；导出&amp;rbrack；将预设导出到Redshift(&amp;L)
* &amp;lbrack；导出&amp;rbrack；将预设导出到Vray Next
* &amp;lbrack；导出&amp;rbrack；将预设导出到Lens Studio
* 打包；导出&amp;rbrack；将预设导出到Spark AR Studio(&amp;L)
* &amp;lbrack；导出&amp;rbrack；将预设从PBR金属粗糙度导出到PBRSpecular光泽度
* &amp;lbrack；导出&amp;rbrack；新的导出UI
* &amp;lbrack；导出&amp;rbrack；记住导出设置
* &amp;lbrack；导出&amp;rbrack；导入和管理自定义导出预设
* &amp;lbrack；Export&amp;rbrack；删除和替换自定义导出预设
* &amp;lbrack；Export&amp;rbrack；重命名自定义导出预设
* &amp;lbrack；Export&amp;rbrack；将默认导出分辨率设置为当前分辨率
* &amp;lbrack；Export&amp;rbrack；将创建子文件夹的选项添加到导出位置
* &amp;lbrack；Export&amp;rbrack；替换现有文件前的警告消息
* &amp;lbrack；应用程序&amp;rbrack；新版本编号方案
* &amp;lbrack；Application&amp;rbrack；在启动时打开创建并更改实验室顺序
* &amp;lbrack；欢迎屏幕&amp;rbrack；新的欢迎横幅
* &amp;lbrack；Project&amp;rbrack；启动时打开上一个项目
* 打包；UI&amp;rbrack；新建组合框样式(&amp;L)
* &amp;lbrack；2D视图&amp;rbrack；在2D视图中聚焦的快捷键
* &amp;lbrack；Filters&amp;rbrack；在图形中添加了对alchemist：：parameterVisibility标记的支持
* &amp;lbrack；Filters&amp;rbrack；进行全局调整，以根据工作流程管理参数可见性
* &amp;lbrack；资源&amp;rbrack；使用配置文件设置资源和链接文件夹的新命令行选项
* &amp;lbrack；版本检查器&amp;rbrack；版本检查的配置
* &amp;lbrack；Content&amp;rbrack；新入门材料
* &amp;lbrack；Content&amp;rbrack；将位图转换为素材 — 添加定义金属通道的可能性（统一、自定义图像导入、拾色）
* &amp;lbrack；Content&amp;rbrack；调整 — 添加对PBRSpecular/光泽度工作流程的支持
* &amp;lbrack；Content&amp;rbrack；Atlas Scatter — 新参数

**已修复：**

* 两次导入同一项目时崩溃&amp;lbrack；项目&amp;rbrack；
* &amp;lbrack；Project&amp;rbrack；在多次导入和打开项目时修复了崩溃
* 加载未命名材料时的&amp;lbrack；Application&amp;rbrack；崩溃
* &amp;lbrack；Application&amp;rbrack；重新导入缺失的文件时识别它们
* &amp;lbrack；Application&amp;rbrack；在关机时修复随机崩溃
* &amp;lbrack；Application&amp;rbrack；修复了在Create中卸载材料时出现的罕见崩溃
* &amp;lbrack；Application&amp;rbrack；修复了使用UI控件时的随机崩溃
* &amp;lbrack；应用程序&amp;rbrack；修复了在Windows 10上将日志文件导出到桌面的问题
* 当您在“创建”面板中打开时，&amp;lbrack；UI&amp;rbrack；导出面板的大小不正确
* &amp;lbrack；UI&amp;rbrack；单击即可打开项目
* &amp;lbrack；UI&amp;rbrack；正确设置了滑块的最小值和最大值
* &amp;lbrack；UI&amp;rbrack；显示通道用法的标签而不是ID
* &amp;lbrack；UI&amp;rbrack；单击材料时总是打开/关闭调整面板
* 打包；UI&amp;rbrack；修复隐藏图层颜色(&amp;L)
* &amp;lbrack；UI&amp;rbrack；欢迎屏幕按钮改进
* Lbrack；Layers&amp;rbrack；不必要的重新计算(&amp;L)
* 使用“仿制修补”时崩溃Layers&amp;rbrack；(&amp;L)
* &amp;lbrack；Layers&amp;rbrack；选择图像导入图层不再触发计算
* &amp;lbrack；Layers&amp;rbrack；仿制修补和内容识别填充图层在选中时不再重新计算
* &amp;lbrack；通道设置&amp;rbrack；启用或禁用使用现在会触发渲染
* &amp;lbrack；资源&amp;rbrack；在批量单击库中的堆叠时防止冻结
* 重新添加以前添加的链接文件夹时&amp;lbrack；资源和rbrack；性能受到影响
* &amp;lbrack；资源&amp;rbrack；在尝试打开已删除的。sbsar 文件时修复了崩溃
* &amp;lbrack；Performance&amp;rbrack；避免加载材料以访问其参数
* &amp;lbrack；仅在项目或创作材料中使用时，才备份资源(&amp;R)
* &amp;lbrack；Export&amp;rbrack；导出队列中的固定素材有时会被跳过或用错误的参数导出
* &amp;lbrack；2D 视图&amp;rbrack；恢复平移和缩放
* Content&amp;rbrack；镶板图案考虑了Ambient occlusion声道(&amp;L)
* &amp;lbrack；Content&amp;rbrack；绘画 — 启用自定义蒙版时显示蒙版输入
* &amp;lbrack；Content&amp;rbrack； Stonewall图案 — 在法线图中移除可能的带状效果
* &amp;lbrack；Content&amp;rbrack；Height调制 — 校正2d视图中的双base color条目

**已知问题：**

* “内容识别填充”滤镜在高分辨率下速度较慢
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 在滑块中键入特定值时，可以忽略昏迷或点

## 版本1

### 1.1.4 (2019.1.4)芝麻

*（发布日期：2020年1月30日）*

**已添加：**

* 清除资源文件夹时的&amp;lbrack；资源和rbrack；确认提示

**已修复：**

* Lbrack；Layers&amp;rbrack；将图层移动到下方或上方的两个或更多图层(&amp;L)
* &amp;lbrack；Create&amp;rbrack；分配足够的VRAM预算以获得良好的性能

**已知问题：**

* 导入大量资源确实会减慢Substance Alchemist速度
* “内容识别填充”滤镜在高分辨率下速度较慢
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可以在MacOS上崩溃

### 1.1.3 (2019.1.3)芝麻

*（发布日期：2020年1月28日）*

**已添加：**

* &amp;lbrack；Workflow&amp;rbrack；支持多个工作流
* &amp;lbrack；Workflow&amp;rbrack；支持PBR光泽度工作流
* &amp;lbrack；Workflow&amp;rbrack；新建通道设置面板
* &amp;lbrack；创建项目时的工作流选择&amp;rbrack；工作流
* &amp;lbrack；通道设置&amp;rbrack；激活/停用特定通道计算
* &amp;lbrack；声道设置&amp;rbrack；显示当前材料中可用的自定义声道列表
* &amp;lbrack；声道设置&amp;rbrack；需要时自动计算自定义声道
* &amp;lbrack；声道设置&amp;rbrack；强制/阻止计算自定义声道
* &amp;lbrack；图层&amp;rbrack；Atlas Scatter和飞溅滤镜中材料输入占位符的新UI
* 滤镜的图像输入参数可通过下面的图层提供(&amp;L)
* &amp;lbrack；图层&amp;rbrack；在某些图层过期时显示通知
* &amp;lbrack；Layers&amp;rbrack；可通过通知更新到过时图层的最新版本
* &amp;lbrack；Project&amp;rbrack；项目创建时的新元数据字段
* &amp;lbrack；Inspire&amp;rbrack；生成的变体特定于项目
* &amp;lbrack；2D 视图&amp;rbrack；在图层输入、图层输出和材料输出之间切换
* &amp;lbrack；欢迎屏幕&amp;rbrack；添加导入项目(.alch)选项
* &amp;lbrack；Preferences&amp;rbrack；用于设置缓存位置和分析隐私设置的新首选项窗口
* &amp;lbrack；UI&amp;rbrack；新建UI按钮
* 并行化系统的整体改进(&amp;L)
* &amp;lbrack；性能优化&amp;rbrack；材料计算数的优化
* &amp;lbrack；引擎&amp;rbrack；Substance 引擎更新
* &amp;lbrack；Framework&amp;rbrack；升级到Qt 5.13
* &amp;lbrack；MacOS&amp;rbrack；对macOS Catalina支持的全局改进
* &amp;lbrack；Content&amp;rbrack；调整滤镜 — 法线强度和反转参数

**已修复：**

* 删除图层时&amp;lbrack；图层&amp;rbrack；取消设置图像输入参数
* &amp;lbrack；图层&amp;rbrack；在添加仿制修补图层时修复崩溃
* &amp;lbrack；Layers&amp;rbrack；修复在其他材料中混合图层堆叠材料时出现的某些崩溃
* 现在遵循导出的&amp;lbrack；Export&amp;rbrack；通道选择
* &amp;lbrack；资源在“资源”面板中导航时不崩溃(&amp;R)
* &amp;lbrack；资源&amp;rbrack；在导入损坏的Substance文件时修复崩溃
* &amp;lbrack；资源&amp;rbrack；在加载大型文件夹时减少崩溃数量
* &amp;lbrack；缩略图&amp;rbrack；缩略图计算不会冻结界面
* &amp;lbrack；映像导入&amp;rbrack；统一整个应用程序支持的映像类型
* &amp;lbrack；预设&amp;rbrack；从SBSAR创建预设时保存描述
* &amp;lbrack；Inspire&amp;rbrack；修复图像拖放问题
* &amp;lbrack；Application&amp;rbrack；在退出时修复崩溃
* &amp;lbrack；Application&amp;rbrack；在导出崩溃时在退出时修复材料
* &amp;lbrack；UI&amp;rbrack；修复和改进
* &amp;lbrack；UI&amp;rbrack；将临时资源重命名为“未保存的材料”
* &amp;lbrack；Content&amp;rbrack；所有滤镜的全局更新和清理

**已知问题：**

* 导入大量资源确实会减慢Substance Alchemist速度
* “内容识别填充”滤镜在高分辨率下速度较慢
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可以在MacOS上崩溃

### 1.1.2 (2019.1.2)芝麻

*（发布日期：2019年12月11日）*

**已添加：**

* 可通过图层堆叠工具栏中的界面访问&amp;lbrack；图层&amp;rbrack；保存和另存为选项
* &amp;lbrack；资源&amp;rbrack；可在“资源”面板中导航文件夹的Clearer痕迹导航
* &amp;lbrack；资源&amp;rbrack；按住后退按钮以访问所有上层文件夹
* &amp;lbrack；资源&amp;rbrack；添加重新加载导入的材料选项以将其更新到最新版本
* layers&amp;rbrack；可在“图像导入”图层中更改图像
* &amp;lbrack；Layers&amp;rbrack；可将图像定义为声道（base color、正常、Height...） 在图像导入图层中
* &amp;lbrack；Content&amp;rbrack；新Atlas Scatter筛选器以从Substance Source散点新的贴图集元素
* &amp;lbrack；Content&amp;rbrack；新油绘画效果滤镜
* &amp;lbrack；Content&amp;rbrack；新通道生成滤镜，可根据基色和法线图生成Height、环境遮蔽和粗糙度

**已修复：**

* &amp;lbrack；UI&amp;rbrack；重新激活图层栈栈工具栏上的工具提示
* &amp;lbrack；UI&amp;rbrack；修复在滑块值中键入两个小数点时出现的问题
* &amp;lbrack；Performance&amp;rbrack；修复在材料之间快速切换时的崩溃
* &amp;lbrack；Export&amp;rbrack；在导出结束前切换到另一材料不再会崩溃
* 右键单击材料时，&amp;lbrack；资源和rbrack；上下文菜单显示在列表顶部
* &amp;lbrack；Layers&amp;rbrack；当图层栈栈为空时，“单击此处”链接有效
* 如果是在Alchemist中创建的材料，&amp;lbrack；预设&amp;rbrack；删除“调整”面板中的“存储”按钮
* &amp;lbrack；调整&amp;rbrack；在Alchemist中创建的材料时显示的信息消息
* &amp;lbrack；Viewport&amp;rbrack；Specular level纹理的默认值被更正为0.04
* &amp;lbrack；文件菜单&amp;rbrack；修复并重命名“保存”和“另存为”选项
* &amp;lbrack；引擎&amp;rbrack；更新Substance引擎版本以避免在导入期间崩溃某些SBSAR文件。
* &amp;lbrack；Content&amp;rbrack；拼贴滤镜正在环境遮蔽通道上工作
* &amp;lbrack；Content&amp;rbrack；裁剪滤镜正在ambient occlusion频道上工作
* &amp;lbrack；Content&amp;rbrack；水滤镜修改获得高度图
* &amp;lbrack；Content&amp;rbrack；在不透明度混合模式下更正顶部材料的拼贴
* &amp;lbrack；顶层材料的Content&amp;rbrack；Height在不透明度混合模式下保留
* &amp;lbrack；Content&amp;rbrack；可在“穿孔”滤镜中添加自定义蒙版、自定义图案或比例图
* &amp;lbrack；Content&amp;rbrack；Height调制滤镜强制Height和法线图使用16位
* &amp;lbrack；Content&amp;rbrack；调整筛选器强制16位Height和法线图

**已知问题：**

* 导入大量资源确实会减慢Substance Alchemist速度
* “内容识别填充”滤镜在高分辨率下速度较慢
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可以在MacOS上崩溃

### 1.1.1 (2019.1.1)芝麻

*（发布日期：2019年11月26日）*

**已添加：**

* &amp;lbrack；混合&amp;rbrack；新不透明度混合模式
* &amp;lbrack；引擎&amp;rbrack；新Substance 引擎版本

**已修复：**

* &amp;lbrack；Layers&amp;rbrack；在删除仍在计算的图层时修复崩溃
* &amp;lbrack；Layers&amp;rbrack；在删除底部图层时修复崩溃
* &amp;lbrack；图层&amp;rbrack；修复材料名包含特殊字符时的崩溃
* &amp;lbrack；Layers&amp;rbrack；停止计算每个使用小部件的滤镜
* &amp;lbrack；Layers&amp;rbrack；在使用“仿制修补”和“内容识别填充”滤镜时，避免崩溃
* &amp;lbrack；图层&amp;rbrack；在飞溅输入插槽中拖放滤镜时修复崩溃
* &amp;lbrack；资源&amp;rbrack；修复链接本地文件夹或在Substance Alchemist中导入资源时的崩溃
* &amp;lbrack；Collection&amp;rbrack；修复崩溃，同时在材料之间快速切换
* &amp;lbrack；UI&amp;rbrack；在视口上的拼贴和位移滑块中，当值为空或无效时修复崩溃
* 访问“启发”选项卡时&amp;lbrack；Inspire&amp;rbrack；修复崩溃
* &amp;lbrack；Inspire&amp;rbrack；修复刚刚保存的图层材料上的崩溃，同时为之提供灵感
* &amp;lbrack；性能&amp;rbrack；重型材料和滤镜(拼贴)计算速度更快
* &amp;lbrack；帮助&amp;rbrack；修复导出日志文件
* &amp;lbrack；Content&amp;rbrack；随机化滤镜适用于所有渠道
* &amp;lbrack；Content&amp;rbrack；多角度工作流程会考虑所有扫描
* &amp;lbrack；Content&amp;rbrack； AO混合正确混合
* &amp;lbrack；Content&amp;rbrack；混合正确混合
* &amp;lbrack；Content&amp;rbrack；颜色ID混合正确混合
* &amp;lbrack；Content&amp;rbrack；自定义蒙版混合校正混合
* &amp;lbrack；Content&amp;rbrack；修复调整筛选器以修改粗糙度(&amp;R)
* &amp;lbrack；Content&amp;rbrack；修复用于自定义普通通道上传的基础材质筛选器
* &amp;lbrack；Content&amp;rbrack；修复浮雕滤镜的自定义导入图案

**已知问题：**

* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可以在MacOS上崩溃

### 1.1.0 (2019.1.0)芝麻

*（发布日期：2019年11月4日）*

**已添加：**

* 创建项目(&amp;L)
* &amp;lbrack；Project&amp;rbrack；包含项目数据的.alch文件格式简介
* &amp;lbrack；Project&amp;rbrack；导出包含集合及其lch项目
* &amp;lbrack；项目&amp;rbrack；导入.alch项目
* &amp;lbrack；Project&amp;rbrack；打开最近的项目
* &amp;lbrack；欢迎屏幕&amp;rbrack；启动时会显示欢迎屏幕
* &amp;lbrack；欢迎使用屏幕&amp;rbrack；从欢迎使用屏幕创建项目
* &amp;lbrack；欢迎使用屏幕&amp;rbrack；访问欢迎使用屏幕中所有项目的列表
* &amp;lbrack；欢迎屏幕&amp;rbrack；用于访问文档、弹出窗口和许可证管理的快速链接
* &amp;lbrack；文件菜单&amp;rbrack；集成文件菜单
* &amp;lbrack；文件菜单&amp;rbrack；从“文件”选项卡访问项目命令并保存图层堆叠
* &amp;lbrack；文件菜单&amp;rbrack；从“编辑”选项卡访问撤消和重做命令
* &amp;lbrack；File Menu&amp;rbrack；前一个帮助菜单移动到“帮助”选项卡下的“文件”菜单中
* &amp;lbrack；Layers&amp;rbrack；图层堆叠的新体系结构
* &amp;lbrack；图层&amp;rbrack；图层堆叠的新UI
* &amp;lbrack；Layers&amp;rbrack；直接在工具栏中选择混合模式
* &amp;lbrack；图层&amp;rbrack；分别访问混合参数和材料参数
* &amp;lbrack；Layers&amp;rbrack；直接在图层堆叠中“飞溅”滤镜的专用输入中添加材料
* &amp;lbrack；图层&amp;rbrack；直接在图像导入图层中更改扫描顺序
* &amp;lbrack；视口&amp;rbrack；控制相机视角
* &amp;lbrack；视口&amp;rbrack；在正交或透视相机之间切换的可能性
* &amp;lbrack；视口&amp;rbrack；显示每个通道的分辨率和位深度信息
* &amp;lbrack；资源&amp;rbrack；基础材质按缺省值打开
* &amp;lbrack；缓存&amp;rbrack；查找缩览图缓存文件夹
* &amp;lbrack；缓存&amp;rbrack；查找渲染缓存文件夹
* &amp;lbrack；面板&amp;rbrack；材料设置面板暂时隐藏
* &amp;lbrack；Workflow&amp;rbrack；Specular/光泽度暂时停用
* &amp;lbrack；MacOS&amp;rbrack； Catalina OS版本公证
* &amp;lbrack；Content&amp;rbrack；Delighter滤镜的新版本
* &amp;lbrack；Content&amp;rbrack；新建图像内容识别填充滤镜
* &amp;lbrack；Content&amp;rbrack；新材料内容识别填充滤镜
* &amp;lbrack；Content&amp;rbrack；变换筛选器具有安全变换选项

**已修复：**

* 以前，所有与“创建”相关的错误现在都不再有效（新的UI和体系结构版本）
* 工具提示不会隐藏顶部栏(3D、2D、2D/3D)中的图标
* &amp;lbrack；Content&amp;rbrack；飞溅滤镜接受具有完整高度图的Atlas
* &amp;lbrack；Content&amp;rbrack；变换滤镜对图像(scan1、scan2、...)有效

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可能会在MacOS上崩溃

## 测试版

### 0.8.1-beta藜麦

*（发布日期：2019年8月19日）*

**已添加：**

* 能够将Substance Source资源从启动器发送到项目Substance Alchemist

**已修复：**

* &amp;lbrack；Create&amp;rbrack；某些滤镜列在快速访问器中，但未列在滤镜面板中
* &amp;lbrack；MacOS&amp;rbrack；修复了退出时出现的一些崩溃问题

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* 不建议使用“愉悦”阶段的快速可见性切换
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可能会在MacOS上崩溃
* 在MacOS上退出时仍然可以随机崩溃

### 0.8.0-beta藜麦

*（发布日期：2019年8月8日）*

**已添加：**

* &amp;lbrack；资源&amp;rbrack；在本地磁盘上连接和镜像材质文件夹
* &amp;lbrack；资源&amp;rbrack；浏览您的材质文件夹及其子文件夹
* &amp;lbrack；资源&amp;rbrack；将材质资源面板分离到一个单独的窗口中，以全屏查看资源
* &amp;lbrack；资源&amp;rbrack；支持文件夹和子文件夹导航的新资源面板布局
* &amp;lbrack；资源&amp;rbrack；使用breadcrum浏览文件夹
* &amp;lbrack；资源&amp;rbrack；强制同步您的本地文件夹，通过右键单击使用“同步”选项进行同步
* &amp;lbrack；资源&amp;rbrack；断开您的本地文件夹连接，通过右键单击可访问“断开连接”选项
* &amp;lbrack；Manage&amp;rbrack；显示Substance文件的嵌入标签
* &amp;lbrack；管理&amp;rbrack；添加、编辑和删除材料的标签
* 打包；管理和打包；评价材质(&amp;R)
* &amp;lbrack；图层&amp;rbrack；支持全景输出
* &amp;lbrack；Layers&amp;rbrack；您可以在“图像导入”图层中删除图像输入
* &amp;lbrack；图层&amp;rbrack；自动选择新添加的图层
* 图层删除后自动选择下方图层的&amp;lbrack；图层&amp;rbrack；
* &amp;lbrack；UX&amp;rbrack；在切换到其他实验室时保持左面板可见性
* &amp;lbrack；UX&amp;rbrack；在非空图层栈栈中导入图像时，不创建基底图层或打开材质工作流程弹出窗口
* &amp;lbrack；UI&amp;rbrack；新建文本字段样式
* &amp;lbrack；UI&amp;rbrack；新建搜索框样式
* &amp;lbrack；UI&amp;rbrack；新建面板标题样式
* 打包；UI&amp;rbrack；新建忙碌指示器样式(&amp;L)
* &amp;lbrack；UI&amp;rbrack；新建图层堆叠背景样式
* &amp;lbrack；UI&amp;rbrack；使用Adobe Clean字体
* &amp;lbrack；UI&amp;rbrack；移除颜色输入参数的吸管图标占位符
* Lbrack；Performance&amp;rbrack；忙碌指示器优化(&amp;R)
* &amp;lbrack；Content&amp;rbrack；新模式生成器过滤器
* 标记；内容标记；新建模糊滤镜(&amp;R)

**已修复：**

* &amp;lbrack；Inspire&amp;rbrack；在使用10种以上颜色时修复崩溃
* &amp;lbrack；2D 视图&amp;rbrack；在2D 视图的频道列表中修复滚动条
* &amp;lbrack；Viewer&amp;rbrack；在导入非2次幂的环境图时修复崩溃
* &amp;lbrack；Content&amp;rbrack；为浮雕和穿孔滤镜的自定义图案修复PNG导入
* &amp;lbrack；导出&amp;rbrack；修复普通和Height16位/通道导出
* 在导入包含两个同名预设的材料时，修复无限循环
* 修复基础材质图层中显示的长文件路径

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* 不建议使用“愉悦”阶段的快速可见性切换
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可能会在MacOS上崩溃
* 在MacOS上退出时可能会随机崩溃

### 0.7.0-beta胡椒

*（发布日期：2019年6月13日）*

**已添加：**

* &amp;lbrack；Filters&amp;rbrack；通过按空格键可快速访问滤镜
* &amp;lbrack；Filters&amp;rbrack；新的专用面板用于管理、浏览和导入过滤器
* &amp;lbrack；元数据&amp;rbrack；右键单击材料以查看其元数据
* &amp;lbrack；元数据&amp;rbrack；右键单击材料以查看其在磁盘上的位置
* 按住Ctrl键将滑块悬停在Animate滑块上时(&amp;L)
* 按P停止并重新启动滑块动画(&amp;L)
* &amp;lbrack；导出&amp;rbrack； SBSAR导出遵循Substance Source准则
* &amp;lbrack；License&amp;rbrack；使用环境变量激活Substance Alchemist
* &amp;lbrack；UX&amp;rbrack；的“文件”对话框记住最后选定的文件路径
* &amp;lbrack；UX&amp;rbrack；文件夹对话框记住最后一个选定的文件夹路径
* &amp;lbrack；UI&amp;rbrack；更新资源面板UI
* &amp;lbrack；UI&amp;rbrack；更新搜索栏UI
* &amp;lbrack；更新UI&amp;rbrack；“创建新材料”图标
* &amp;lbrack；帮助&amp;rbrack； URL更新为substance3d.com域
* 现在提供了&amp;lbrack；网格&amp;rbrack；布料网格
* &amp;lbrack；Content&amp;rbrack；新腐蚀过滤器
* 标记；Content&amp;Rbrack；新氧化滤镜(&amp;L)
* &amp;lbrack；Content&amp;rbrack；新建Moss筛选器
* &amp;lbrack；Content&amp;rbrack；新建Dust过滤器
* brack；Content&amp;rbrack；新建墙式图案滤镜(&amp;L)
* &amp;lbrack；Content&amp;rbrack；新建石墙图案过滤器
* &amp;lbrack；Content&amp;rbrack；新建木饰面滤镜
* &amp;lbrack；Content&amp;rbrack；新金属光洁度滤镜
* &amp;lbrack；Content&amp;rbrack；新建Snow过滤器
* &amp;lbrack；Content&amp;rbrack；新建随机化筛选器
* &amp;lbrack；Content&amp;rbrack；现在可直接在纹理过滤器中导入基础材质

**已修复：**

* 在保存图层堆叠时修复崩溃
* 可以在环境旋转滑块中添加一个大于1的值
* 在将混合图层从混合图层来回变换到材料图层时，不会丢失混合参数
* 在多次生成同一图层堆叠的变体时修复重复项
* 重新打开材料时，Alchemist会记住已修改的滑块范围（最小和最大）

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* 不建议使用“愉悦”阶段的快速可见性切换
* 自定义环境导入可能会变成黑色
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点
* “正常使用Height”滤镜可能会在MacOS上崩溃

### 0.6.1-Beta橙色

*（发布日期：2019年6月13日）*

**已添加：**

* &amp;lbrack；引擎&amp;rbrack；Substance 引擎更新以便与最新Substance Designer版本兼容
* &amp;lbrack；License&amp;rbrack；更新首次安装的许可证文件夹
* &amp;lbrack；图层&amp;rbrack；可随时重新加载您的图层堆叠以更新自定义滤镜(&amp;R)

**已修复：**

* &amp;lbrack；数据兼容性&amp;rbrack；用于在升级时限制数据损坏的预防性修复

**已知问题：**

* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 不建议使用“愉悦”阶段的快速可见性切换
* 自定义环境导入可能会变成黑色
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点

### 0.6.0-Beta橙色

*（发布日期：2019年4月18日）*

**已添加：**

* &amp;lbrack；元数据&amp;rbrack；在专用选项卡中查看和填充材料元数据
* &amp;lbrack；Collection&amp;rbrack；直接从搜索结果创建集合
* &amp;lbrack；媒体发布&amp;rbrack；导出收藏夹的展示板
* 按Ctrl+Z撤消微调更改或图像导入(&amp;L)；UX&amp;R
* 按Ctrl+Shift+Z重做微调更改或图像导入(&amp;L)
* 打包；UI打包；具有新样式的新图标(&amp;L)
* &amp;lbrack；Performance&amp;rbrack；新的会话管理器可更好地处理选项卡切换
* &amp;lbrack；Performance&amp;rbrack；更快地打开图像导入图层
* &amp;lbrack；Content&amp;rbrack；新建Metal通用材料
* &amp;lbrack；Content&amp;rbrack；新建材料
* &amp;lbrack；Content&amp;rbrack；新建石头通用材料
* &amp;lbrack；Content&amp;rbrack；浮雕过滤器更新
* 标记；内容标记；刺绣滤镜更新(&amp;R)
* &amp;lbrack；Content&amp;rbrack；绘画筛选器更新
* &amp;lbrack；Content&amp;rbrack； Delighter滤镜更新

**已修复：**

* &amp;lbrack；Content&amp;rbrack；水滤器正在Specular/光泽度工作流程中工作
* 在激活弹出窗口中修复灰度单选按钮
* 接受包含昏迷字符的文件
* 修复弹出窗口上的小字体问题
* 修复由于与某些NVIDIA显卡的FXAA参数冲突而导致的透明度UI问题
* 在滑块中输入值后移除字段的焦点
* 将最小的VRAM量分配给要享受此优惠的商家以减少崩溃
* 修复了调整应用程序窗口大小时窗口冻结的问题
* 修复了在评估时删除图层堆叠的崩溃

**已知问题：**

* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* 不建议使用“愉悦”阶段的快速可见性切换
* 自定义环境导入可能会变成黑色
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点

### 0.5.4-beta Nacho

*（发布日期：2019年3月26日）*

**已修复：**

* &amp;lbrack；删除飞溅图层时堆叠&amp;rbrack；崩溃
* 应用程序崩溃时&amp;lbrack；Data&amp;rbrack；资源数据库损坏
* 资源数据库损坏时，无法启动&amp;lbrack；Data&amp;rbrack；Substance Alchemist
* 导入材料时的随机崩溃

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能
* 自定义环境导入可能会变成黑色
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点
* 要保存到的默认收藏夹可以为空

### 0.5.3-beta Nacho

*（发布日期：2019年3月19日）*

**已添加：**

* 在“资源”面板中按材质名称搜索
* &amp;lbrack；UI&amp;rbrack；仿制工具带有画笔大小可视化的新UI
* &amp;lbrack；UI&amp;rbrack；选择并删除隐藏阶段
* &amp;lbrack；UI&amp;rbrack；新建文本字段UI
* &amp;lbrack；帮助&amp;rbrack；访问Substance Source、Substance share和Substance学院网站
* &amp;lbrack；Content&amp;rbrack；新的默认材料（带有生成器和贴图集）
* 用于材料更新的位图(&amp;L)；Content&amp;R
* &amp;lbrack；Content&amp;rbrack；Dirt更新
* &amp;lbrack；Content&amp;rbrack；铁锈更新
* 标记；内容标记；新建浮雕滤镜(&amp;R)
* 标记；内容标记；新建刺绣滤镜(&amp;R)
* &amp;lbrack；Content&amp;rbrack；新侵蚀滤镜
* &amp;lbrack；Content&amp;rbrack；新砾石生成器
* &amp;lbrack；Content&amp;rbrack；新绘画过滤器
* &amp;lbrack；Content&amp;rbrack；新建镶板图案滤镜
* &amp;lbrack；Content&amp;rbrack；新建路面图案滤镜
* &amp;lbrack；Content&amp;rbrack；新建穿孔过滤器
* &amp;lbrack；Content&amp;rbrack；新建飞溅滤镜
* 包装；内容&amp;包装；新纺织品磨损过滤器(&amp;R)
* &amp;lbrack；Content&amp;rbrack；新建变换过滤器

**已修复：**

* 视口&amp;lbrack；拼贴为x2的Sphere网格(&amp;L)
* 加载您自己的视口时崩溃(&amp;l)
* &amp;lbrack；视口&amp;rbrack；环境图现在也使用曝光值
* &amp;lbrack；视口&amp;rbrack； F快捷键不重置相机角度
* &amp;lbrack；导出&amp;rbrack； SBS导出适用于最新的Substance Designer2018.3.3
* &amp;lbrack；导出&amp;rbrack； SBSAR导出遵循与材料相同的准则
* 可拖动&amp;lbrack；UI&amp;rbrack；滚动条
* 文件夹和文件路径支持特殊字符
* 保存材质时重新生成缩略图

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能
* 自定义环境导入可能会变成黑色
* Tif图像未显示在“图像导入”图层的“属性”面板中
* 在滑块中键入特定值时，可以忽略昏迷或点
* 要保存到的默认收藏夹可以为空

### 0.5.2-beta Nacho

*（发布日期：2019年3月7日）*

**已添加：**

* 高分辨率GPU的检测与使用

**已修复：**

* 旋转参数具有适当的滑块构件
* 在拖放材料时修复蓝色线条可见性
* 修复将材料放到第一个图层下方时的材料混合问题
* 仅在未设置自定义图像路径的情况下才插入图像输入

**已知问题：**

* 文件路径中的特殊字符会导致无法保存材料
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能
* 加载您自己的环境时崩溃

### 0.5.1-beta Nacho

*（发布日期：2019年3月4日）*

**已修复：**

* 修复崩溃报告、错误报告和许可证弹出窗口

**已知问题：**

* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能
* 加载您自己的环境时崩溃

### 0.5.0-beta Nacho

*（发布日期：2019年2月28日）*

**已添加：**

* 打包；图层堆叠&amp;rbrack；图层重新排序(&amp;l)
* 打包；图层堆叠&amp;rbrack；删除隐藏图层(&amp;L)
* &amp;lbrack；图层堆叠&amp;rbrack；直接在您选择的位置导入材料
* &amp;lbrack；图层堆叠&amp;rbrack；材料输入作为新的过滤器参数类型
* &amp;lbrack；性能&amp;rbrack；Substance 引擎预算是动态的，可获得更好的性能
* &amp;lbrack；性能更好&amp;rbrack；更出色的OpenGL性能，特别是在MacOS上
* &amp;lbrack；Data&amp;rbrack；新版本发布后数据升级速度更快
* &amp;lbrack；Content&amp;rbrack；可在Windows 7和Windows 8上使用AI Delighter
* RTX GPU上提供的&amp;lbrack；Content&amp;rbrack； AI Delighter

**已修复：**

* 在退出应用程序时修复可能的崩溃
* 导出大型收藏夹时，导出弹出窗口打开速度更快

**已知问题：**

* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能
* 加载您自己的环境时崩溃

### 0.4.0-Beta松糕

*（发布日期：2019年1月17日）*

**已添加：**

* &amp;lbrack；导出收藏集的Substance归档(sbsar)导出
* 导出&amp;lbrack；导出收藏集的Substance文件(sbs)(&amp;L)
* &amp;lbrack；导出&amp;rbrack；导出队列在“导出”面板中可见
* &amp;lbrack；Export&amp;rbrack；导出前命名收藏夹或材料
* 按Ctrl+Shift+S将&amp;lbrack；Data&amp;rbrack；另存为材料
* 按Ctrl+S保存材料(&amp;L)；Data&amp;R
* &amp;lbrack；Data&amp;rbrack；集合和材料跨版本兼容
* &amp;lbrack；Data&amp;rbrack；使用最新滤镜更新材质图层栈栈
* &amp;lbrack；Data&amp;rbrack；导入的自定义过滤器的热重装
* &amp;lbrack；UI&amp;rbrack；计算时视口中的视觉反馈
* &amp;lbrack；UI&amp;rbrack；新建按钮样式
* &amp;lbrack；UI&amp;rbrack；保存弹出窗口显示活动收藏夹的名称
* &amp;lbrack；UI&amp;rbrack；修改图像的源图像导入图层
* 现在支持&amp;lbrack；Content&amp;rbrack；自定义用法
* 图像输入参数中支持更多图像格式(&amp;L)
* &amp;lbrack；Content&amp;rbrack；新的拼贴滤镜名为Make It Tile Advanced
* &amp;lbrack；Content&amp;rbrack；水滤镜的更新

**已修复：**

* “位图到材质”处理Specular/光泽度工作流程

**已知问题：**

* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* RTX GPU卡不支持Delighter
* Delighter阶段的快速可见性切换会影响性能

### 0.3.1-Beta版千层面

*（发布日期：2018年12月17日）*

**已修复：**

* 使用10种提取的崩溃生成颜色变化
* 使用刚刚保存的崩溃生成颜色变化
* Substance Alchemist版本更新弹出窗口上的链接不正确

**已知问题：**

* “将位图转换为材料”无法处理Specular/粗糙度工作流
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能

### 0.3.0-beta版千层面

*（发布日期：2018年12月12日）*

**已添加：**

* &amp;lbrack；导出&amp;rbrack；新建导出弹出窗口
* &amp;lbrack；导出&amp;rbrack；导出整个集合
* &amp;lbrack；导出&amp;rbrack；以您选择的格式导出位图
* &amp;lbrack；导出&amp;rbrack；以您选择的分辨率导出位图
* &amp;lbrack；Export&amp;rbrack；仅导出您选择的通道
* &amp;lbrack；Export&amp;rbrack；预览导出的估计大小
* &amp;lbrack；导出&amp;rbrack；导出前预览磁盘上的可用大小
* &amp;lbrack；UX&amp;rbrack；集合上的操作可使用右键单击访问
* &amp;lbrack；UX&amp;rbrack；允许在Inspire中取消设置图像或资源
* 最大程度地启动&amp;lbrack；UX&amp;rbrack；Substance Alchemist
* &amp;lbrack；Assets&amp;rbrack；保存材料的新方式，以便在下一个版本中保持这些文档的持久性
* &amp;lbrack；帮助&amp;rbrack；通过帮助菜单访问联机文档
* &amp;lbrack；Performance&amp;rbrack；在使用Substance Alchemist创建的复杂材料上实现更快的颜色变化
* &amp;lbrack；Performance&amp;rbrack；减少切换实验室时的内存泄漏
* &amp;lbrack；Content&amp;rbrack；缩放检查器用于诊断材料的物理尺寸
* &amp;lbrack；Content&amp;rbrack；更新意大利威尼斯马赛克图块材料
* &amp;lbrack；Content&amp;rbrack；更新苔藓飞溅

**已修复：**

* 存储材料时不再使用默认名称
* 保存材料并重新打开Substance Alchemist后，过滤器参数丢失
* &amp;lbrack；Content&amp;rbrack；为AO和弯曲混合从底部和从顶部逻辑修复

**已知问题：**

* 使用早期版本创建的材料在新版本中不可用。
* “将位图转换为材料”无法处理Specular/粗糙度工作流
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能

### 0.2.0-beta奇异果

*（发布日期：2018年11月9日）*

**已添加：**

* 查看器设置从一个会话保存到另一个会话
* 将材料设置从一个会话保存到另一个会话
* 快速加载“属性”面板
* &amp;lbrack；Log&amp;rbrack；通过帮助菜单导出日志文件
* 打包；UI打包；新建滑块样式(&amp;L)
* 合并&amp;lbrack；UI&amp;rbrack；预设和调整面板(&amp;R)
* 打包；UI&amp;rbrack；新建缩略图样式(&amp;L)
* 可直接在视口中访问的位移、拼贴和阴影设置
* &amp;lbrack；Content&amp;rbrack；新的默认材料
* &amp;lbrack；Content&amp;rbrack；苔藓飞溅更新
* &amp;lbrack；Framework&amp;rbrack；更新Substance 引擎框架

**已修复：**

* 通过切换实验室删除您的图层堆叠已修复
* 视口中显示的加载时间值正确
* 材料工作流的默认声道已正确初始化
* 禁用自定义网格导入
* 位图导出
* &amp;lbrack；MacOS&amp;rbrack；关闭Substance Alchemist可能需要“强制退出”

**已知问题：**

* 使用早期版本创建的材料在新版本中不可用。
* 不建议在一个材料中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）的Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能

### 0.1.1-beta卡纸

*（发布日期：2018年10月24日）*

**已添加：**

* BaseColor Delighter现已推出
* 通过“帮助”菜单访问Substance Alchemist信息
* 当有新版本的Substance Alchemist可用时获取通知
* 控制台在Windows上不再可见
* 新建缩略图样式
* 可以在全屏模式下设置&amp;lbrack；MacOS&amp;rbrack；Substance Alchemist
* &amp;lbrack；Filter&amp;rbrack；导入自定义蒙版以管理两个材料之间的混合
* 标记；过滤器&amp;标记；控制苔藓缩放(&amp;R)
* &amp;lbrack；Filter&amp;rbrack；克隆修补程序更新

**已修复：**

* 在参数列表中的图像输入中添加图像将更新输出
* “导入自定滤镜”不会添加黑色的环境遮蔽和黑色的不透明度

**已知问题：**

* 使用早期版本创建的素材在新版本中不可用。
* &amp;lbrack；MacOS&amp;rbrack；关闭Substance Alchemist可能需要“强制退出”
* 不建议在一个素材中使用多个喜悦
* 使用较旧的NVIDIA驱动程序（低于400.x）时Delighter崩溃
* Delighter阶段的快速可见性切换会影响性能
* 材料导出可以崩溃

### 0.1.0-beta版冰淇淋

*（发布日期：2018年10月17日）*

**已添加：**

* 具有4种混合类型的混合（Height混合、示例混合、弯曲混合、AO混合）
* 引入缓存机制以优化图层堆叠重新计算
* 如果视口中有显示，则在Inspire中自动选择材料
* “材料设置”面板中的“普通格式”中心
* 裁剪和拼贴Widget控件（–90xB0，+90xB0，绘制正方形……） 清理
* 新建Snow过滤器

**已修复：**

* 面板用户界面清理
* 调整窗口和面板大小时视口闪烁
* 保存时未重新计算图层堆叠
* 在界面中命名的资源使用标签而不是图形名

**已知问题：**

* 通过快速切换图层可见性而拉长的光照
* 焦点重置相机角度
