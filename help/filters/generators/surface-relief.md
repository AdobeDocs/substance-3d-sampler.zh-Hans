---
helpx_url: "https://helpx.adobe.com/substance-3d-sampler/filters/generators/surface-relief.html"
breadcrumb-title: ''
description: 使用Substance 3D Sampler中的表面浮雕生成器，在素材中创建浮雕和浮雕表面图案。
helpx_creative_field: ""
helpx_description: Sampler > Filters > Generators > Surface Relief
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 表面浮雕
user-guide-description: ''
user-guide-title: ''
source-git-commit: 55277f7a92e97bf530dd2a2edf4e16c88bb57793
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# 表面浮雕

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

![](../../assets/s-surfacerelief-18-n-d.png)

**英寸：**&#x200B;生成器

</td>
<td width="58.30%" style="border: 0;" valign="top">

## 描述

使用“表面浮雕”滤镜为材质添加杂色。 这有助于分解大型形状或增加视觉趣味。

</td>
</tr>
</table>

## 参数

<b>基本参数</b>

* <b>随机植入</b>：\
  此过滤器中所有其他随机参数所基于的随机植入。
* <b>强度</b>： 0-1\
  更改噪声的振幅
* <b>模糊强度</b>： 0-1\
  应用于杂色的模糊强度
* <b>表面瑕疵</b>：图像/画笔/纹理生成器\
  使用图像或纹理生成器作为表面瑕疵。

<b>噪声参数</b>

* <b>夹具</b>： 0-1\
  将噪声固定在一定范围内
* <b>对比度</b>： 0-1\
  修改杂色的对比度
* <b>反转</b>：切换\
  反转噪点的Height图

<b>转换</b>

* <b>拼贴</b>： 1-16\
  与<b>基本参数>缩放</b>不同，<b>拼贴</b>管理杂色的实例数。
* <b>镜像</b>：\
  沿一个或两个轴镜像噪声
* <b>偏移</b>：\
  重新定位X轴和Y轴中的噪声
* <b>旋转</b>：\
  旋转噪点。 旋转角度将捕捉以确保仍然可以拼贴。

<b>蒙版</b>

* <b>使用自定义蒙版</b>：切换\
  启用以查看自定义蒙版控件：
  * <b>蒙版</b>：图像/画笔/纹理生成器\
    导入图像以用作蒙版，或使用画笔直接在<b>2D视图</b>中绘画
  * <b>自定义蒙版 — 模糊</b>： 0-1\
    模糊蒙版
  * <b>自定义蒙版 — 反转</b>：切换

<b>高级参数</b>

* <b>Height强度</b>： 0-1\
  控制杂色高光图与基础材质高光图的混合
* <b>Height — 替换基数</b>：切换\
  切换是否替换基本Height
* <b>正常强度</b>： 0-1\
  调整噪点法线图的强度
* <b>正常 — 替换基数</b>：切换\
  切换是否替换基础法线图
* <b>法向 — 方向</b>：\
  修改用于常规生成的轴
* <b>正常 — 旋转方向</b>
* <b>环境遮蔽 — 强度</b>
* <b>环境遮蔽- Radius</b>
