# Google Buzz 得到一个 API 将集成到 Seesmic、TweetDeck 等 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/05/19/google-buzz-gets-an-api-will-be-integrated-into-seesmic-tweetdeck-and-more/>

# Google Buzz 得到一个 API 将集成到 Seesmic、TweetDeck 等等

自从 Google Buzz 第一次发布以来，有一个主要的功能已经明显消失了:一个 API。这项服务推出后不久，我们[一起黑进了](https://web.archive.org/web/20221003211328/https://beta.techcrunch.com/2010/02/10/google-buzz-button/)我们自己的“与 Buzz 分享”按钮，两个月后，谷歌[推出了](https://web.archive.org/web/20221003211328/https://beta.techcrunch.com/2010/04/13/google-buzz-spreads-across-the-web-launches-official-share-buttons/)一套“真正的”分享按钮。不幸的是，如果开发者想进行更强大的集成，他们仍然没有运气——这就是为什么你没有真正看到 Buzz 集成到任何主要的 Twitter/脸书客户端，这确实阻碍了 Buzz 的发展。如今，这种情况正在改变，因为谷歌正在推出一套 Buzz APIs，最终将允许开发者做 Gmail 中集成的 Buzz 主客户端可以做的一切，包括阅读评论、添加富媒体、喜欢等等。

我在 Google I/O，Buzz 团队成员 Chris Chabot 正在详细介绍新的 API(这篇文章将在整个会议过程中更新)。

众多受欢迎的服务，包括 Tweetdeck 和 Seesmic，都是 API 的合作伙伴(你可以在这里看到它们的完整列表)。其他与 Buzz 集成的应用有 Boxee、Meebo Bar、Plancast 和 Socialwok。

使用 OAuth 完成认证(尽管 Chabot 指出这需要两个间隙屏幕，团队意识到这并不理想)。

Chabot 说更多的正在进行中。未来，Buzz 将获得全面支持。

Seesmic 已经将 Buzz 集成到他们的 Android、桌面和网络应用程序中。你可以在这里找到更多关于 Seesmic 集成的信息。

Socialwok 也展示了他们的集成。在未来，他们计划使用 Buzz 附件来整合富媒体，使用 Salmon 进行评论联盟，并在其搜索引擎中提供“关键字监控”。

来自谷歌代码[博客](https://web.archive.org/web/20221003211328/http://googlecode.blogspot.com/):

> 最终用户选择使用 Google Buzz API 构建的应用程序，通过一个间隙确认屏幕来概述应用程序请求的访问范围(只读、读/写等。).他们可以看到哪些应用程序可以访问他们的数据，并可以随时从谷歌账户页面、谷歌仪表板、Gmail 设置中的“Buzz”选项卡或应用程序本身禁用访问。
> 
> 这个 API 的初始迭代包括支持获取公共的每用户活动提要、获取授权和认证的每用户活动提要(包括用户创建的内容和他们看到的内容)、搜索公共更新(按关键字、按作者和按位置)、发布新的更新(包括文本、html、图像等等)、发布评论、喜欢更新、检索和更新个人资料和社交图等等。最好的开始方式是开始阅读 Google Buzz API 开发人员文档。