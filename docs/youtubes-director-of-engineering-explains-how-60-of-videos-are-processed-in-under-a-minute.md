# YouTube 的工程总监解释了如何在不到一分钟的时间内处理 60%的视频 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/16/youtubes-director-of-engineering-explains-how-60-of-videos-are-processed-in-under-a-minute/>

你很难找到一个不认为 YouTube 是互联网巨头的人。毕竟，每一次病毒点击都有一个大而醒目的计数器，累计其收到的数百万或数千万次点击，如果你愿意，你可以浪费一生的时间点击无穷无尽的猫视频。

但即便如此，也很难不对该网站不时下降的一些统计数据感到吃惊。比如，从技术上讲，它是仅次于谷歌的互联网第二大搜索引擎。或者是它首次公布的一个新数据:YouTube 用户现在仅从移动设备上每分钟就上传两个小时的视频。它每天从移动设备上获得超过 2 亿的浏览量。

对于这样的统计数据，一个合理的反应是，“怎么做？”

我有机会与 YouTube 工程总监克里斯蒂安·凯泽(Christian Kaiser)交谈，他最近辞去了网飞工程副总裁的职务，执掌谷歌这个视频巨头。Kaiser 于 4 月加入 YouTube，他不能透露太多幕后的细节。但他确实有一些更广泛的东西可以分享，关于 YouTube 处理海量输入数据的方法，以及未来的挑战。

鉴于 YouTube 的巨大规模，该公司在后端运行大量定制工具来尽快转码视频就不足为奇了(这种转码系统被称为 *Viper* )。Kaiser 表示，最近推出的一项关键速度改进与视频处理的顺序有关，这些步骤过去是按顺序进行的，现在是并行进行的，这导致了视频直播时间的“巨大改善”。

多大？今天，60%的视频在不到一分钟的时间内上线——一年前，*没有*视频被处理得这么快。

至于团队目前关注的挑战，Kaiser 表示，对快速无缝播放的需求(这显然一直是一个关键问题)比以往任何时候都更大，特别是在向电视传送内容时。该团队目前正在实现自适应流媒体，它可以根据你的连接速度动态改变视频的比特率(Hulu，Ooyala 和其他一些网站上的视频已经在这样做了)。当我问 HTML5 是否会很快实现这一点(这是 YouTube 正在慢慢走向的方向)时，Kaiser 说它现在还没有在任何地方实现，但它正在努力使它成为现实。

凯泽还讨论了 YouTube 用来在全球范围内快速提供所有这些视频的一个“技巧”。该公司已经在全球范围内建立并部署了数百个硬件设备，用于缓存和提供最受欢迎的 YouTube 视频，其方式与 CDN 非常相似。

在结束我们的简短采访时，我问凯泽，他是否认为我们还没有到达“转折点”，即人们将开始使用在线服务而不是有线电视作为他们消费视频内容的主要方式。凯泽说，我们已经看到了一点这种情况——尤其是像 Hulu 和网飞这样的服务正在起飞。但是他不确定从有线到 IP 的转变会有一个陡峭的拐点。相反，他认为这可能更为渐进(并且已经在发生)。