# 这不是你自以为了解的网络 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/12/17/this-is-not-the-net-you-thought-you-knew/>

你知道互联网是怎么运作的，对吧？你当然知道:你是 TechCrunch 的读者，超级用户。你知道地址栏中的“HTTP”是什么意思(如果你没有使用 Chrome。)你知道在幕后，域名系统会将你对 beta.techcrunch.com 等域名的请求翻译成 76.74.254.121 T2 等数字地址，安全连接由 SSL 加密。你知道网络服务器通过电线(或空气)将 HTML，网络的通用语言*发送到你的电脑，网络开发者编写 JavaScript 来控制你的浏览器用它做什么。*

…除非你实际上是个技术人员。在这种情况下，你可能已经知道上面的描述——姑且称之为经典网络——越来越完全错误。

接下来的内容有点技术性，但请原谅我，我有一个更大的观点。(此外，即使你自己不是技术人员，为了做出明智的决定，你也需要对当今的技术做什么以及如何做有一些了解。)

为什么 Chrome 不再在网址前显示标志性的“http://”?因为它和亚马逊的[屌丝](https://web.archive.org/web/20230110022000/http://www.belshe.com/2011/11/17/spdy-of-the-future-might-blow-your-mind-today/)以及即将推出的[火狐](https://web.archive.org/web/20230110022000/http://www.pingnuts.com/enable-spdy-protocol-support-in-firefox-11/)一样，不一定再用 HTTP 了。相反，在可能的情况下，他们使用谷歌速度更快的替代品 SPDY，它也让服务器将数据推送到浏览器，而不是等待请求。

