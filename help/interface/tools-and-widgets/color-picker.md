---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/interface/tools-and-widgets/color-picker.html"
breadcrumb-title: ''
description: 了解如何在Substance 3D Sampler中使用拾色器为材质、滤镜和纹理编辑选择颜色。
helpx_creative_field: ""
helpx_description: Sampler > Interface > Tools and Widgets > Color Picker
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 拾色器
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# 拾色器

每次需要选择颜色时，都会显示拾色器。

## UI概述

![](../../assets/color-picker-11.png){width="300px"}

1. **颜色方形**：使用选定的色相微调颜色的饱和度和亮度。
1. **色相滑块**：调整颜色的色相。
1. **当前/上一个**：左侧的颜色是拾色器的当前颜色。 正确的颜色是打开拾色器时的颜色 单击右侧的颜色，将当前颜色重置为原始值。
1. **十六进制输入**：您可以直接输入所需颜色的十六进制颜色代码。
1. **滴管**：启动滴管以从屏幕中选取颜色。 光标旁将出现一个气泡，用于预览将选取的颜色。
1. **滑块**：使用不同的色彩空间（RGB或HSV）微调颜色。
1. **色板**：保存颜色以快速访问它们以供将来使用。

### 滑块

#### 色彩空间

RGB（红色、绿色、蓝色）和HSV（色相、饱和度、值）是两个可用的色彩空间。

![](../../assets/rgb-hsv.jpg){width="200px"}

#### 滑块选项

![](../../assets/slider-options.jpg){width="200px"}

**显示滑块**

此选项允许您隐藏滑块以节省空间。 即使隐藏了滑块，您仍然可以修改值输入。

**浮点值**

![](../../assets/float-value.jpg){width="200px"}

切换对滑块使用浮点值还是整数值。 浮点值介于0和1之间，而整数值介于0和255之间。

**动态滑块**

切换滑块背景是否随值的更改而动态更新。 下图显示了关闭动态滑块时的滑块外观。

![](../../assets/no-dynamic-slider.jpg){width="200px"}

### 色板

当您想要保存特定颜色以在应用程序或多个项目间使用时，色板非常有用。

色板对Sampler来说是全局性的，而不是特定于每个项目。

单击“+”按钮将添加一个色板，其中当前颜色是列表中的第一个色板。

![](../../assets/swatches-2.jpg){width="200px"}

注意：您不能两次添加具有相同颜色的色板。 当您再次尝试添加时，已保存的色板将突出显示。

当鼠标悬停在色板上时，会显示一个工具提示，其中颜色值以十六进制表示。

#### 色板选项

全部删除选项。

![](../../assets/swatches-options-2.jpg){width="200px"}

右键单击色板以将其删除或替换为当前颜色。

![](../../assets/swatch-options.jpg){width="200px"}

还可以通过将色板拖放到拾色器外部来删除它。
