---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/pipeline-and-integrations/hp-z-captis-support/your-first-capture-step-by-step.html"
breadcrumb-title: ''
description: 通过分步说明，了解如何在Substance 3D Sampler中使用HP Z Captis执行您的第一个3D 捕捉。
helpx_creative_field: ""
helpx_description: Substance 3D Sampler
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 您的第一个分步拍摄
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '1267'
ht-degree: 0%

---


# 启动Sampler并打开HP Z Captis

启动Sampler并将HP Z Captis设备插入计算机后，单击左栏中的Captis/cone图标。

如果您未在UI中看到HP Z Captis ，请参阅常见问题解答。

![在Sampler中单击“加号”图标和HP Z Captis以启动设备](../../assets/5_1.png)

单击HP Z Captis后，将打开一个包含3个选项的专用窗口：

1. <b>浏览内容</b>：它将打开您的文件资源管理器，以浏览HP Z Captis设备的本地存储。
1. <b>开始扫描</b>：它将初始化HP Z Captis设备并启动捕获流。
1. <b>关闭</b>：它将关闭设备并关闭窗口。

![](../../assets/captis-captis-welcome-window.png)

## 关闭HP Z Captis窗口

如果关闭HP Z Captis窗口，系统将询问您是要<b>继续此过程</b>还是<b>中止</b>。

如果选择“继续”，设备将在当前步骤结束时离线继续执行其当前任务并暂停。 您可以稍后重新连接Sampler以继续捕获会话的下一个步骤。

![](../../assets/captis-abort-capture.png)

## 预览步骤

Sampler将初始化HP Z Captis设备的预览。 建议<b>在初始化视图时</b>不要与该视图交互。

在此新更新中，有两种模式：自动和手动。

### 常规设置

#### 自动模式

![Captis自动模式](../../../help/assets/sampler_captis-default-interface.png)

您现在可以一键启动捕捉：Sampler将：

* 定义默认名称，
* 使用背光自动定义目标区域(ROI)/裁切区域，
* 将重点放在全部ROI上，以及
* 将强度设置更改为适合您的素材的强度设置。

如果您之前进行过捕捉，则所选的材质类别、输出和捕捉分辨率将与您之前的捕捉相同。

#### 手动模式

![Substance 3D Sampler手动模式下的Captis工作流程](../../../help/assets/sampler_captis-manual-mode.png)

您也可以选择手动定义某些设置：

*项目名称*

您可以定义捕捉的项目名称，并定义要检索的输出类型。

*输出*

* 默认情况下，只存储材质PBR通道（基色、正常、Height和不透明度）。\
  您可以在LDR（低动态范围）和HDR(高动态范围)之间选择输出类型。


*捕捉分辨率*

* 239 px/in - 94 px/cm（预览：较低质量，更快的扫描）
* px/in - 142 px/cm（默认：高质量，在大多数工作流程中易于管理 — 相当于30x30cm捕捉的4k）
* 718px/in - 284 px/cm（全分辨率 — 相当于8k，适用于30x30cm拍摄）

![在Captis和Sampler工作流程中捕捉分辨率](../../../help/assets/sampler_captis-capture-resolution-6.0-1.png)
注意：Sampler中将仅加载PBR通道。\
可以在首选项中修改存储所用的默认文件夹捕获。


<b>材质类别</b>

将此项设置为要扫描的素材类型，以便生成微调到特定素材的地图。\
选择的默认类别是“结构”。 这有助于优化粗糙度通道的结果。

如果您要扫描的内容包含多种类型的材料，请选择最大材料的类别。

<b>裁剪</b>

裁剪可以自动完成，也可以手动完成。

![物理尺寸和松饼大小之间的感兴趣区域的潜在作物](../../assets/captis-51-crop.png)

