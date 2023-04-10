# Wordpress.com 在帖子订阅中启用 RSSCloud

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/09/07/wordpress-enables-rsscloud-in-post-feeds/>

# WordPress.com 在帖子订阅中启用 RSSCloud

![are we there yet](img/26b3df17ac1a68128323539b1eb91eb2.png "are we there yet")

[RSSCloud](https://web.archive.org/web/20230321184140/http://www.rsscloud.org/) 是一种新的提要格式规范，解决了轮询和通知问题。它的工作方式是在提要中添加一个`cloud`元素，这个元素描述了提要更新时应该通知的云服务器的路径。反过来，云服务器会将更新后的提要内容发送给所有订阅者和聚合者。RSSCloud 网站上有这个过程的[描述。](https://web.archive.org/web/20230321184140/http://rsscloud.org/walkthrough.html)

该协议是由 Dave Winer 设计的，他还起草了最初的 RSS 规范，并率先使用提要作为聚合内容的方式。RSSCloud 让 feeds 更具响应性和实时性。它不是一个轮询模型(“我们到了吗，我们到了吗”)，而是通过云服务器和 API 将更新和更新通知推送到用户。

新协议今天向前迈出了一大步，因为 WordPress.com[在所有帖子订阅源上启用了云标签](https://web.archive.org/web/20230321184140/http://en.blog.wordpress.com/2009/09/07/rss-in-the-clouds/)(评论订阅源将在稍后启用)。Winer [今天在推特上发布了这件事](https://web.archive.org/web/20230321184140/http://twitter.com/davewiner/status/3825067005)，Automattic 的[马特·莫楞威格](https://web.archive.org/web/20230321184140/http://ma.tt/)在一封电子邮件中证实，现在所有 WordPress.com 博客都支持这个标签。如果你在 WordPress 上查看一个 feed 的源，比如这个，你可以看到新的标签:

`<cloud domain='rsscloud.wordpress.com' port='80' path='/?rsscloud=notify' registerProcedure='' protocol='http-post' />`

为提要中的每个`channel`定义一个云通知服务器。这意味着，只要用户订阅的 WordPress.com 博客上有新帖子，支持新协议的客户端工具就会被推送更新。

这也可能意味着实时网络新格式战争的开始，让人想起过去的 RSS 和 Atom 之战。由 Brad Fitzpatrick 领导的另一组开发人员发布了一个名为 [pubsubhubbub](https://web.archive.org/web/20230321184140/http://code.google.com/p/pubsubhubbub/) 的格式和云中心，现在由 Google Reader 提供支持。肯定会有很多关于 WordPress.com 属于 RSSCloud 阵营的讨论，以及哪种协议/格式/方法等等。比另一个更好(毫无疑问，我们将在这个博客上展开一场辩论)。

Twitter 和 Friendfeed 等服务集中了实时数据和更新。RSSCloud 和对这种协议的更广泛支持是朝着分散这种服务的方向迈出的一步。

**更新:**WordPress.com 博客现在[有一个关于](https://web.archive.org/web/20230321184140/http://en.blog.wordpress.com/2009/09/07/rss-in-the-clouds/)更新的帖子