---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/interface/panels/channel-settings-panel.html"
breadcrumb-title: ''
description: 了解如何使用Substance 3D Sampler中的“声道设置”面板来管理材料声道和控制声道可见性。
helpx_creative_field: ""
helpx_description: Sampler > Interface > Panels > Channel Settings panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: “通道设置”面板
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 1%

---


# “通道设置”面板

<table>
<tr style="border: 0;">
<td style="border: 0; width: 30%" valign="top">


**声道设置**&#x200B;面板控制为当前材料计算的声道列表。 您可以管理频道可见性、在材料中添加或删除频道，或者更改正在使用的材质模型。

</td>
<td style="border: 0;" valign="top">

![通道设置面板。](../../assets/6.0_ChannelSettingsPanel.png)

</td>
</tr>
</table>

## 材质模型

使用此下拉列表选择用于渲染材料的着色器框架。 **声道设置面板**&#x200B;中的选项将根据所选材质模型而更改。

更改材质模型时，需要为新模型重新计算您的图层堆叠，并且会提供不同的渠道。 Sampler会尝试最大限度地减少转换过程中的数据丢失；但是，此更改可能会导致新材质模型的外观出现细微差异。

>[!NOTE]
>
> 可以从Adobe Standard Material(ASM)更改为OpenPBR，但当前无法从OpenPBR更改为ASM。


## 材质通道

<table>
<tr style="border: 0;">
<td style="border: 0; width: 30%" valign="top">


此部分显示默认情况下基于工作流程计算的通道的列表。

您可以使用&#x200B;**“编辑列表”按钮**&#x200B;打开&#x200B;**声道选择**，并更改为您的材料计算的声道。

</td>
<td style="border: 0;" valign="top">

![突出显示了“材料声道”部分的“声道设置”面板](../../assets/6.0_ChannelSettingsPanel_MaterialChannels.png){width="200px"}

</td>
</tr>
</table>

>[!NOTE]
>
> 例如，Substance Source中的某些材料不输出不透明度或ambient occlusion声道。 即使不透明度通道被标记为“已计算”，如果Substance文件不输出，Sampler也不会生成它。

### 通道选择

“声道选择”窗口可让您在材料中添加或删除声道。

![选择Adobe Standard Material作为材质模型的频道选择窗口的屏幕截图。](../../assets/6.0_ChannelSelectionWindow.png)

若要将频道添加到您的材料，请选择一个可用频道，然后使用&#x200B;**>按钮**。
若要从您的材料中删除频道，请从**所选频道列表**&#x200B;中选择该频道，然后使用&#x200B;**&lt;**按钮。
您可以使用**≫按钮**&#x200B;将所有可用声道添加到材料，或使用&#x200B;**≪按钮**&#x200B;从您的材料中删除所有声道。

您还可以使用预设来快速选择材料的声道列表。 默认情况下，Sampler包含许多预设，但您也可以创建自己的预设：

1. 将所需声道添加到材料。
1. 使用&#x200B;**另存为预设按钮**。
1. 为预设命名。

>[!NOTE]
>
>保存预设不会将预设应用于您的素材。

## 自定义通道

切换默认情况下未包含在选定工作流程中的其他通道。

<table>
<tr style="border: 0;">
<td style="border: 0; width: 30%" valign="top">

每个自定义通道都有两个可用于控制它的选项：

1. 使用“可见性”切换开关可在2D视图中显示或隐藏通道。
2. 使用&#x200B;**自动按钮**&#x200B;切换是否自动计算通道。
   * 打开后，如果堆叠中位于通道上方的层要求通道，则会计算该通道。
   * 关闭时，始终计算通道。

</td>
<td style="border: 0;" valign="top">

![突出显示了“自定义通道”部分的“通道设置”面板。](../../assets/6.0_ChannelSettingsPanel_CustomChannels.png){width="200px"}


</td>
</tr>
</table>



