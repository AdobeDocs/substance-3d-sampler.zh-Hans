---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/features-and-workflows/texture-import.html"
breadcrumb-title: ''
description: 了解如何将纹理导入Substance 3D Sampler以在您的材质创建工作流程中使用现有图像文件。
helpx_creative_field: ""
helpx_description: Sampler > Features and workflows > Texture Import
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 纹理导入
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0f989901713dd30f8f936de2445caf5dc70a9225
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 5%

---


# 纹理导入

![](../assets/Capture-decran-2025-02-19-162128.png.img.png)

**纹理导入**&#x200B;模板将加载多个图像，并根据其文件名自动将其连接到正确的输出通道。

通道匹配基于下面详述的特定命名约定。 如果存在重复项目或不匹配的纹理，则将在界面中按此方式标记图像。

## OpenPBR

Sampler会将带有以下OpenPBR标识符的文件与素材中的等效通道进行匹配。

>[!NOTE]
>
> Height通道标识符与用于ASM的通道标识符相同。


| OpenPBR标识符 | SBSAR用法 |
| --- | --- |
| base_weight | baseWeight |
| base_color | 基色 |
| base_metalness | 金属性/金属性 |
| base_spream_roughness | baseSpreamRoughness |
| Specular_权重 | 镜面粗细 |
| Specular | specularColor |
| Specular_粗糙度 | 镜面粗糙度/粗糙度 |
| Specular_粗糙度_各向异性 | specularRoughnessInspecialistic/inspecialisticLevel |
| Specular(_i) | specularIOR/IOR |
| transmission_weight | transmissionWeight |
| transmission_color | transmissionColor/assabilityColor |
| 传输深度 | transmissionDepth/absorptionDistance |
| 传输散点 | transmissionScatter |
| 传输各向异性 | transmissionScatterInspeciality |
| transmission_dispersion_scale | transmissionDispersionScale |
| transmission_dispersion_abbe_number | transmissionDispersionAbbeNumber |
| subsurface_weight | subsurfaceWeight/transparency |
| subsurface_color | subsurfaceColor/scatteringColor |
| subsurface_radius | subsurfaceRadius/scatteringDistance |
| subsurface_radius_scale | subsurfaceRadiusScale/scatteringDistanceScale |
| subsurface_散点_各向异性 | subsurfaceScatterInspecirospeciality |
| coat_weight | 皮毛粗细/皮毛不透明度 |
| coat_color | coatColor |
| 涂层_粗糙度 | 皮毛粗糙度 |
| 涂层_粗糙度_各向异性 | 涂层粗糙度各向异性 |
| coat_ior | coatIOR |
| 涂层_变暗 | 皮毛变暗 |
| fuzz_weight | fuzzWeight/sheenOpacity |
| fuzz_color | fuzzColor/sheenColor |
| fuzz_粗糙度 | fuzzRoughness/sheenRoughness |
| emission_weight | emissionWeight |
| 发射_亮度 | 发射亮度 |
| 发射颜色 | 发射颜色/发射颜色 |
| 薄膜_重量 | ThinFilmWeight |
| 薄膜Thickness | ThinFilmThickness |
| 薄膜_或 | ThinFilmIOR |
| 不透明度 | 不透明度 |
| 薄壁 | 薄壁 |
| 正常 | 正常 |
| 切线 | 切线 |
| 涂层_正常 | coatNormal |
| coat_tangent | coatTangent |

## Adobe 标准材质

下面列出了每个通道支持的文件命名约定：

| **频道** | **Adobe标准素材** |
| --- | --- |
| **环境遮蔽** | <ul><li>环境包容</li><li>ao</li><li>遮蔽</li><li>ambient_occlusion</li></ul> |
| **基色** | <ul><li>基色</li><li>颜色</li><li>反照率</li><li>base_color</li><li>基底</li><li>列</li><li>颜色</li><li>base_color</li><li>基色</li></ul> |
| **扩散** | <ul><li>扩散</li><li>差异</li></ul> |
| **具发射性** | <ul><li>自发光</li></ul> |
| **光泽度** | <ul><li>光泽度</li><li>光亮</li></ul> |
| **Height** | <ul><li>Height</li><li>heightmap</li><li>位移</li><li>disp</li></ul> |
| **金属质感** | <ul><li>金属</li><li>mtl</li><li>金属性</li></ul> |
| **正常** | <ul><li>正常</li><li>nrm</li></ul> |
| **不透明度** | <ul><li>不透明度</li><li>alpha</li></ul> |
| **粗糙度** | <ul><li>粗糙度</li><li>粗糙</li></ul> |
| **Specular** | <ul><li>Specular</li><li>规范</li></ul> |
| **Specular level** | <ul><li>specularlevel</li><li>Specular级别</li></ul> |

