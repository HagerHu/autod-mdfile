---
title: "目标和现实的差距"
date: 2023-06-04T23:11:20+08:00
draft: false
Summary: 回顾刚过去的 5 月份，看着月初定下的目标，回顾每一天发现一个月后现实与目标之间的差距是如此之大。今年刻意培养的一个习惯就是反思总结，形成反馈循环。 “目标 - 跟踪 - 总结” 就是我给自己设定的反馈循环，希望每一周、每个月、每个季度不断的自省，最终能实现《原则》中提到的螺旋式上升。
Description: 回顾刚过去的 5 月份，看着月初定下的目标，回顾每一天发现一个月后现实与目标之间的差距是如此之大。今年刻意培养的一个习惯就是反思总结，形成反馈循环。 “目标 - 跟踪 - 总结” 就是我给自己设定的反馈循环，希望每一周、每个月、每个季度不断的自省，最终能实现《原则》中提到的螺旋式上升。
keywords: ["原则","反馈循环","目标与现实","听过的播客","精益创业","过早优化"]
categories:
  - "每周总结"
tags:
  - "反思总结"
image: "https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.07.49@2x.png"
---

![gap-between-goal-and-real](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.07.49@2x.png)

### 目标与现实的差距

周五去浙江图书馆，相比西湖图书馆、文二路博库书城，这里的桌椅高度现实更适合一些。

![review goal of may](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.59.57@2x.png)

回顾刚过去的 5 月份，看着月初定下的目标，回顾每一天发现现实与目标之间，差距是如此之大。当初定的目标，分别是新的应用推广渠道、博客显示健身训练记录、苹果公司财报阅读和继续湾区周报但分配好时间 4 个方面；到了月底，推广渠道想到了威锋社区，等级不够没有发帖权限，已经有段时间没去了；博客显示健身训练记录和苹果公司财报阅读从未开始；湾区周报虽在继续，但并没有很好的分配时间来阅读英文文章，还是会专门抽时间寻找和阅读，却有时间刷油管、B站，而且去黄山的那一周少了一起湾区周报，目前为止 4，5 月份各有一期没有发布。

每天的事情都记录和跟踪下来，这样回头看的时候就知道这段做过的事，投入的时间。也才在月底总结的时候，发现 5 月目标和显示之间的差距。当初定下 5 月目标的时候，还把「重要且有意义的事」写在了目标的最前面，算是给自己明显的提示。月初的 4 个目标也是给自己接下来一个努力的方向，可惜最终发现自己还是没有经常看看自己是否在正确的方向上。

![loop in principle](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.00.17@2x.png)

达利欧在《原则》中提到，反思 + 总结 = 进步，五步流程法不断重复，保持螺旋式上升。年度目标 -> 季度目标 -> 月度目标 -> 每周目标 -> 每天跟踪 -> 每周总结 -> 月度总结 -> 季度总结 -> 年度总结，就是我给自己的反馈循环，希望能够发现问题，改进执行，最终螺旋式上升。以前没意识到目标和现实之间的差距如此之大，而且是到了月底总结才发现与之前的目标相差甚远，如果能前 2 周总结的时候发现，能早点意识到或许这个月会过的好一点，差距不会想现在这样大。

《精益创业》中提到过的最小化可行产品，就是用最快的方式，用最少的精力完成 “开发 - 测量 - 认知” 的反馈循环，避免浪费资源和精力。对于反思总结也是一样，就是要加快 “目标 - 跟踪 - 总结” 这个反馈循环，更快意识到偏离了方向，也就能更快从偏离的方向上纠正，缩小目标和现实的差距，久而久之也就会进入螺旋上升的趋势。

### 从分享的播客开始

社交上会分享跑步听到的播客，自己也在听一些关注的播客。2022 年度总结的时候，总结了 读过的图书，看过的电影，买过的设备等方面。今年想着给自己做的集合应用，也是围绕记录和量化来做，想到了记录听过的播客。

跑步的时候偶尔会听播客，听到好听的也会用「跑步电台」分享听到的播客。分享一方面是为了记录自己听过的播客和感悟，另一方面也是将自己觉得好的东西分享出来。

想到可以通过播客分享的链接，识别播客信息可以做为自己的任务，听完之后记录为听过的播客。于是开始寻找和研究可行方案，先复制 Podcast 分享链接看具体格式，通过搜索发现 iTunes Lookup API 可以使用播客 ID 获取播客和剧集信息，分享的链接中就带上了 Podcast 的 id (id1475113228) 和 episode 的 trackId (i=1000548957645)，再通过 trackId 检查就可以找到 Podcast 分享链接的 Episode 信息了。

