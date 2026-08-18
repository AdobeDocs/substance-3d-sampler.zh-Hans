---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: 了解如何激活和管理Substance 3D Sampler的许可证，以开始使用该应用程序并访问所有功能。
helpx_creative_field: ""
helpx_description: Sampler > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 激活和许可证
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 1%

---


# 激活和许可证

此页面包含有关如何激活和管理许可证的信息，以便您可以开始使用Sampler。

## 每个应用程序类型的激活流程

激活过程取决于您购买或有权访问Sampler的位置：

| 应用程序类型 | 激活过程 |
| --- | --- |
| Creative Cloud 桌面版 | 请参阅[HelpX文档](https://helpx.adobe.com/support/substance-3d-sampler.html)中的专用页面。如果有任何问题，[Creative Cloud文档](https://helpx.adobe.com/creative-cloud/user-guide.html)可能会提供其他答案。 |
| 蒸汽 | 直接从Steam库中启动产品。 |
| Substance 3D独立 | 请参阅下述激活流程。 |

## 激活步骤

### 激活向导

![](../assets/activation-wizard.png){width="350px"}

有三种选择可用：

* **评估此产品**：旧版试用不再可用。 您可以改为在[此处](https://www.adobe.com/creativecloud/3d-augmented-reality.html)或使用Creative Cloud桌面版为每个Substance 3D应用程序开始30天试用。 每个试用都独立于其他Substance 3D应用程序，因此您可以一次试用一个应用程序或一次试用所有应用程序。
* **使用许可证文件进行激活**：在2022年9月30日之前，使用从[Substance 3D网站](https://store.substance3d.com/user)上的帐户页面下载的许可证文件(**\*.key**)激活产品。
* **使用您的帐户激活**：旧版Substance帐户无法再用于激活。 [此处提供了有关Substance帐户的更多信息](https://helpx.adobe.com/substance-3d/unlisted/faq-end-of-life-accounts.html)。

>[!WARNING]
>
> 要使用“激活向导”安装许可证文件，请确保以管理员身份运行Sampler并暂时禁用防病毒软件。

### 手动激活

可以通过将&#x200B;**license.key**&#x200B;文件放入以下文件夹来手动激活Sampler：

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Platform</th><th>Version</th><th colspan="2">路径</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>3.0</strong>或更高版本</td><td colspan="1">应用程序数据（本地）</td><td colspan="1">C:\Users\用户\[用户名]\AppData\Local\Adobe\Adobe Substance 3D Sampler</td></tr><tr><td colspan="1">应用程序数据（漫游）</td><td colspan="1">C:\Users\用户\[用户名]\AppData\Roaming\Adobe\Adobe Substance 3D Sampler</td></tr><tr><td rowspan="2">旧版</td><td colspan="1">应用程序数据（本地）</td><td colspan="1">C:\Users\[用户名]\AppData\Local\Allegorithmic\SubstanceAlchemist</td></tr><tr><td colspan="1">应用程序数据（漫游）</td><td colspan="1">C:\Users\[用户名]\AppData\Roaming\Allegorithmic\SubstanceAlchemist</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>3.0</strong>或更高版本</td><td colspan="2">/用户/[用户名]/资源库/Application Support/Adobe/Adobe Substance 3D Sampler</td></tr><tr><td colspan="1">旧版</td><td colspan="2">/用户/[用户名]/资源库/Application Support/Allegorithmic/Substance Alchemist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>3.0</strong>或更高版本</td><td colspan="2">/home/[用户名]/.local/share/Adobe/Adobe Substance 3D Sampler</td></tr><tr><td>旧版</td><td colspan="2">/home/[用户名]/.local/share/Allegorithmic/Substance Alchemist</td></tr></tbody></table>

>[!NOTE]
>
> 上述路径中的某些目录可能默认处于隐藏状态。 在文件资源管理器中手动键入路径，或者显示隐藏的文件以查看它们。

>[!NOTE]
>
> 确保该文件名为&#x200B;**license.key**，否则应用程序将无法找到它。

### 环境变量

您可以使用[环境变量](../pipeline-and-integrations/environment-variables.md)覆盖Sampler为&#x200B;**license.key**&#x200B;文件检查的位置。
