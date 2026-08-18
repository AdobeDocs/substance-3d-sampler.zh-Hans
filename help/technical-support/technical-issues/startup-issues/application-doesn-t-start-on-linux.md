---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/technical-support/technical-issues/startup-issues/application-doesn-t-start-on-linux.html"
breadcrumb-title: ''
description: 了解如何修复Linux上的Substance 3D Sampler启动问题，以解决应用程序启动问题和错误消息。
helpx_creative_field: ""
helpx_description: Sampler > Technical Support > Technical Issues > Startup issues > Application doesnt start on Linux
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 应用程序在Linux上无法启动
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---


# 应用程序无法在Linux上启动

应用程序无法在Linux上启动，且终端中出现以下错误消息：

```
error while loading shared libraries: libicui18n.so.50
```


这意味着库ICU （[Unicode的国际组件](http://site.icu-project.org/)）缺失或安装的版本太新。 应用程序需要版本50。

要解决此问题，请从包管理器安装版本50，或者[手动下载](http://mirror.centos.org/centos/7/os/x86_64/Packages/libicu-50.2-4.el7_7.x86_64.rpm)缺少的版本并将其安装在&#x200B;**/usr/lib64**&#x200B;中。
