
![gap-between-goal-and-real](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.07.49@2x.png)

### 目标与现实的差距

周五去浙江图书馆，相比西湖图书馆、文二路博库书城，这里的桌椅高度显然更适合一些。

![review goal of may](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.59.57@2x.png)

回顾刚过去的 5 月份，看着月初定下的目标，回顾每一天发现现实与目标之间，差距是如此之大。当初定的 4 个方向，第 1 项推广渠道想到了最早逛的威锋社区，发现帐号等级不够没有发帖权限；第2、3 两项则没有开始；湾区周报 5 月份少了一期，还是没安排好时间来寻找和阅读，还发现刷了不少油管和 B 站视频。

记录和跟踪每天的事情，月底总结回头看，才发现 5 月目标和现实的差距。当初定下月度目标的时候，还把「重要且有意义的事」写在目标的前面，想给自己一个明显的提醒。现在看来，这个提醒并没有起到应有的作用。

![loop in principle](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.00.17@2x.png)

达利欧在《原则》中提到，反思 + 总结 = 进步，五步流程法如此往复，最终达到螺旋式上升的态势。年度目标 -> 季度目标 -> 月度目标 -> 每周目标 -> 每天跟踪 -> 每周总结 -> 月度总结 -> 季度总结 -> 年度总结，就是我给自己的反馈循环，希望能够通过如此往复实现正反馈或者正循环。之前的习惯还没意识到目标和现实的差距，这次突然意识到原来差距是如此之大，而且是到了月底总结才察觉。

如果能在前 2 周每周总结的时候意识到并调整，也许这个月会好一点。《精益创业》中提到最小化可行产品，就是用最快的方式，用最少的精力完成 “开发 - 测量 - 认知” 的反馈循环，避免浪费资源和精力。对于反思总结应该也一样，就是要加快 “目标 - 跟踪 - 总结” 的反馈循环，更快意识到是否偏离了方向，也就能更快从偏离的方向上纠正，久而久之也会进入螺旋上升的态势。

### 从分享的播客开始

2022 年度总结的时候，总结了 读过的图书，看过的电影，买过的设备等方面。今年想着给自己做的集合应用，也是围绕记录和量化来做，也想到了记录听过的播客。

跑步的时候偶尔会听播客，听到喜欢的也会用「跑步电台」分享出来。分享一方面是为了记录自己听过和感受，另一方面也是好的东西值得分享。

为了识别播客分享的链接来分享和记录，开始寻找和研究可行方案。复制了 Podcast 的分享链接，通过搜索发现 iTunes Lookup API 可以使用播客 ID 获取 Podcast 和 Episode 信息，分享链接中带上的 Podcast 的 id (id1475113228) 和 Episode 的 trackId (i=1000548957645) 就可以确定  Podcast 或者 Episode 的元数据了。

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

后来发现有专门站点 [Get RSS Feed](https://cmcn.me/link?target=https://getrssfeed.com/) 也是这个功能， 而且还支持从 Google Podcast，SoundCloud，Blog 和 Site。Get RSS Feed 是 [Podcast Addict](https://cmcn.me/link?target=https://podcastaddict.com/) 的一个功能, 作者主要靠广告获得收入，但广告收入持续下滑；后来开通了 一次性付费 支持，觉得也并不可持续；又增加了 订阅功能 来希望能有个稳定的收入，想要了解详情可以[点击阅读](https://podcastaddict.com/premium)这篇文章。

![GetRSSFeed stats](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2016.49.27@2x.png)

![Podcast Addict stats](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2016.50.56@2x.png)

很好奇作者的广告收入，于是看了一下这两个站点的流量数据，Podcast Addict 流量挺高的。

### 依然还在浪费资源

这周总结回顾的时候发现，本周依然浪费了不少时间和精力。

![riding just for fun](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2021.08.23@2x.png)

被 B站 推荐了 UP 主 [我就骑着玩](https://cmcn.me/link?target=https://space.bilibili.com/1493959577) 的旅行视频，开始看就一发不可收拾，看过之后知道 UP 主是个退役女兵，是不是文艺兵不知道，但拍出来的景色和配乐真的很棒，如果你也喜欢这类旅拍视频可以试试。

看过不少摩旅去西藏的视频，不少都是很好的摩托和装备，「我就是骑着玩」则是骑着小踏板就上路了。可见，想去外面看世界的人很多，但关键还是有多想要去看。除了 我就是骑着玩 的小踏板摩旅，还刷了 [袁学周](https://cmcn.me/link?target=https://space.bilibili.com/295041700) 公路车比赛视频，一不注意就过去了近两小时，时间就这么在指尖溜走。看着 B 站这一周观看的历史记录，这个月的支付宝会员也就没有继续领 B站大会员，而是换成了 QQ 音乐会员。

周六想到社交分享的跑步电台，想到分享的播客带上链接可以直接打开体验会更好；还想到看到想听的播客可以通过链接添加为任务，听完把听过的播客记录下来。想到了播客分享的链接怎么识别 Episode 信息，通过分析 Podcast 分享的链接 和 iTunes Lookup API 找到了确定 Episode 信息的方案。虽然用半天时间完成了接口开发，现在想来，其实这件事也不是重要和紧急，完全可以做为待办留到后面，[番茄工作法](https://cmcn.me/link?target=https://www.youtube.com/watch?v=c9v4CPaV1s8) 中提到过突如其来的事情可以记录下来而不是立马去做，而我就这么用掉了周六半天，现在看来就是时间和精力的浪费。

也是同一天，还在自测的集合模块记录，照片是直接引用 PhotoKit 的 PHAsset，如果照片在 Photos 中删除了也就无法显示了。要解决这个问题，想过存到后端或者 OSS，一直各种拖延；这周想到可以将图片存储到 App 中，使用 SDImageCache 存储到磁盘。如果只是实现这个方案也还正常，看文档发现 SDImageCache 支持自定义 Cache 实现，可以切换为 YYCache，哎，我又去升级依赖库。到这里忽然觉得有点画蛇添足，多此一举，有点像软件开发中提到的过早优化。从精益创业的角度来考虑，这个优化能有多大效果先不说，却一点也不影响功能和体验，事后想来依然是在浪费。

就像 [第一篇增长最快的文章#精益创业先要避免浪费](https://hagerhu.com/post/2023w21-the-first-most-growth-article/#%E7%B2%BE%E7%9B%8A%E5%88%9B%E4%B8%9A%E5%85%88%E8%A6%81%E9%81%BF%E5%85%8D%E6%B5%AA%E8%B4%B9) 提到的一样，上面这些事情并没有很好的实践避免浪费，依然还在浪费时间和精力。也正是这些浪费，没有聚焦，才造成了开始提到的目标和现实的差距。
