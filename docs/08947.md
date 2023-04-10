# HTML5 移动应用框架 PhoneGap 添加脸书连接插件 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/30/html5-mobile-app-framework-phonegap-adds-facebook-connect-plugin/>

# HTML5 移动应用框架 PhoneGap 添加脸书连接插件

基于 HTML5 的移动应用框架 [PhoneGap](https://web.archive.org/web/20230203103216/http://www.phonegap.com/) 的创造者 Nitobi 今天发布了 [PhoneGap 脸书连接插件](https://web.archive.org/web/20230203103216/https://github.com/davejohnson/phonegap-plugin-facebook-connect)。插件的加入意味着使用 HTML 和 JavaScript 等 Web 技术开发应用程序的开发者现在可以通过允许用户使用他们的脸书凭据登录来简化他们应用程序的登录过程。

为了使第三方能够集成脸书连接技术，脸书向开发者提供了一个 JavaScript 软件开发工具包(SDK)。

然而，Nitobi 说使用脸书 SDK 是一个挑战，因为它要求[使用 OAuth 2.0 标准](https://web.archive.org/web/20230203103216/https://developers.facebook.com/docs/authentication/)，一个开放的授权标准。该公司发现，这种登录过程并不总能很好地适用于 PhoneGap 开发者的应用。通常，用户的屏幕上会弹出一个登录框，因为他们的脸书用户名和密码凭证不太可能存储在设备上。

Nitobi Inc .的首席技术官 Dave Johnson 说:“我们开始开发脸书插件，因为我们提倡用户体验。“移动应用的 OAuth 认证工作流程并不理想，因此我们创建了 PhoneGap 脸书连接插件，作为简化该流程并改善最终用户体验的一种方式。”

新插件使用与脸书自己的 SDK 相同的 API(应用程序编程接口),但它不是复制你在网上看到的使用桌面浏览器的相同工作流程，而是与安装在用户自己设备上的原生脸书应用程序一起工作。最终结果是，应用程序的最终用户登录过程变得不那么繁琐。

这个插件现在已经可以从 Gitub 这里下载了。

Nitobi 现在每月有超过 40，000 次 PhoneGap 下载，它说它预计这个新插件会很受欢迎。