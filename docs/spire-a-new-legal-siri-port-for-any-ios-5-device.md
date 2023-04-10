# Spire:任何 iOS 5 设备的新合法 Siri 端口

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/12/27/spire-a-new-legal-siri-port-for-any-ios-5-device/>

知名 iOS 黑客 [chpwn](https://web.archive.org/web/20230404105446/https://twitter.com/#!/chpwn) (又名格兰特·保罗)与[瑞安·彼得里奇](https://web.archive.org/web/20230404105446/http://rpetri.ch/)一起[发布了](https://web.archive.org/web/20230404105446/http://blog.chpwn.com/post/14689740472)一款在越狱手机上安装 Siri 的新工具。Siri 端口名为“Spire”，可以在任何可以运行 iOS 5 的手机上工作。然而，由于苹果只正式支持来自 iPhone 4S 的 Siri 请求，代理服务器地址仍然是必需的。

哦，还有一件事:尖顶是合法的。

虽然技术上可以在非 iPhone 4S 设备上运行 Siri，[正如之前的 Siri 端口所显示的](https://web.archive.org/web/20230404105446/https://techcrunch.com/2011/12/05/dont-do-it-new-siri-port-h1siri-is-illegal-breaks-your-iphone/)，这些端口侵犯了苹果的版权。Siri 的资源文件、图像和代码并不意味着被复制和广泛传播。所以取而代之的是，Spire 直接从苹果下载 Siri 本身。聪明！

一旦 100 MB 的下载被安装在越狱设备上，用户就必须用代理服务器地址配置软件。保罗通过 Spire Proxy FAQ 解释道，“苹果已经让(Siri 的)授权要求变得不可能了。我对它进行了逆向工程，如果没有来自 iPhone 4S 的信息，似乎不可能将 Siri 连接到云端。”

记住，黑客不会经常抛出“不可能”这样的字眼。显然，苹果已经为管理 Siri 请求准备了一些重型安全措施。

那么，如何获得 Siri 的代理地址呢？保罗建议你可以向一个拥有 iPhone 4S 的朋友索要他们的认证令牌。但更有趣的是，他推测，我们很快就会看到付费的 Siri 代理服务，为访问安装在他们自己的 iPhone 4S 设备上的 Siri 副本收取月费。

第三种可能性——也是黑客社区必须建立的一种可能性——是挖出 Siri 的内脏，换成谷歌 Chrome 的[语音“API”](https://web.archive.org/web/20230404105446/http://src.chromium.org/viewvc/chrome/trunk/src/content/browser/speech/)来解码 Siri 请求并返回结果。

换句话说，截至目前，Spire 是合法实现 Siri 端口的良好开端，但在合法 Siri 代理解决方案出现之前，人们很难真正使用它。

Spire 现在可以在越狱应用商店 Cydia 中获得。