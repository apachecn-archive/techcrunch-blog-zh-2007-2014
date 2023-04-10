# RSSCloud Vs. PubSubHubbub:为什么胖 Pings 会赢

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/09/09/rsscloud-vs-pubsubhubbub-why-the-fat-pings-win/>

![](img/79aabc24ce7fe53861178a9b8e747391.png)

***编者按**:随着最近 RSSCloud 和 PubSubHubbub 之间的[争论](https://web.archive.org/web/20230321184118/http://www.techcrunchit.com/2009/07/23/hey-you-get-off-of-my-cloud/)，我们想听听开发者的意见，他能告诉我们哪一个可能更好，为什么。以下客座博文由 [Josh Fraser](https://web.archive.org/web/20230321184118/http://www.joshfraser.com/) 撰写，他是 [EventVue](https://web.archive.org/web/20230321184118/http://www.eventvue.com/) 的联合创始人，空闲时是 PubSubHubbub 的活跃撰稿人。他为 PubSubHubbub 贡献了几个客户端库，包括一个 WordPress 插件。猜猜他站在辩论的哪一边。*

在过去的几个月里，实时网络的兴起引起了很多关注。问题是网络的设计并没有考虑到实时性。技术社区非常需要支持新的协议，这些协议将推动 web 应用程序工作方式的根本转变。今天，我想看看两个在网络上实现实时通知的领先协议。虽然有像 XEP-0060 这样的支持实时通知的旧协议，但 [PubSubHubbub](https://web.archive.org/web/20230321184118/http://code.google.com/p/pubsubhubbub/) (PuSH)和 [rssCloud](https://web.archive.org/web/20230321184118/http://www.rsscloud.org/) 是两个很有希望获得采用的新协议。

PuSH 和 rssCloud 都解决了当今 web 应用程序工作方式中的一个根本缺陷。目前，在网上获取更新需要不断的轮询。订户被迫表现得像唠叨的孩子一样，问“我们到了吗？”订阅者必须不断地 ping 发布者，询问是否有新的更新，即使 99%的情况下回答是“没有”。这是非常低效的，浪费资源，并且一旦新内容出现就很难找到。两个协议[颠倒了当前的模型](https://web.archive.org/web/20230321184118/https://techcrunch.com/2009/07/09/speeding-up-rss/),因此更新是事件驱动的，而不是请求驱动的。我的意思是，这两种协议都通过告诉用户“不要问我们是否有新的东西”来消除轮询的需要。我们会告诉你的。”

戴夫·温纳比任何人都更早提出这个想法，这值得称赞。事实上，< cloud >元素在 2001 年就被添加到 RSS 2.0 规范中，但直到最近才被重新启用(很大程度上是为了响应人们对推送的兴趣)。rssCloud 本周取得了重大进展，[宣布【WordPress 正在](/web/20230321184118/https://techcrunch.com/2009/09/09/2009/09/07/wordpress-enables-rsscloud-in-post-feeds/)[为 WordPress.com 750 万博客添加 rssCloud 支持](https://web.archive.org/web/20230321184118/https://techcrunch.com/2009/09/07/wordpress-enables-rsscloud-in-post-feeds/)。相比之下，目前有超过 1 亿个订阅源支持推送，采用者包括 Friendfeed、Blogger、 [Google Reader](https://web.archive.org/web/20230321184118/https://techcrunch.com/2009/08/05/google-reader-speeds-up-sharing-with-pubsubhubbub/) 、LiveJournal、 [Google Alerts](https://web.archive.org/web/20230321184118/https://techcrunch.com/2009/08/19/google-continues-to-feed-the-pubsubhubbub-google-alerts-now-in-real-time/) 和 FeedBurner。我希望很快看到更多的服务采用这些新协议。

但是如果你发现自己对它们的不同感到困惑，你并不孤单。

从概念上讲，这两种协议非常相似。两者都在 feed 中添加了一个简单的声明，告诉订阅者哪个 hub/cloud 被委托负责处理订阅。这两种协议都有一个集中的中心，在新内容发布时通知订阅者。这两种协议都是基于 HTTP 的。

然而，理解实现中的细微差别是很重要的。在我看来，推送是目前更好的协议。基本上有三个因素使推送成为更健壮的协议:

首先，推送并不只是告诉你有什么东西改变了，它实际上向你发送了新的内容(也称为“胖 ping”))这是 rssCloud 缺少的一个重要特性。fat pings 不仅简化了订阅者的集成，还消除了无意中拒绝服务攻击的危险，因为成千上万的订阅者同时响应 ping 通知并请求更新的提要。这个问题在计算机科学中是众所周知的，通常被称为“雷群问题”虽然在 rssCloud 中解决这个问题相对简单，但它还没有得到解决。

第二，PuSH 允许可变的回调(通知发送的自定义 URL ),而 rssCloud 不允许。rssCloud 规范声明“通知被发送到发出请求的 IP 地址。您不能代表另一台服务器请求通知。这是非常有限的，因为您无法将处理订阅的服务器与接收 ping 通知的服务器分开。

第三，PuSH 对于处理退订有更友好的政策。在 rssCloud 中，每一个 feed 都会在 25 小时后自动退订。在推送中，有一个明确的取消订阅功能，可以选择在给定的时间后自动取消订阅。同样，当你大规模经营时，这个小细节很重要。有了 rssCloud，RSS 阅读器将负责每晚重新订阅数百万条 feeds 这远不如只在事情发生变化时才发送订阅/退订请求高效。

这并不是说 rssCloud 没有任何好处。实现 RSS 云比实现推送中心要容易得多。从设计上来说，推送集线器实现起来并不简单。

还有其他一些小差异，但这些是最重要的问题。其他一切都归结于语义。

我想解决两个协议中的一些误解。例如，许多人认为 rssCloud 仅仅是构建 Twitter 的分布式替代品。这在很大程度上是因为戴夫·怀纳[为 rssCloud](https://web.archive.org/web/20230321184118/http://rsscloud.org/walkthrough.html) 设定的目标是创建“一个松散耦合的类似 Twitter 的人际网络和 140 个字符的状态消息。”虽然这肯定是一个有趣的用例，但它促进了对协议及其功能的非常狭隘的看法。我认为 rssCloud 的潜力远比 Dave 认为的要大。

对 PuSH 最大的误解是它在某种程度上被谷歌拥有和控制。这根本不是真的。不仅有很多像我一样的独立开发者在开发推送，还有其他的推送中心，比如不受谷歌控制的 [SuperFeedr](https://web.archive.org/web/20230321184118/http://superfeedr.com/) 。[布雷特·斯拉特金](https://web.archive.org/web/20230321184118/http://www.crunchbase.com/person/brett-slatkin)指出:

> 我们的规范开发过程是完全透明的。您可以查看自 2008 年 8 月 5 日以来的所有代码签入。所有的讨论都在公共邮件列表上(没有谷歌内部的)。这个规范的要点是开放、去中心化，不受任何公司的控制。

总的来说，我相信 PubSubHubbub 和 rssCloud 都代表了网络的巨大进步。虽然我个人认为推是更好的选择，但竞争总是好的，会使两种协议都更强大。

(图片来源:Flickr/ [Libertinus](https://web.archive.org/web/20230321184118/http://www.flickr.com/photos/libertinus/171410082/) )