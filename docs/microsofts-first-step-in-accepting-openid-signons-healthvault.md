# 微软接受 OpenID 登录的第一步——health vault TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/06/23/microsofts-first-step-in-accepting-openid-signons-healthvault/>

# 微软接受 OpenID 登录的第一步——health vault

![](img/920d4483457cd590dd0630ba3ab5f35a.png)

在第一次[宣布](https://web.archive.org/web/20221209120958/http://blog.wired.com/27bstroke6/2007/02/microsoft_to_su.html)支持 [OpenID](https://web.archive.org/web/20221209120958/http://www.openid.net/) 认证平台超过 16 个月后，微软终于第一次实现了这一点，允许 OpenID 登录其 [Health Vault](https://web.archive.org/web/20221209120958/http://www.healthvault.com/) 医疗网站。不幸的是，Health Vault 将只支持来自两个 OpenID 提供者的认证: [Trustbearer](https://web.archive.org/web/20221209120958/http://www.trustbearer.com/) 和 [Verisign](https://web.archive.org/web/20221209120958/http://www.verisign.com/) 。OpenID 中的*打开*到底怎么了？

有限引入背后的基本原理是，健康是敏感的，因此访问应该限于少数最受信任的 OpenID 提供者。这当然有道理，但它也强调了 OpenID 固有的一个问题:安全性。

分散在网络上的基于文本的密码并不能很好地起到保护作用。我们听过无数关于黑客或网络钓鱼密码导致身份盗窃的故事——当用户的整个网络(包括财务和健康数据)都与一个密码相关联时会发生什么？这是导致灾难的原因。

为了解决这个问题，许多公司想出了不同的方法来提高安全性。 [Trustbearer](https://web.archive.org/web/20221209120958/http://openid.trustbearer.com/) 要求用户提供一个物理 ID“令牌”来验证他们的身份(如果用户还没有一个可接受的 ID 卡，可以订购一个 40 美元的 u 盘)。 [Vidoop](https://web.archive.org/web/20221209120958/http://www.vidoop.com/) 提供免费的基于浏览器的图像认证系统，利用广告创收。诸如此类。

每一项新的安全措施都会带来新的、主观的系统分层。OpenID 的承诺是一个“消除跨不同网站的多个用户名的需要，简化您的在线体验”的平台。但是通过只接受“安全的”OpenID 提供者，微软已经证明了这个系统在它当前的形式下绝不是统一的。很快，用户将需要记住他们的“安全”OpenID，以及他们的“正常”凭证。当另一个提供商提供一个“超级安全”的 ID，强迫用户记住另一个登录时会发生什么？

除了微软之外，还有许多公司可能会因为 OpenID 实施缓慢或不佳而受到批评——谷歌已经通过其 T2 博主 T3 地产成为 OpenID 提供商，但尚未在其任何旗舰服务上实施该平台。但似乎这个平台本身更值得关注。当统一登录的默认形式只在最不私密和安全的网站上被接受时，它有什么用？