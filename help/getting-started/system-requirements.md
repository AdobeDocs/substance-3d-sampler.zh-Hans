---
helpx_url: 'https://helpx.adobe.com/cn/substance-3d-sampler/getting-started/system-requirements.html'
breadcrumb-title: ''
description: 查看Substance 3D Sampler的系统要求，确保您的硬件和软件符合兼容性标准。
helpx_creative_field: ''
helpx_description: Sampler > Getting Started > System requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 系统要求
user-guide-description: ''
user-guide-title: ''
source-git-commit: cd61972eaf1567863dc8c3549a1c90c84ffee825
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---


# 支持的系统

以下是应用程序支持的硬件和系统的列表：

>[!WARNING]
>
> 已知以下Nvidia驱动程序会在运行Sampler时导致不稳定：
>
> * 610.47
>
> 我们建议避免使用这些版本 — 理想情况下，使用更新版本，或者，如果没有更新的版本，则使用以前的版本。

## Windows

|  | 最小 | 推荐 | 最佳 |
| --- | --- | --- | --- |
| **操作系统** | Windows 11（64位）23H2版 | Windows 11（64位）24H1版 | Windows 11（64位）24H2版 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada代AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **存储空间** | 具有30 GB可用空间的固态硬盘 | 具有50 GB可用空间的固态硬盘 | 具有70 GB可用空间的固态硬盘 |

### macOS

|  | 最小 | 推荐 | 最佳 |
| --- | --- | --- | --- |
| **操作系统** | macOS13 Ventura | macOS14 Sonoma | macOS26 Tahoe |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 24 GB | 32 GB | 64 GB |
| **存储空间** | 具有30 GB可用空间的固态硬盘 | 具有50 GB可用空间的固态硬盘 | 具有70 GB可用空间的固态硬盘 |

### Linux

| 企业 | 蒸汽 |
| --- | --- |
| RHEL 8 <br>RHEL 9 | Ubuntu 22.04 |

>[!NOTE]
>
> 如果您的系统满足上述系统要求，但性能仍然缓慢，则Sampler可能使用了错误的GPU。
>
> 如果使用的是NVIDIA GPU，请[按照本页中的说明更改Sampler使用的GPU](../technical-support/configuration/nvidia-driver-settings.md)。

## 一般建议

* 为了在舒适的条件下工作，我们建议使用分辨率大于1 MegaPixel且宽于1280像素的显示器。
* 许多Substance应用程序依靠OpenSSL 1.1.1来与RHEL8/9兼容。 对于具有较新OpenSSL版本的系统，您需要手动提供它。

## 不支持的配置

**Windows**

* 不支持虚拟机。
* 不支持Windows Server。

**Mac**

* 仅支持官方Apple配置。
* eGPU当前不受支持，可能存在稳定性问题。

**Linux**

* 不支持Linux上的Mesa驱动程序。

**任何平台**

* x86-64 (Intel、AMD) CPU不支持集成GPU。
* 不支持将Sampler与拦截Sampler对图形驱动程序的调用的第三方软件结合使用。 此类软件包括：
  * 后期处理喷射器，例如应用颜色分级的整形器、相机效果等……
  * 屏幕叠加，例如自定义十字线、GPU性能度量、视频流的外观……

## 最低GPU驱动程序版本

下表列出了运行无问题的应用程序所需的最低GPU驱动程序版本。 此列表可能会随着新版本的发布而发生更改。

要下载新驱动程序，请参阅： [GPU具有过时的驱动程序](https://experienceleague.adobe.com/zh-hans/docs/substance-3d-painter/using/technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers)。

| 操作系统 | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **Windows** | GeForce 551.86 Quadro/RTX 538.33 | Radeon 23.8.1 Radeon Pro / FirePro 24.q2 | 31.0.1015590 |
| **Linux** | 525.116.04或更高版本&#x200B;*或* 535.54.03或更高版本 | Radeon 23.20 Pro 23.Q3 | 不支持 |

>[!NOTE]
>
> 在&#x200B;**Mac OS**&#x200B;上，GPU驱动程序由操作系统本身提供。 更新到最新版本的操作系统以访问最新驱动程序。

## 语言

软件界面提供以下语言版本：

* English
* 德语
* Français
* 日本語
* 朝鲜语
* 中文
* 意大利语
* 葡萄牙语
* 西班牙语
