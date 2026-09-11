---
helpx_url: "https://helpx.adobe.com/cn/substance-3d-sampler/technical-support/configuration/update-checker.html"
breadcrumb-title: ''
description: 了解如何使用Substance 3D Sampler中的更新检查器及时了解新版本和发行说明。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Configuration > Update Checker
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 更新检查程序
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# 更新检查程序

“更新”窗口指示是否有新版本的Substance Alchemist可用，并显示最新的[发行说明](../../release-notes/release-notes.md)。

如果有新版本可供下载，此窗口将在Substance Alchemist启动期间自动出现。

可以使用以下方法避免在启动期间显示此窗口：

* 使用窗口中的“直到下一个版本时再提醒我”设置可暂时跳过窗口显示，直到下一个版本为止。
* 禁用“编辑”>“首选项”>“检查更新”中的“**检查更新**”设置
* 使用命令行&#x200B;**—skip-version-check**&#x200B;它将不会检查Substance Alchemist启动时是否有新版本的应用程序可用
* 使用环境变量&#x200B;**SUBSTANCE\_ALCHEMIST\_SKIP\_CHECK\_FOR\_UPDATES**:Value 0或1 （1 =禁用更新检查）

>[!NOTE]
>
> 自Substance Alchemist2020.1 (2.1)以来受支持
