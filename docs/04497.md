# 现场报道:脸书的签到功能和新的“地点”标签 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/05/09/facebook-places-check-in/>

代码不会说谎。

在过去的几周里，有很多关于脸书定位功能的猜测。至少部分猜测现在可以结束了。我们现在知道脸书计划很快推出什么样的定位服务，因为这就在他们的代码里。

具体来说，它就在网站的[touch.facebook.com](https://web.archive.org/web/20230204224320/http://touch.facebook.com/)版本的 JavaScript 中。这是移动版的脸书，针对 iPhone 和 Android 手机等触摸屏手机进行了优化。在 Safari 浏览器(当然，iPhone 使用的是的一个版本)上访问这个网站会导致有趣的事情发生:它只是挂起。当您启用调试模式时，很容易看出原因。

这个脸书网站的触摸版试图填充一个叫做“位置标签”的东西不幸的是，脸书还没有启用它，所以它抛出了错误。虽然这本身很有趣，但更有趣的是当您更深入地研究这个 JavaScript 时会发现什么。

根据代码，这似乎是脸书即将推出的内容:该网站的移动版本使用 HTML5 定位组件从你的手机中获取你的位置信息。一旦它这样做了，你就会被带到脸书这个新的地点区域，这里大概会有你周围的地点列表。在这里，您可以点击按钮办理登机手续。是的，会有签到。

但它也比那更有趣。根据这个代码，脸书不仅会记录你的纬度和经度，还会记录你的高度、方向和速度(假设他们能获得所有这些信息)。它还将记录位置测量的精度。我只是在这里推测，但也许这将有助于遏制作弊行为，这种行为已经开始在 Foursquare 等其他位置服务上猖獗起来。

同样，这段代码目前只在 touch.facebook.com 版本的网站上找到(这段代码专门放在 iPhone 的目录中)。这可能意味着脸书将首先在这里推出该功能，然后将其转移到 iPhone 和 Android 等平台上的本地移动应用程序中。这也意味着它可能不在脸书本土。这很有意义，因为目前只有一些桌面浏览器支持定位。不过，你必须假设 Places 区域将位于 Facebook.com 的某个地方，即使你不能在发布时从桌面登录。

这一信息似乎与上周[的](https://web.archive.org/web/20230204224320/http://adage.com/digital/article?article_id=143761)[报道](https://web.archive.org/web/20230204224320/http://adage.com/digital/article?article_id=143742)相吻合，报道称脸书正与一些大品牌合作开发他们的定位功能。据推测，在这个新的位置标签中，这些品牌将被填充，甚至可能被突出显示。

读完这些故事后，[我想知道](https://web.archive.org/web/20230204224320/https://techcrunch.com/2010/05/07/facebook-location-foursquare-twitter/)脸书是否打算做签到，或者做一些类似 Twitter 的事情:简单地让人们在状态更新中标记他们的位置。现在很清楚(假设他们完全部署了这段代码),签入实际上正在到来。

也就是说，如果脸书允许 Foursquare 和 Gowalla 等其他定位服务通过脸书连接或更新的 OpenGraph APIs 来填充位置参数，我也不会感到惊讶。接下来的问题是，脸书是否也会利用这些服务的位置数据库来建立自己的数据库——或者他们是否已经在幕后这么做了。[正如我昨天写的](https://web.archive.org/web/20230204224320/https://techcrunch.com/2010/05/08/place-database/)，脸书很可能是走向一个每个人似乎都想要，但似乎没有人能实现的位置数据库的关键组成部分。

更有趣的是，我们听说脸书首席执行官马克·扎克伯格昨天在纽约会见了 Foursquare 的联合创始人 T2·丹尼斯·克劳利。第二个消息来源证实，双方最近又在[谈判](https://web.archive.org/web/20230204224320/https://techcrunch.com/2010/04/22/facebook-and-microsoft-check-in-with-foursquare-will-crowley-sell/)(两家公司谈判并不罕见，但时机很有意思)。那么昨天的会面是他们开始正面交锋前的最后一次友好会面吗？巩固合作关系的会议？还有别的吗？我们应该很快就会知道…

![](img/dd0c2fe6ade0010eaf92295d80540436.png "1")

[![](img/0d1c4851ccb51815c23c4fb44fa4c0c4.png "2")](https://web.archive.org/web/20230204224320/https://techcrunch.com/wp-content/uploads/2010/05/2.png)