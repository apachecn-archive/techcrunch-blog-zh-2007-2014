# Twitter 开始用户流测试。实时技术应该有助于缓解 API 压力

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/07/28/twitter-user-streams/>

# Twitter 开始用户流测试。实时技术应该有助于缓解 API 压力

一段时间以来，Twitter 一直在开发一个新的 API:Twitter 流媒体 API。其背后的想法是允许第三方 Twitter 客户端实时接收持续的推文更新。正如开发者倡导者泰勒·辛格特里[今天](https://web.archive.org/web/20221218151704/http://groups.google.com/group/twitter-development-talk/browse_thread/thread/f7b3dd8ac9e10395)在 Twitter 开发对话谷歌小组上指出的，针对桌面客户端的这一新功能(也称为“用户流”)的有限测试现在已经开始。

目前，两个流行的 Twitter 桌面客户端 TweetDeck 和 Echofon 已经可以访问新的 API 进行测试。Singletary 指出，并不是所有这些客户端的用户一开始都会看到这项新技术的应用。取而代之的是，每款应用都将逐步推出。一旦发生这种情况，Twitter 将开始向其他客户开放流媒体 API。

今年四月，Twitter 在他们的 Chirp 会议上第一次谈论这个新的 API。其他人已经在内部测试了一段时间，因为 Twitter 也在通过 API 测试其新的[注释功能。](https://web.archive.org/web/20221218151704/https://techcrunch.com/2010/06/02/twitter-annotations-testing/)

虽然该功能非常酷，并使第三方客户端更有趣，但流媒体 API 也对 Twitter 有很大帮助。正如 Singletary 指出的那样，“*向用户流的过渡应该会给
REST 和 Search APIs 带来可观的容量，增加 Twitter 用户的稳定性&开发者也是如此。*“由于他们最近的[扩展问题](https://web.archive.org/web/20221218151704/https://techcrunch.com/2010/06/15/twitter-world-cup-2/)，Twitter 不得不施加的[限制伤害最大的一个方面是 API](https://web.archive.org/web/20221218151704/https://techcrunch.com/2010/06/29/twitter-api-limit/) 。像 TweetDeck 和 Seesmic 这样的服务在很大程度上依赖于他们各种窗口的搜索 API 所以很明显，这是一个问题。流式 API 应该可以缓解这种情况。

还有更多。Singletary 指出:

> 此外，还有几个有趣的新事件类型:收藏、转发、关注和列表添加也与直接消息、提及、用户时间表和主页时间表一起传输。

同样，所有这些应该有助于缓解 Twitter 其他 API 的压力。唯一的问题是:以一种有意义的方式铺开需要多长时间？Twitter 表示，公开测试暂定于 2010 年第三季度或第四季度进行。

在消息的最后，Singletary 还暗示了一个名为 Site Streams 的新 API 产品:

> 需要同时使用多个用户流的应用程序开发人员将由一个即将推出的叫做 Site Streams 的流 API 产品提供服务。当我们准备好的时候，请继续关注更多的信息。

*【感谢理查德】*