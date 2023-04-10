# 由前谷歌和前美国国家安全局工程师创建的 Disconnect Search 让你可以在不被追踪的情况下使用谷歌、必应和雅虎

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/10/07/disconnect-search-built-by-ex-google-and-ex-nsa-engineers-lets-you-use-google-bing-and-yahoo-without-tracking/>

早在 2010 年，当时的谷歌公司 Brian Kennish [就开始了一个兼职项目，目的是在一个人的脸书浏览会话期间切断广告跟踪，](https://web.archive.org/web/20230403031932/https://techcrunch.com/2010/10/20/google-facebook-disconnec/) [Disconnect](https://web.archive.org/web/20230403031932/http://www.disconnect.me/) 已经进行到[筹集资金](https://web.archive.org/web/20230403031932/https://techcrunch.com/2010/10/20/google-facebook-disconnec/)(两次)，在多种浏览器和网站上工作，为特定用户(例如[孩子](https://web.archive.org/web/20230403031932/https://techcrunch.com/2013/08/12/disconnect-the-anti-ad-tracking-startup-now-has-a-privacy-app-specifically-for-children-built-by-an-ex-nsa-engineer/))创建应用程序，并雇用更多的工程师，包括两名来自谷歌的工程师和一名来自国家安全局的工程师。随着每周有 100 万人使用其应用程序，Disconnect 现在正在处理当今人们在网上发现内容的最流行的方式:搜索引擎。今天，该公司推出了 [Disconnect Search](https://web.archive.org/web/20230403031932/https://www.disconnect.me/search) ，这是 Chrome 和 Firefox 浏览器的扩展，允许用户在谷歌、必应和雅虎以及 Blekko 和 DuckDuckGo 上搜索时保持隐私。

该扩展既可以在搜索门户的主网站上运行，也可以通过浏览器的 omnibox(对于 Firefox)或浏览器栏(对于 Chrome)运行。(“从任何地方搜索”功能仍处于测试阶段。)Disconnect 表示，它已经申请了专利来保护其专有的操作方式。

Casey Oppenheim 是前消费者权益律师，也是 Disconnect 和 Kennish 的联合创始人，他指出，部分由于搜索引擎是其他一切的门户，当涉及到用户隐私时，搜索引擎往往是最具侵犯性的。“你的搜索绝不是隐私，”他在一份声明中指出。“搜索引擎，甚至网站和互联网服务提供商，都可以保存你的搜索，并通过你的用户账户将它们与你的真实姓名联系起来。”事实上，如果你登录了你的 Gmail 或其他谷歌服务，然后访问了 Google.com，你就会确切地知道这是如何运作的。

前国家安全局工程师、现任 Disconnect 首席技术官的帕特里克·杰克逊(Patrick Jackson)指出，更令人担忧的是，即使你没有登录其他服务，这种情况也会发生。“即使你从未登录帐户，搜索引擎和许多网站通常会保存你的搜索并将其连接到一个 IP 地址，这可以让公司唯一地识别你的计算机。”我想，这是一个国安局工程师非常熟悉的技术。

该公司表示，Disconnect Search 通过四个渠道工作，其中一些方法借鉴了 VPN 隧道服务，可以屏蔽你的 ip 地址:

—搜索查询通过 Disconnect 的服务器路由，“这使得查询看起来像是来自 Disconnect，而不是特定用户的电脑，”该公司表示。

—因此，搜索引擎被阻止(封锁)将关键字传递到从搜索结果页面访问的站点。

—所有查询都是加密的，这可以防止 ISP 看到它们。

—最重要的是，在将您的查询路由到自己的服务器后，Disconnect 不会记录任何关键字、个人信息或 IP 地址。

结果不会以任何明显不同的方式传递给用户。他们仍然是搜索引擎的“原生”用户，就像用户可以用他们已经用过的方式参与网站一样。我在测试产品时进行了两次搜索，一次使用了断开连接搜索过滤器，另一次没有使用，差不多产生了一组相似的结果。通过断开连接搜索提供这些结果会有一点延迟。

(Chrome，带断开搜索)
![Disconnect Google Chrome](img/c4707fc5337d736ffe19dc4f73e7efb4.png)

![non-disconnect safari](img/a15520e6b8b5c3334aeaca5e3032808f.png)(Safari，不带)

与 Disconnect 的其他产品一样，更长期的想法是建立特定的付费服务，为用户提供额外的功能；如果我们看到该公司也转向特定的解决方案，这些解决方案可能会与那些让用户坐在防火墙后面的组织合作，今天，出于安全和隐私保护的原因，防火墙可能会阻止这些用户访问整个互联网(例如，政府组织中的一些网络就是这种情况)，我不会感到惊讶。

但是现在，断开搜索，作为一项无偿服务。仍然是一个强有力的例子，说明为什么不总是这样，如果你接受免费服务，你[默认成为产品](https://web.archive.org/web/20230403031932/http://www.techdirt.com/articles/20121219/18272921446/stop-saying-if-youre-not-paying-youre-product.shtml)。

**注意/更新**:需要澄清的是，虽然 Disconnect 可以在搜索引擎或其他公司的广告跟踪等领域帮助保护用户隐私，但这并不一定意味着 Disconnect 可以被视为针对政府等其他力量的完全隐私屏障，正如下面的评论所指出的那样。

我向奥本海默提出了这个问题，他是这样解释的:“根据最近披露的情况，人们不应该认为 Disconnect 或任何其他组织可以阻止政府访问你的搜索查询。Disconnect Search 专注于阻止公司访问你的搜索结果。所以这是一种帮助，但在联邦政府改变政策之前，不会完全阻止。