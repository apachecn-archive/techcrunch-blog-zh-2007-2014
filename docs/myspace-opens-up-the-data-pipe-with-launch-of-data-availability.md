# MySpace 开放数据管道，全面推出数据可用性 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/06/26/myspace-opens-up-the-data-pipe-with-launch-of-data-availability/>

 [MySpace](https://web.archive.org/web/20230213024755/http://www.crunchbase.com/company/myspace) 是三大巨头中第一个宣布第三方网站将 MySpace 用户数据整合到其服务中的工具(统称为[数据可用性](https://web.archive.org/web/20230213024755/https://techcrunch.com/2008/05/08/myspace-embraces-data-portability-partners-with-yahoo-ebay-and-twitter/))。一天后，脸书宣布[脸书连接](https://web.archive.org/web/20230213024755/https://techcrunch.com/2008/05/09/facebook-responds-to-myspace-with-facebook-connect/)，三天后[谷歌好友连接](https://web.archive.org/web/20230213024755/https://techcrunch.com/2008/05/12/google-confirms-friend-connect/)。

今天，MySpace 正在全面推出数据可用性(今天下午在[developer.myspace.com](https://web.archive.org/web/20230213024755/http://developer.myspace.com/)寻找它)，任何第三方开发者现在都可以使用他们的 API 构建应用程序。谷歌的产品仍在少数网站上处于测试阶段([例如](https://web.archive.org/web/20230213024755/http://blog.go2web20.net/2008/06/testing-google-friend-connect-1-2-3.html))，在 7 月下旬的 F8 会议之前，我们可能不会从脸书那里听到更多消息。

MySpace 采取了比谷歌更有趣的方法，谷歌通过 iframe 控制发送到第三方网站的数据。MySpace 实际上是向这些网站传输数据，这允许服务之间真正的集成，而不仅仅是一个附加的社交工具。

开发人员可以从 MySpace 用户那里访问任何公开可用的个人资料数据，并将其集成到他们的网站中。这包括用户的姓名、照片、简历、社交图(朋友列表)和其他信息。用户通过从第三方服务到 MySpace 的一次性安全 [OAuth](https://web.archive.org/web/20230213024755/http://oauth.net/) 登录来授权数据传输。然后允许服务访问数据。

由于实际数据从 MySpace 流出，他们有一个严格的使用条款政策，禁止第三方网站存储或缓存数据，除了用户的唯一 MySpace 用户 id。每次呈现页面时，第三方必须通过一组 API 从 MySpace 重新请求数据。这意味着用户对 MySpace 个人资料或好友列表的任何更改都会立即应用到访问这些数据的第三方。

像谷歌和脸书一样，用户可以通过 MySpace 账户上的隐私控制面板撤销任何第三方的访问:

![](img/fb5575b2e12ba0eb745f2e2d440f00f1.png)
 **实际数据可移植，但没有同步**

这是迈向数据可移植性的真正一步，因为 MySpace 实际上允许数据从其服务器库流出。第三方不能存储这些数据的事实并不是一个完美的解决方案，因为 MySpace 保留了对它的最终控制权(我在我的 [Centralized Me](https://web.archive.org/web/20230213024755/https://techcrunch.com/2008/03/30/friendfeed-the-centralized-me-and-data-portability/) 帖子中讨论了这个问题)。真正的数据可移植性要求不断同步数据，以便用户保持控制。但是，在真正的标准出现之前，MySpace 的方法似乎不太合理。就用户数据权利而言，这是一个真正的进步，我希望我们会看到大量非常有创意的数据可用性实现。

我们现在正在构建一个测试应用程序，应该会在几个小时内投入使用。在接下来的几天里，我们会看到很多实现。