```text
// Podcast 的分享链接
https://podcasts.apple.com/us/podcast/%E4%B8%89%E4%BA%94%E7%8E%AF/id1475113228
// Podcast 某 Episode 的分享链接
https://podcasts.apple.com/us/podcast/%E4%B8%89%E4%BA%94%E7%8E%AF/id1475113228?i=1000548957645

// iTunes Lookup API 通过 id 搜索播客信息
https://itunes.apple.com/lookup?id=1000548957645&entity=podcast

// iTunes Lookup API 通过 id 和 podcastEpisode 获取播客 Episodes 列表
https://itunes.apple.com/lookup?id=1000548957645&country=US&media=podcast&entity=podcastEpisode&limit=100
```

接下来，我用 Goland 配合 gin 开发了一个接口服务，传入 Podcast 分享的链接，识别到播客信息和订阅链接，也可以获取播客所有的 Episodes。这些全部搞好差不多用了周六半天时间。

![api service to get rss feed](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2016.47.25@2x.png)

后来发现有个专门站点 [Get RSS Feed](https://cmcn.me/link?target=https://getrssfeed.com/) 也是做这个功能， 而且还支持从 Google Podcast，SoundCloud，Blog 和 Site 中获取。知道了 Get RSS Feed 是 [Podcast Addict](https://cmcn.me/link?target=https://podcastaddict.com/) 下的一个功能, 作者主要靠广告获得收入，但广告收入持续下滑；后来开通了 一次性付费 支持，但也并不可持续；又增加了 订阅功能 来希望能有个稳定的收入，想要了解详情可以[点击阅读](https://podcastaddict.com/premium)这篇文章。

![GetRSSFeed stats](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2016.49.27@2x.png)

![Podcast Addict stats](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2016.50.56@2x.png)

顺手看了一下这两个站点的流量，Podcast Addict 流量还挺高。顺手看一下站点流量，也表示现我开始有些增长的意识了😊。

### 依然还在浪费资源

这周总结回顾的时候发现，本周依然浪费了不少时间和精力。

![riding just for fun](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2021.08.23@2x.png)

偶然的机会，看到 B站 UP 主 [我就骑着玩](https://cmcn.me/link?target=https://space.bilibili.com/1493959577) 的旅行视频，看过几个之后才知道 UP 主是个退役女兵，是不是文艺兵不知道，但视频的景色和配乐真的很棒，如果你也喜欢看这类视频推荐给你。

之前看过不少摩旅去西藏都是很好的摩托车和装备，「我就是骑着玩」则是骑着最快也就 50公里的入门级小踏板 铃木125  上路了，可见，想出去看外面的世界的人很多，但关键还是有多想要去看看的心。除了 我就是骑着玩 的小踏板摩旅，还刷了 [袁学周](https://space.bilibili.com/295041700) 公路车比赛的视频，一不注意就过去了近两小时，时间就这么悄悄的溜走了。看着 B 站这一周观看的历史记录，这个月支付宝会员没有继续领 B站大会员，改为 QQ 音乐会员 还是明智的，还是要少打开 B 站为好。

周六想到社交分享的跑步电台，想到分享的播客带上链接可以直接打开体验会更好；还想到看到别人分享的播客通过链接可以添加为任务，听完还可以把听过的播客记录下来。想到了播客分享的链接怎么识别 Episode 信息，这样可以在集合模块中记录下来。通过分析 Podcast 分享的链接 和 iTunes Lookup API 找到了确定 Episode 信息的方案，用了半天时间完成了接口开发。现在想来，其实这件事也不是重要和紧急，完全可以做为待办留到后面，而我又用掉了周六半天，现在看来就是时间和精力的浪费。

另外，还在自测的集合模块记录，图片是直接引用 PhotoKit 的 PHAsset，如果在 Photos 中删除了图片也就无法显示了。也想过存到后端或者 OSS，一直各种拖延；这周想到可以将图片存储到 App 中，使用 SDImageCache 存储到磁盘。如果只是实现这个方案也算正常，然而发现 SDImageCache 支持自定义 Cache 实现，还能切换为 YYCache，哎，我又去升级依赖库。到这里就有点画蛇添足，多此一举了。整个过程虽然没有花很多时间，却有点像软件开发中提到的过早优化；从精益创业的角度来考虑，这个优化效果先不说，没有这一步也不影响功能和使用，事后想来依然是在浪费。

就像 [第一篇增长最快的文章#精益创业先要避免浪费](https://hagerhu.com/post/2023w21-the-first-most-growth-article/#%E7%B2%BE%E7%9B%8A%E5%88%9B%E4%B8%9A%E5%85%88%E8%A6%81%E9%81%BF%E5%85%8D%E6%B5%AA%E8%B4%B9) 提到的一样，上面这些事情并没有很好的实践避免浪费，依然还在浪费时间和精力。也正是这些浪费，没有聚焦，才造成了开始提到的目标和现实的差距。
