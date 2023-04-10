# 新的 Android 应用 Smozzy 让你不用数据套餐就能上网冲浪 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/09/09/new-android-app-smozzy-lets-you-surf-the-web-without-a-data-plan/>

Smozzy 是一款新的 Android 应用，可以让你在没有数据套餐的情况下在手机上搜索网页。这款应用只在美国有效，只在 T-Mobile 手机上运行，并且要求你有一个短信计划(除非你想付费)。尽管有这些限制，该应用程序本身是纯粹的天才——它巧妙地使用短信和彩信发送请求和接收内容。对最终用户来说，这款应用看起来就像你自己的安卓手机浏览器一样，只是速度稍慢一些。

[![](img/d6318f1953a9cac74e05a289f24e0c27.png "smozzy-image")](https://web.archive.org/web/20230203161023/https://techcrunch.com/wp-content/uploads/2011/09/smozzy-image.jpeg)[时髦的](https://web.archive.org/web/20230203161023/http://smozzy.com/)应用程序非常简单——顶部只有一个组合 URL/搜索栏，下面有一个键盘。您可以在地址栏中键入您的搜索查询，也可以键入您希望 Smozzy 检索的确切 URL。

最终用户的请求通过 SMS 发送到 Smozzy 的服务器，响应通过 MMS 发送回来。这就是事情变得棘手的地方。Smozzy 下载请求的页面及其所有资源(样式表、图像等)。)并将所有内容放到一个 Zip 文件中。然后，该文件被编码为 PNG，并通过 MMS 发送出去。这是彻头彻尾的黑客味道！

也就是说，你应该知道 Smozzy 的信息没有加密，所以你不应该试图通过应用程序浏览安全内容或发送密码。(不好意思，没有 Facebooking，各位。)

令人难以置信的是，该应用程序完全按照承诺运行。我今天早上在我的 HTC Sensation 上测试了它，没有任何问题。网页没有以任何方式被剥离，功能如常，链接完好无损。

黑客新闻上的人正在为这个应用疯狂，他们也应该如此。(没错，我就是在那里发现的)。甚至有人提议帮助托管。

Smozzy 背后的概念并不完全新颖，然而，在发展中市场之外实现这样的想法却很少见。例如，2010 年夏天，[我写了一篇关于](https://web.archive.org/web/20230203161023/http://www.readwriteweb.com/archives/hp_launches_siteonmobile_web_surfing_via_sms_or_voice.php)惠普实验室一项名为 [SiteonMobile](https://web.archive.org/web/20230203161023/http://www.siteonmobile.com/) 的技术的文章，该技术允许手机用户通过短信上网。

但是有了 SiteonMobile，网络发行商就有责任使用类似小部件的工具，称为“小任务”,通过 SMS 来帮助网站导航。有了 Smozzy，尽管网上的任何东西都是可以得到的，而且出版商也不需要做任何改变。

Smozzy 是最近的 UT 奥斯汀毕业生，现在伯克利研究生杰夫多纳休的创作。他说，几年前他有了这个想法，当时他有一部没有数据套餐的黑莓手机。Donahue 对这款应用没有任何未来计划，因为非 T-Mobile 运营商对这款应用的测试还没有真正成功。

现在唯一的问题是 T-Mobile 是否会关闭它。希望运营商不会将 Smozzy 视为威胁——毕竟，虽然它让你在没有数据套餐的情况下上网，但这不是一种非常有效的方式。

*更新时间:上午 11:30，开发者详情。*