自动裁剪将使用背光来定义材料的轮廓，并在其周围放置目标区域(ROI)。 它不适用于同时数字化多个材料样品，或当材料非常透明时。
在这种情况下，可以通过在预览中拖动裁切构件的角点，或通过设置定义的分辨率或物理尺寸来定义ROI。

<b>相机设置</b>

* 强度：调整相机曝光度。\
  单击“自动”将使用ROI的中心来定义材料的最佳强度。

* 焦点：它可以调整相机的焦点。\
  单击“Auto（自动）”将使用完整的ROI定义理想的焦点。
  这种新的聚焦算法，不再聚焦在单个点上，使聚焦在数字化材料上更加一致，从而产生更高质量的扫描，更易于平铺。

如果您愿意，可以手动设置这两个选项。

<b>其他设置</b>

其他类型的设置<b>只需在</b>时修改：颜色和对齐校准。

![在Substance 3D Sampler中校准HP Z Captis](../../../help/assets/sampler_captis-calibration.png)

* 颜色校准

借助HP Z Captis技术领域校准基准颜色图的颜色。 \
这将使最终材料的颜色与您在HP Z Captis托盘中添加的样品完全相同。\
带有色板的技术区域被自动检测并用于校准。 它们必须放置在样本每侧的特定空间中。

这仅在Studio模式下可用。 请确保在进行颜色校准之前进行聚焦。

必须<b>每隔几个月</b>进行此校准。 无需在每次扫描或每次使用设备时都执行此操作。

* 对齐校准

必须在<b>第一次设置设备</b>时</b>完成此对齐<b>，每次物理移动设备时，然后每两个月移动一次。 <b>无需</b>为每个捕获</b>执行此过程<b>。

请确保在对齐校准之前进行对焦。

若要进行对齐，请<b>将包含清晰锐利信息的内容（例如，一张包含印刷文本的纸）放在拍摄空间的中心</b>，关闭抽屉，然后单击对齐按钮。 完成此操作后，您可以确保一切到位，在扫描空间每侧都放置技术区域，将材料放在中心，必要时使用HP Z Captis设备提供的磁铁将其固定，然后您就可以开始扫描材料了。

完成设置后： <b>开始扫描</b>。


## 捕获、处理和复制步骤

扫描开始后，预览将显示该过程中拍摄的照片。

加工部分分为三部分：

* <b>拍摄</b>：拍摄所有必需的照片

* <b>处理</b>：处理照片以生成PBR通道（基色、正常、Height、不透明度）

* <b>正在复制</b>：正在将结果从HP Z Captis设备复制到您的计算机

在捕获和处理元数据时，您可以添加元数据（与您将在Sampler“元数据”面板中找到的元数据相同）。

![捕获步骤](../../../help/assets/sampler_captis-capturing.png)

在处理过程中，您将看到结果按拼贴构建。

## 摘要步骤

![使用Sampler和Captis数字化过程中的摘要步骤](../../../help/assets/sampler_captis-summary.png)

在此步骤中，您可以查看扫描结果。 此时会显示所有已创建的通道（在资源管理器模式中，不会创建不透明度，因为资源管理器环没有背景光）。

您可以选择将素材发送到Sampler，将其添加到您的项目并开始处理。
您也可以直接开始新的捕捉，而无需将其添加到项目中。
在这两种情况下，您都可以在计算机上的等效文件夹中找到扫描地图： C:\Users\username\Documents\Adobe\Adobe Substance 3D Sampler\Captis\Material

## 材质版本

退出HP Z Captis窗口后，通道（基色、正常、Height、粗糙度和不透明度，如相关）将作为图层添加到“图层”面板中。

![替代文本](../../../help/assets/sampler_captis-imported-material.png)


使用Sampler滤镜（色调均化、透视裁剪、拼贴……）处理和清理您的材质。

完成后，您可以：

* 保存您的Sampler项目：文件>另存为…… (Ctrl + S)

* 导出您的材料：文件>导出…… (Ctrl + E)

