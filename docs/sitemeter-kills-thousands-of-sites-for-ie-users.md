# Sitemeter 扼杀了 IE 用户的数千个网站 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/08/02/sitemeter-kills-thousands-of-sites-for-ie-users/>

# Sitemeter 为 IE 用户扼杀了数千个网站

[![](img/1e1e44a3a70349785a250c1e64b6971f.png)](https://web.archive.org/web/20221210070419/http://crunchbase.com/company/sitemeter)

在另一个小工具变得疯狂并造成破坏的案例中， [Sitemeter](https://web.archive.org/web/20221210070419/http://www.sitemeter.com/) 中的一个错误导致大量使用免费网络分析工具的网站和博客无法为 Internet Explorer 用户加载。谷歌[博客](https://web.archive.org/web/20221210070419/http://crunchbase.com/product/blogger)的用户是第一批[报告](https://web.archive.org/web/20221210070419/http://groups.google.com/group/blogger-help-publishing/browse_thread/thread/4ce232f2581d21e4)在太平洋时间周五下午 6 点运行 Sitemeter 的网站遇到问题的用户之一。这个问题已经得到了部分纠正，尽管大约 16 个小时后，该公司仍未通过电子邮件或博客给出通知或官方回应。

Sitemeter 自豪地在他们的主页上展示了一个流量最大的网站列表。这些网站包括整个 Gawker 媒体网络、八卦博客 PerezHilton 和流行的政治博客 DailyKos。我们验证了所有这些网站都无法在 Internet Explorer 中加载，只有一个空白页面和一个 IE 错误窗口形式的响应，表明与 sitemeter.com 的连接问题。这个问题也影响了我们自己的 Techcrunch 法国博客，该博客将删除 sitemeter 代码作为唯一的解决方案。浏览器错误表明问题出在每个页面中包含的 Javascript 代码上。

正常运行时间监控服务，如 [Netcraft](https://web.archive.org/web/20221210070419/http://www.netcraft.com/) 没有报告这些网站的任何停机时间，因为该问题是 Javascript 和浏览器特定的，而不是更广泛的 HTTP 连接问题。主 [sitemeter](https://web.archive.org/web/20221210070419/http://crunchbase.com/company/sitemeter) 网站仍在运行，同时数百名博客作者发布了关于该问题的帖子，我们的 [tips 邮箱](https://web.archive.org/web/20221210070419/mailto:tips@beta.techcrunch.com)充满了关于该问题的链接和投诉。

早在 5 月份， [Michael 写了一篇关于](https://web.archive.org/web/20221210070419/http://www.beta.techcrunch.com/2008/05/17/dont-screw-your-partners-over-a-marketing-promotion/)我们自己与 Techcrunch 上的小工具提供商之间的问题如何影响了该网站的性能和正常运行时间，以及提供商不沟通这些问题如何使事情变得更糟的文章。没有真正的理由让广泛使用的服务(如 Sitemeter)关闭，因为有一些解决方案(如使用 IFRAME)可以绕过嵌入式代码中的错误，至少允许加载页面的其余部分。更糟糕的是，问题出现 16 个小时后，尽管嵌入了该服务的网站的用户和访问者发出了很大的噪音，但该公司仍没有任何官方消息，这也没有真正的原因。

**更新**:原来这是 ie 浏览器的一个错误造成的，Sitemeter 开发者没有考虑或测试这个错误。技术细节和对[错误的描述在这里](https://web.archive.org/web/20221210070419/http://motls.blogspot.com/2008/08/fix-internet-explorer-7-with-sitemeter.html)。这是否仍然意味着 Sitemeter 是罪魁祸首，还是因为一个已知的错误和一个没有测试的开发者，我们将看到反弹转移到微软。