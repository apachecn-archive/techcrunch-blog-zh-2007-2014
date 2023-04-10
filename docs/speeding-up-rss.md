# 加速 RSS 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/07/09/speeding-up-rss/>

![](img/0836fa65afe4a40c317b8b15ae030b1f.png)

对不起，但是 RSS 订阅太慢了。我直接了解这一点。作为我在 TechCrunch 工作的一部分，我会监控大量 RSS 订阅源，寻找突发新闻。我们还制作自己的 feed，我可以看到它传播到各种 feed 阅读器和 feed 驱动的新闻聚合服务的速度有多快。发布一个故事和看到它在 RSS 提要中弹出之间的滞后时间通常是几分钟，然后它可能需要 10 到 15 分钟左右才能出现在类似 Google Reader 的东西中。TechCrunch 订阅源可能比大多数其他订阅源更频繁地被检查更新。在我们的业务中，每一秒都很重要，而 RSS 就是不能缩短时间。

虽然有一种观点认为 [RSS 正在消亡](https://web.archive.org/web/20230321184140/http://www.techcrunchit.com/2009/05/05/rest-in-peace-rss/)，被更即时的内容交付形式所取代，如 Twitter 和其他实时流，但许多人还没有准备好放弃它。相反，他们想通过加速来挽救它。明天，在我们的[实时流处理](https://web.archive.org/web/20230321184140/https://techcrunch.com/2009/07/08/win-a-ticket-to-the-real-time-stream-crunchup-this-friday/)上，我们将看到三个项目的演示，只是以稍微不同的方式。

谷歌工程师 Brad Fitzpatrick 和 Brett Slatkin 将展示一个名为 [pubsubhubbub](https://web.archive.org/web/20230321184140/http://code.google.com/p/pubsubhubbub/) 的新推送协议的演示，Netvibes 首席执行官 Freddy Mini 将展示他类似的 RSS 即时更新中心，WordPress 工程师 Andy Skelton 将展示一个 Jabber 客户端，它使用 [XMPP](https://web.archive.org/web/20230321184140/http://xmpp.org/) 协议将博客标题以比 RSS 更快的速度推送到一个类似 IM 的环境中。

pubsubhubbub 和 Netvibes 技术创建了 RSS hubs，一旦有可用的提要，它就会推送出去。这种方法与作为 RSS 基础的轮询方法形成对比。[轮询方法很糟糕](https://web.archive.org/web/20230321184140/http://code.google.com/p/pubsubhubbub/wiki/WhyPollingSucks),因为它要求代表 RSS 订阅者的服务器不断地 ping 发布 RSS 提要的服务器，询问是否有新的内容。取决于这种情况发生的频率，你最终会有一个滞后。随着通信变得更加实时，这种滞后变得更加明显。

pubsubhubbub 解决这个问题的方法是在中间放置一个 RSS Hub，它可以更有效地将提要推送到订阅它们的服务器。它是一个开放的协议，可以应用于任何现有的 RSS 或 Atom 提要，以及其他实时流。如果你想到每个人都想访问的 Twitter firehose，这种方法让任何人都可以为不同类型的数据流创建自己的 firehose。它更像是一种联合方法。您可以将这些 RSS Hubs 视为各种 RSS 提要的内容交付网络，在概念上类似于 Akamai 为视频流所做的工作。

Netvibes 正在为自己的服务创建自己的专有版本，这是它独立开发的。它被称为 RSS 即时更新中心。今天，Netvibes 页面上的所有这些小部件都要花很长时间来加载，因为它们都必须获取底层的数据源。即时更新中心将自动缓存和推送这些提要，这样小部件可以更快地加载，并且无需刷新即可持续更新。如今，Netvibes 小部件支持的任何数据流(远远超过 RSS)都将通过即时更新中心推送。它也将成为 Netvibes 今年晚些时候推出的新流阅读器的基础，作为当前小工具网格和[杂志风格布局](https://web.archive.org/web/20230321184140/https://techcrunch.com/2008/12/08/netvibes-adds-slick-magazine-layout-options-supports-opensocial/)的替代(见下面的截图)。

WordPress Jabber 客户端使用不同的推送技术 XMPP 来加速 RSS。效果是标题像即时消息一样弹出。Jabber 主要用于 Gtalk 之类的 IM 客户端，但 WordPress 将其用作提要阅读器和微博发布者。它的伟大之处在于它是双向的。在演示中，Skelton 将展示如何使用 Jabber 客户端作为直接发布到您的博客的界面。订阅源阅读和博客发布都可以在同一个地方以更实时的方式完成。Jabber 客户端也可以用作博客评论系统，并作为一个小部件直接嵌入到网页中，将评论变成一个聊天室。

我们所看到的是出版和即时通讯世界的碰撞。我们越快结束发布和响应之间的循环，我们就越能看到实时数据流呈现公共 IM 系统的外观和感觉。Twitter 是异步的，但它经常给人一种即时的感觉，来回的对话有时就像私人即时消息聊天一样快。随着所有出版平台的加速发展，这仅仅是未来事物的一个缩影。

(图片来源:Flickr/ [joiseyshowwa](https://web.archive.org/web/20230321184140/http://www.flickr.com/photos/joiseyshowaa/2760573261/) )

[![new_feedreader_listview02](img/a80d0f3dbb2cacf77c8dca7ea34a4346.png "new_feedreader_listview02")](https://web.archive.org/web/20230321184140/https://techcrunch.com/wp-content/uploads/2009/07/new_feedreader_listview02.png)

以下是 PubSubHub 在实时活动中的演示视频:

【YouTube = http://www . YouTube . com/watch？v=ewQBgbysSOQ&w=425&h=344]