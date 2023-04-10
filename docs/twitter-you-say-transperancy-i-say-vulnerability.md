# Twitter:你说透明，我说脆弱 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/10/21/twitter-you-say-transperancy-i-say-vulnerability/>

# 推特:你说透明，我说脆弱

![](img/af5dcf4367917e2279b5a155cd898e08.png "twitter")

今天早上我们收到了一些提示，称 [Twitter](https://web.archive.org/web/20221006192647/http://www.twitter.com/) 的大多数网络服务器向公众公开了服务器和负载平衡器的状态信息。[状态页面](https://web.archive.org/web/20221006192647/http://httpd.apache.org/docs/2.0/mod/mod_status.html)，这是开源 [Apache web 服务器](https://web.archive.org/web/20221006192647/http://httpd.apache.org/)中的一个(通常是默认的)选项，转储特定服务器的所有连接和状态信息的输出。管理员使用这些信息来监控服务器，这些页面通常要么被完全删除，要么被锁定，以防止这些信息被用于恶意目的。

在过去 24 小时的某个时间点(根据状态页面本身，我更准确地猜测是 22 小时 28 分 4 秒前)，Twitter web 服务器引入了一个错误配置，将这些信息暴露给公众。该页面包括整体服务器统计数据，以及该服务器当前处理的每个 HTTP 请求，以及完整的请求 URL。通常通过请求 web 服务器的`/server-status`来访问服务器状态页面。就 Twitter 而言，这种暴露允许任何人看到有时依赖于保密来保持安全的请求，例如 oAuth 密钥，它用于授权应用程序访问 Twitter 帐户。

页面开放的消息通过 Twitter 迅速传播开来，一些人称之为“巨大的透明度”,而另一些人则认识到这是什么——有点太透明了，而且是无意的。Twitter 非常迅速地做出了回应，屏蔽了对该页面的所有访问，绝大多数发现的信息纯粹是信息性的，可以通过其他方式推断出来。你的 Twitter 账户可能又安全了，但这并不意味着我们不能出去玩，同时偷偷看看幕后的 Twitter。

下面一个这样的页面的截图，其中一些信息被删除了。

![twitter-status](img/315762a03de3fd9a9c06b536d0f3edee.png "twitter-status")