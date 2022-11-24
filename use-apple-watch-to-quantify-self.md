---
title: "使用 Apple Watch 运动和量化自我"
date: 2022-11-21T16:14:20+08:00
draft: false
categories:
  - "Blog"
tags:
  - "Apple Watch"
  - "Quantified Self"
  - "量化自我"
  - "智能设备"
---

我是在读了耐克创始人菲尔·奈特的亲笔自传《鞋狗》后开始认真跑步的。

曾经用过 RunKeeper 记录单车骑行和跑步，再后来还用过 Keep，悦跑圈，还有咕咚。有了 Apple Watch，我会直接用 Apple Watch 上的体能训练直接开始，然后用 iPhone 上的【健康】来查看体能训练详情。与 Keep 和 悦跑圈这些三方应用相比，这些体能训练的详细数据都会记录在苹果系统的 HealthKit 中，这样的数据可以被其它应用共享和使用，我们自己还可以继续分享数据。

慢慢的，我也就不再使用三方应用，一方面是数据不够开发，另一方面是这些应用掺杂了很多我基本不会用的功能，比如社区，商城等。现在，我基于苹果的 HealthKit 给自己开发了量化自我的应用 - 集合。



## 跑步跟踪

我的跑步三件套就是 Apple Watch、AirPods Pro 和 iPhone，有时候就只带 Apple Watch。Apple Watch 的运动圆环让我相信坚持的力量，坚持的同时积累了不少数据和奖章。搭配 Workout, AutoSleeep, Tyme 2 基本能把我的运动，睡眠，时间进行量化，看着自己获得的成就，赢到的奖章，让我更加相信坚持的力量。

![CleanShot 2022-11-13 at 23.36.25@2x.png](https://cdn.nlark.com/yuque/0/2022/png/177619/1668353805342-0c3a1064-8651-4a60-9668-bc6775f08529.png#averageHue=%2351512e&clientId=u9a2bc7fb-39e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=806&id=uf183ede0&margin=%5Bobject%20Object%5D&name=CleanShot%202022-11-13%20at%2023.36.25%402x.png&originHeight=1612&originWidth=1328&originalType=binary&ratio=1&rotation=0&showTitle=false&size=2093032&status=done&style=none&taskId=uf30b82b3-3ae6-4d39-aa6a-742fd61ac90&title=&width=664)



## 量化自我

没有记录便没有发生，没有量化便无法优化。于是我给自己做了应用《集合》，定位于一款自我量化工具类应用。自我量化，看见成长。通过数据和图表的形式量化自我，主要由数据和图表模块组成。

![image.png](https://cdn.nlark.com/yuque/0/2022/png/177619/1668261094631-187a0073-41f8-4d84-bb34-8f915ef7548c.png#averageHue=%232e7f67&clientId=u179ed617-74d6-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=346&id=RsQhH&margin=%5Bobject%20Object%5D&name=image.png&originHeight=692&originWidth=1324&originalType=binary&ratio=1&rotation=0&showTitle=false&size=863741&status=done&style=none&taskId=uea9f81db-4be4-44a2-b536-764a0fc8447&title=&width=662)



### 数据模块

数据模块，将某一类型的数据整合到一起，列表显示。

![image.png](https://cdn.nlark.com/yuque/0/2022/png/177619/1668261101687-0b8f4211-e035-4460-9503-82be0115b06f.png#averageHue=%2323886a&clientId=u179ed617-74d6-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=346&id=m7glt&margin=%5Bobject%20Object%5D&name=image.png&originHeight=692&originWidth=1328&originalType=binary&ratio=1&rotation=0&showTitle=false&size=611272&status=done&style=none&taskId=u70287115-6140-44e4-821c-df79076464a&title=&width=664)

- 体能训练，自动读取苹果健身中的训练数据，显示训练时间、详情、步频、步幅、心率等数据；
- 时间管理，自动读取苹果健身中的训练数据和健康中的睡眠数据，自动记录训练时间和睡眠时间。另外，还可以手动记录不同种类的时间投入，分析时间都去哪了；
- 睡眠跟踪，自动读取苹果健康中的睡眠数据，整合心率数据，展示睡眠期间的心率曲线，睡眠时心率范围。
- 跑马之旅，手动记录去不同城市跑过的马拉松成绩；几年下来，你会看到已经在哪些城市跑过马拉松，成绩变化趋势。



### 图表模块

图表模块，通过图表形式展示数据，如进度条，圆环、线图、柱状图等；

![CleanShot 2022-11-13 at 14.28.16@2x.png](https://cdn.nlark.com/yuque/0/2022/png/177619/1668320923322-bace9eeb-4de0-4802-acae-c0ada93e660e.png#averageHue=%231e8566&clientId=u74f8395f-4790-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=347&id=M84ME&margin=%5Bobject%20Object%5D&name=CleanShot%202022-11-13%20at%2014.28.16%402x.png&originHeight=694&originWidth=1326&originalType=binary&ratio=1&rotation=0&showTitle=false&size=799535&status=done&style=none&taskId=u12029d11-ecef-4430-b93b-9e823774237&title=&width=663)

- 进度条，如时间进度，时间跟踪类型占比；
- 圆环，可以跟踪目标进度，如运动时间，目标跑量；
- 线图，曲线表示数据变化，如心率曲线对应心率变化；
- 柱状图，柱状表示数据变化，如每周跑量，睡眠时长，骑行里程；



更多的数据记录和图表显示会通过版本更新支持。。。

建议你使用 iPhone 的同时，最好全天佩戴 Apple Watch，使用 Apple Watch 上的【体能训练】开始运动。这样可以保证有全面的健康数据，如心率、站立时间、心率、运动等信息。



## 下载使用

如果你愿意体验使用，欢迎点击 [进入 App Store 下载](https://t.cmcn.me/app)。

使用【集合】的过程中，如果你有任何好的建议或想法，欢迎在应用内联系我们；

如果你恰好是设计师，对这个应用和量化自我方向感兴趣，也欢迎留下联系方式，交流合作都可以。

