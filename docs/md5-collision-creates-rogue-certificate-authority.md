# MD5 冲突创建流氓证书颁发机构

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/12/30/md5-collision-creates-rogue-certificate-authority/>

![scene from Sneakers](img/56f86bab19e47ea0cc6174c46d48ad55.png "scene from Sneakers")

在今天的第 25 届混沌通信大会 (CCC)上，研究人员将揭示他们是如何利用针对 MD5 算法的碰撞攻击来创建一个流氓认证机构的。这是一个相当大的新闻，所以请继续阅读。

当你通过 HTTPS 安全连接到一个网站时，一个[公钥证书](https://web.archive.org/web/20230320170114/http://en.wikipedia.org/wiki/Public_key_certificate)会从服务器发送到你的电脑。此证书包含一个数字签名，您的计算机用它来验证您正在连接的站点的身份。证书是由一个[证书颁发机构](https://web.archive.org/web/20230320170114/http://en.wikipedia.org/wiki/Certificate_authority) (CA)来“签名”的，它充当了一种中间人的角色:您信任 CA，所以您也可以信任由 CA 签名的证书。但是，任何人都可以创建证书颁发机构，所以大多数浏览器都有一个已知的信誉良好且值得信赖的证书颁发机构列表。当您的计算机从服务器获取证书时，您的浏览器会检查颁发该证书的 CA，以确定该 CA 是否可信。如果 CA 是可信任的，您的浏览器会认为所提供的证书是可信任的。

认证机构使用的[公钥加密](https://web.archive.org/web/20230320170114/http://en.wikipedia.org/wiki/Public_key_cryptography)正在发展，就像技术世界中的大多数事物一样。一些 ca 使用 [MD5](https://web.archive.org/web/20230320170114/http://en.wikipedia.org/wiki/MD5) 算法来计算证书的数字签名。众所周知，MD5 很难抵御[碰撞攻击](https://web.archive.org/web/20230320170114/http://en.wikipedia.org/wiki/Collision_attack)，但是运行 CA 是一个非常复杂的操作，所以它们背后的实体变化很慢。

研究人员使用 200 个 PlayStation 3 系统攻击了 MD5 算法，并能够构建一个看起来像已知可信 CA 的伪造证书颁发机构。这意味着这些家伙可以为 www.amazon.com 生成一个证书，当它出现在你的浏览器上时，会被接受为真实的东西。假证书上的数字签名被列为来自一个据称信誉良好的 CA，因此您的浏览器愉快地接受它，并放心地向您显示小挂锁图标。

![rouge CA attack diagram](img/9a7f56909d5d80b5fca9f6330107c1be.png "rouge CA attack diagram")

好吧，那这对你有什么影响？如果研究人员的结果可以被恶意代理复制，他们可以生成任何数量的证书，被世界各地的浏览器所信任。仅此可能就足够了，尽管这种攻击可能会与复杂的 DNS 攻击结合起来，让任何人都很难意识到他们被骗了。你的浏览器会报告你在 yourbank.com；你的浏览器会报告你使用 HTTPS 来保护连接；您的浏览器会报告用于 HTTPS 连接的 SSL 证书确实属于 yourbank.com。诚然，进行这样一次攻击所需的努力程度目前是巨大的，潜在的收益可能是有限的，所以这可能不是普通互联网用户会做的那种事情。但这仍然是值得关注的事情。

[攻击大纲](https://web.archive.org/web/20230320170114/http://events.ccc.de/congress/2008/Fahrplan/attachments/1251_md5-collisions-1.0.pdf)指出“通过优化，在亚马逊 EC2 上花费 2000 美元的攻击可以在一天内完成。”谢天谢地，研究人员没有公布他们的具体实现。这多少让人放心，但期待某些地方的纵容者为了不那么学术的目的而试图重现研究人员的结果。

PDF 的结论是:“没有必要恐慌，互联网并没有完全崩溃”，并向我们保证“受影响的 ca 正在转向 SHA-1”。SHA-1 被认为对某些攻击很弱，所以对易受攻击的 CAs 来说直接跳到 SHA-2 或 SHA-3 可能更好。

底线:一如既往，要认识到你的浏览习惯。如果事情看起来或感觉可疑，不要提供任何帐户名或密码。对不同的网站使用不同的密码，这样如果你被网络钓鱼欺骗了，网络钓鱼者就不会得到你的网络王国的钥匙。

链接: [25C3: MD5 今日被认为有害](https://web.archive.org/web/20230320170114/http://events.ccc.de/congress/2008/Fahrplan/track/Hacking/3023.en.html)
Via: [ZDnet](https://web.archive.org/web/20230320170114/http://blogs.zdnet.com/security/?p=2339)