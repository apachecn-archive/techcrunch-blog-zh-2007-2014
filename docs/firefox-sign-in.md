# Mozilla 将登录按钮引入浏览器级别 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/12/firefox-sign-in/>

如果您在使用帐户的网站上，登录按钮可以在任何地方。当然，有一些常见的最佳实践，但我可以想到许多网站都有这些实践。Mozilla 正试图解决这个问题，将这个标志引入浏览器层面。

Mozilla 为 Firefox 发布的一个新的实验性扩展就是这样做的。安装后，你会在 URL 框的左边看到一个新的“登录”按钮。点击这个，弹出一个窗口，提示你输入你所在网站的用户名和密码。然后，当你登录到一个网站时，它会显示给你，并给你一个点击退出的能力。简单。简单。很好。

当然，你所在的网站必须支持这种功能。但是 Mozilla 让这变得很容易，因为他们在关于这个主题的帖子中概述了[。最好的一点是，它可以用于任何类型的登录——可以是广泛的登录，如 OpenID，也可以是特定的登录，如博客，甚至脸书、Twitter 等——同样，如果这些网站实现了这样的功能。](https://web.archive.org/web/20230203082633/http://identity.mozilla.com/post/8841090082/sign-into-websites-directly-from-your-browser)

有一点很重要:

> 值得注意的是，该功能不与任何服务器端组件通信，也不捕获、存储或传输任何个人信息。该按钮在语义上与在页面上单击“登录”相同:它只是告诉页面您现在想要登录(或退出)。

本质上，Mozilla 只是在浏览器 chrome 中为登录按钮创建了一个公共位置。尽管他们也指出，如果网站也开启了 cookies 功能，它也将支持 cookies。

虽然这是开放给任何网站/服务使用的，但它也是另一个 Mozilla 项目的扩展:BrowserID。正如他们[上个月在这里宣布](https://web.archive.org/web/20230203082633/http://identity.mozilla.com/post/7616727542/introducing-browserid-a-better-way-to-sign-in)的那样，他们对这种新的网络识别系统的想法类似于 OpenID 之类的东西，它从未真正流行起来(Mozilla 也[说](https://web.archive.org/web/20230203082633/http://identity.mozilla.com/post/7669886219/how-browserid-differs-from-openid)它更安全和无缝)。Mozilla 正试图从更高的层面重新思考网络身份识别。

除了 BrowserID(反正是个开放技术)，Mozilla 在这个游戏里没有任何真正的皮肤。但是他们的一些竞争对手可以。例如，谷歌正在为他们的 Chrome 浏览器实现登录体验。这已经在 Sync 上运行了，但谷歌也在为 Chrome 开发配置文件。在浏览器级别登录也允许你登录谷歌网站，这对于 Chrome 操作系统来说很关键。

与此同时，脸书[一直在与 RockMelt](https://web.archive.org/web/20230203082633/https://techcrunch.com/2011/06/14/facebook-rockmelt/) 合作，开发该浏览器的脸书登录体验(巧合的是，该浏览器也基于 Chromium)。

从更广的层面来看，谷歌和脸书都已经对这种总是登录的体验思考了很多。这一点在手机上尤其重要，在手机上反复输入用户名和密码会更烦人。这一点，加上对成为网络中心身份的关注，导致了像脸书的[单点登录](https://web.archive.org/web/20230203082633/https://techcrunch.com/2010/11/03/facebook-single-sign-on/)这样的项目。

因此，尽管 Mozilla 在这方面可能有着高尚的意图，但我仍然怀疑我们会从他们不那么高尚的竞争对手那里看到更多类似的东西。这并不是说他们是邪恶的，只是出于更自私的原因。谷歌已经有了他们的浏览器。我敢打赌，脸书迟早会有一个。这可能对 Mozilla 有所帮助，因为它们最终可能成为真正开放的选择。

[YouTube http://www.youtube.com/watch?v=UHWXoFD81Gs&w=640&h=449]