那个域名系统？这是[越来越](https://web.archive.org/web/20230110022000/http://www.esecurityplanet.com/news/article.php/3929786/com-Domain-Finally-Safe.htm)实际上是 [DNSSEC](https://web.archive.org/web/20230110022000/http://en.wikipedia.org/wiki/Domain_Name_System_Security_Extensions) ，一个防止原始系统中大量安全漏洞的扩展。

你所谓的安全关系呢？嗯，SSL 实际上在一段时间前被 [TLS](https://web.archive.org/web/20230110022000/http://en.wikipedia.org/wiki/Transport_Layer_Security) 取代，修复了一些安全漏洞，但不是最大的:浏览器自动接受来自数百个不同机构的任何网站的安全证书，其中任何一个都可以，而[通常](https://web.archive.org/web/20230110022000/https://www.eff.org/deeplinks/2011/08/iranian-man-middle-attack-against-google) [则](https://web.archive.org/web/20230110022000/http://arstechnica.com/security/news/2011/09/comodo-hacker-i-hacked-diginotar-too-other-cas-breached.ars)被破坏。是的，这太疯狂了。EFF 的主权钥匙倡议可能最终会解决这个问题；在此期间，Chrome 比其他浏览器更安全，因为它允许网站所有者指定哪些证书是可以的。

(我听起来像是在告诉你用 Chrome 吗？不完全是。我主要使用 Firefox，因为 Chrome [不支持](https://web.archive.org/web/20230110022000/http://forums.informaction.com/viewtopic.php?f=8&t=7475)任何等同于 Firefox 的增强安全性和健全性的 [NoScript 插件](https://web.archive.org/web/20230110022000/https://addons.mozilla.org/en-US/firefox/addon/noscript/)，并且可能永远不会支持。)

至于 JavaScript——当然，所有的浏览器*都运行*它，但是几乎没有开发者*再编写纯粹的 JavaScript 了。相反，我们使用像 jQuery 这样的库框架，它已经或多或少地征服了世界，或者使用更高级的语言，像 CoffeeScript(我不喜欢它，因为这些和其他原因)或者甚至是谷歌有争议的新语言 Dart，它编译成并最终打算取代 JavaScript。[可惜](https://web.archive.org/web/20230110022000/http://blogs.perl.org/users/rafael_garcia-suarez/2011/10/why-dart-is-not-the-language-of-the-future.html)，几乎[没有](https://web.archive.org/web/20230110022000/http://siliconangle.com/blog/2011/10/10/googles-dart-programming-language-disappoints-hackers/) [一个](https://web.archive.org/web/20230110022000/http://arstechnica.com/business/news/2011/10/javascript-has-problems-can-googles-dart-solve-them.ars/3) [之外的谷歌](https://web.archive.org/web/20230110022000/http://en.wikipedia.org/wiki/Dart_%28programming_language%29#Competitive_landscape)好像都喜欢。*

为谷歌辩护的是，他们新的服务器端语言 [Go](https://web.archive.org/web/20230110022000/http://en.wikipedia.org/wiki/Go_%28programming_language%29) 广受赞誉——尽管具有讽刺意味的是，它明显没有通过“你的语言的名称使得它不可能在谷歌上找到”[测试](https://web.archive.org/web/20230110022000/http://colinm.org/language_checklist.html)——而且他们的[本地客户端](https://web.archive.org/web/20230110022000/http://googlecode.blogspot.com/2011/08/native-client-brings-sandboxed-native.html)技术[强大而有趣](https://web.archive.org/web/20230110022000/http://googlecode.blogspot.com/2011/12/games-apps-and-runtimes-come-to-native.html)。唉，我看不到任何其他浏览器支持它。

但是说到底，你的浏览器还是大部分在获取和渲染 HTML，对吧？不要这么肯定。首先，“香草”HTML 在普通网页中所占的比例越来越小。另一方面，越来越多的 HTML5，[不管那是什么意思](https://web.archive.org/web/20230110022000/http://en.wikipedia.org/wiki/Comparison_of_layout_engines_%28HTML5%29#Attributes)。

此外，有一个有趣的趋势是 web 服务器根本不提供 HTML。战地 3 的“战斗日志”网站是客户端和服务器之间的纯 JSON。我以前的同事迈克尔·戴克曼(他的同事通常会无缘无故地在他的名字后面加上“有史以来最伟大的程序员”)开发了一个纯 XML/XSLT web 框架， [Gossamer](https://web.archive.org/web/20230110022000/http://code.google.com/p/gossamer-web/) :正如它的[介绍性的咆哮](https://web.archive.org/web/20230110022000/http://code.google.com/p/dexter-xsl/wiki/CaseForXSL)所说，“如果我们能够以 web 服务模型提供的同样简单优雅的方式处理来自 web 浏览器的页面请求，那不是很好吗？

传统的网络开始看起来像一个杂牌。主要是因为它是。慢慢地，断断续续地，向前三步-向后两步，技术社区最终将其改进成更安全、更精简和更强大的东西。上一次类似的事情发生在 AJAX 支持冲击现代浏览器的时候。非技术人员没有意识到这一点，但正是这一创新带来了 Flickr、谷歌地图和整个 Web 2.0 热潮。我希望 html 5——在我上面列举的鲜为人知的后端迭代的极大帮助下——对网络和我们在那里做的一切产生类似的影响。

也许包括*预言已久的应用帝国的衰亡。但是在下周的专栏中会有更多的内容…*

 ****下面评论者澄清的几点:*** 好吧，所以没有真正的证据表明 Chrome 地址栏删除 HTTP 实际上与它使用 SPDY 有关。上面的“完全没有 HTML”太极端了:“没有动态生成的 HTML”会更好，因为第一次页面加载仍然是 HTML。

***我澄清的几点:*** 人们可以并且确实在一定程度上争论“纯”和“普通”JavaScript 之间的语义区别，但是我相当自信地认为，用 jQuery 编写的 JS 在内容和方法上与“纯/普通”JS 有本质的不同。据我所知，Chrome 的 NotScript 并不是 Firefox 的 NoScript 的替代品，因为它只是屏蔽了 JS，而不是逐个站点地剥离 JS:唉，我找不到详细的技术分析来比较当前版本的内部工作方式。

*图片致谢* : QbiT， [Flickr](https://web.archive.org/web/20230110022000/http://www.flickr.com/photos/fredo/372477459/) 。*