# iPhone SDK 和限制:一些细节不是很好。

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/03/07/iphone-sdk-some-of-the-details-arent-great/>

 [](https://web.archive.org/web/20230403132552/http://www.crunchgear.com/2008/03/06/live-blogging-apples-iphone-sdk-event/) 显然，史蒂夫·乔布斯和他的团队今天在宣布 iPhone SDK 的[上市时，并没有详细说明所有细节。这更像是一次高水平的传球。但细节是第三方开发者在双脚跳入 iPhone 之前需要考虑的。](https://web.archive.org/web/20230403132552/https://techcrunch.com/2008/03/06/iphone-20-enterprise-ready-developer-ready/)

去年，当脸书宣布推出 Facebook 平台时，开发者不得不决定忽略它，为它建立一个标准网站，或者专为脸书建立。风险投资家乔希·科佩尔曼提出了一个论点，即一些开发者应该立即在脸书诉为 MySpace 开发的基础上进行开发，尽管事实上它过去是(现在也是)专有的。

Facebook 平台有自己的[风险](https://web.archive.org/web/20230403132552/https://techcrunch.com/2007/09/17/facebook-launches-fbfund-with-accel-and-founders-fund-to-invest-in-new-facebook-apps/) [基金](https://web.archive.org/web/20230403132552/https://techcrunch.com/2007/07/09/bay-partners-launches-facebook-apps-only-fund/)来支持新的创业公司。从今天起，[iPhone 也是如此](https://web.archive.org/web/20230403132552/https://techcrunch.com/2008/03/06/kleiner-perkins-anounces-100-millioin-ifund-for-iphone-applications/)。

构建 iPhone 应用程序的决定非常相似。一些开发人员会在他们现有的产品中添加一个。其他人将只使用 iPhone。

我们应该期待 Kopelman 写一个新帖子，敦促开发者尽快建立一个 iPhone 应用程序吗？也许吧。但是一些博客作者和开发者今天对细则做了一些挖掘，并且有一些令人不安的细节。

在今天的活动中公布了一些限制。例如，网络电话服务基本上就不走运了。他们只能通过 wifi 上网，而不是手机网络。不过，这是一个更大问题的信号——苹果不会允许应用程序威胁到他们来自 iPhone 的任何收入来源。同样，SIM 卡解锁是[禁止的](https://web.archive.org/web/20230403132552/http://www.ryanblock.com/2008/03/questioning-iphone-sim-unlocks-on-the-sdk-is-the-obvious-unimportant/)。但是其他不那么黑白分明的应用呢？[约翰·格鲁伯](https://web.archive.org/web/20230403132552/http://daringfireball.net/linked/2008/march#thu-06-block)询问亚马逊是否能够推出一款允许用户从亚马逊 MP3 商店购买歌曲的 iPhone 应用程序。这是一个很好的问题，目前还没有答案。

[其他限制](https://web.archive.org/web/20230403132552/http://macdaddyworld.com/2008/03/06/iphone-sdk-first-thoughts/)详见开发商协议。开发者只能使用已发布的 API，并且只能按照苹果公司规定的方式使用。好的，这有助于稳定。应用程序也不能在指定区域之外的任何地方写数据，这意味着开发人员不能从任何其他应用程序修改数据。

但是我们发现的一个最大的问题是 100 页的 iPhone 人机界面指南。这是一个公共文档，但您必须是注册的 iPhone 开发人员才能看到它。我们已经通过 docstoc 将其嵌入下面。

用户一次只能运行一个应用程序，如果他们离开一个应用程序，它就会退出。这看起来没什么大不了的，但这意味着你不能离开一个应用程序，让它继续做事情。这是目前 iPhone 支持网站的一个大问题——一旦你离开浏览器，连接就中断了。对于 iPhone 来说，希望已经安装的应用程序可以继续在后台运行，最有用的是，从网络上收集信息并向网络发送信息。

> 一次只能运行一个 iPhone 应用，第三方应用从不在后台运行。这意味着当用户切换到另一个应用程序，接听电话，或检查电子邮件时，他们正在使用的应用程序退出。(第 16 页)

对于一些开发者来说，这将是一个严重的问题。例如，假设一名开发人员想要从 iPhone 中获取位置信息(通过 iPhone 的蜂窝三角测量功能创建)并将其转储到 [FireEagle](https://web.archive.org/web/20230403132552/http://www.crunchbase.com/product/fire-eagle) 中，以跟踪您去过的地方。除非你一直打开应用程序，并且除此之外不要用 iPhone 做任何事情，否则这是行不通的。另一个例子:即时通讯应用程序(我们今天在活动中看到了一个 AIM 版本的演示)，不能在你做其他事情的时候在后台运行并收集消息。离开应用程序去接电话，它会显示你离线。底线是——任何想要定期与网络交互来做事情的应用程序，都不能持续地与网络交互。

也许未来版本的 iPhone 会有更多的 CPU 和内存资源，不会有这种限制。但是现在，所有类别的应用程序都是无用的，或者比它们本来的用途要少得多。

如果你知道或发现其他重要的限制，请在评论中用链接或文本让我们知道，我们会在这里添加它们。

【http://www.docstoc.com/docs/wrapper.ashx?doc_id=418559】T2&swf _ URL = http % 3A//content 1 . docstoc . com . S3 . Amazon AWS . com/iphoneshumaninterfaceeguidelines . pdf . swf&show related = 0&showotherdocs = 0&showstats = 0&enable full screen = 1
[iphone 人机界面指南](https://web.archive.org/web/20230403132552/http://www.docstoc.com/docs/418559/iPhones-Human-Interface-Guidelines)–获取更多[免费文档](https://web.archive.org/web/20230403132552/http://www.docstoc.com/)