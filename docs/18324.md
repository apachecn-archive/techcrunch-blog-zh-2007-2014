# 互联网是用泡泡糖和铁丝捆在一起的

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/03/29/the-internet-is-held-together-with-bubble-gum-and-baling-wire/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

你知道吗，引用一个愤怒的黑客的话:

> 从各个角度来看，互联网都是用有缺陷的胶带粘在一起的纸牌屋。任何东西能起作用都是奇迹。那些了解大量相关技术的人通常讨厌它，但同时惊讶地发现，对于最终用户来说，事情似乎通常运行得相当好。

今天，我想谈谈过去几个月互联网上所有令人震惊的安全灾难，但正如伊尼戈·蒙托亚曾经说过的:“不，太多了。我来总结一下。”唉，即使是不完整的总结也是一长串灾难。让我们看看:

那就在网上再呆几个月。但是不要误解我。T2 的情况比名单上看起来的要糟糕得多。

你知道吗[安全下载软件几乎是不可能的](https://web.archive.org/web/20230325153854/https://news.ycombinator.com/item?id=7334269)？你知道支持 https(所谓的“安全”浏览)的证书系统是一个灾难性的烂摊子吗？你知道美国国家安全局——嗯，好吧，我猜你知道。(谢谢 Ed！)但是你知道吗，OpenSSL 被业界广泛用于保护各种类型和规模的应用程序，却被广泛认为是糟糕的代码，令人困惑。

这是为什么呢？在一个到处都有无法破解的加密技术的时代，为什么我们不仅不安全，而且越来越不安全？什么出了这么严重的问题？

好吧。三件事，真的。

**1。安保很难。**

不，真的是。

**2。用户不在乎。**

不，他们真的不知道。互联网上最常见的密码是“123456”和“密码”。他们甚至对最基本的安全卫生都不感兴趣:

…直到他们被黑。然后，当然，他们归咎于技术。

然而，我很遗憾地报告，这种指责并不完全是错误的。因为

**3。安全性通常是事后才想到的。**

不，*如果那个*。因为安全是困难的，而用户是懒惰的，所以即使对普通用户来说，制造安全的系统也要花费太多的时间和精力，所以太多的公司只是草草拼凑一些东西，希望不会出什么大问题。

我听起来像是夸大其词吗？引用几年前的“[世界上最危险的代码](https://web.archive.org/web/20230325153854/https://crypto.stanford.edu/~dabo/pubs/abstracts/ssl-client-bugs.html)”:

> 我们证明了 SSL 证书验证在许多安全关键型应用程序和库中完全失效。易受攻击的软件包括亚马逊的 EC2 Java 库和所有基于它的云客户端；亚马逊和 PayPal 的商家 SDK，负责将支付细节从电子商务网站传输到支付网关；osCommerce、ZenCart、Ubercart、PrestaShop 等综合购物车；手机网站使用的 AdMob 代码；大通手机银行和其他几个安卓应用和库；[等等]。来自这些程序的任何 SSL 连接对于中间人攻击都是不安全的。这些漏洞的根本原因是 SSL 实现的 API 设计不当。

我的朋友 Will Sargent 最近写了一系列博客文章，讲述如何在 Java 中正确启用安全 HTTP 连接。这是一本极好的入门书——但它有数万字长，因为它必须是:

1.  [修复世界上最危险的代码](https://web.archive.org/web/20230325153854/http://tersesystems.com/2014/01/13/fixing-the-most-dangerous-code-in-the-world/)
2.  [固定 X.509 证书](https://web.archive.org/web/20230325153854/http://tersesystems.com/2014/03/20/fixing-x509-certificates/)
3.  [修复证书撤销](https://web.archive.org/web/20230325153854/http://tersesystems.com/2014/03/22/fixing-certificate-revocation/)
4.  [修复主机名验证](https://web.archive.org/web/20230325153854/http://tersesystems.com/2014/03/23/fixing-hostname-verification/)

这太棒了，作为一个我自己在 Android 和 Java 上与 SSL 证书搏斗过的开发人员，我真的很高兴是他写的；但是在一个更好的世界——提醒你，不是一个完美的世界；真的，只是一个非灾难性的错误——他不需要这么做。

当然，信用卡更糟糕。在销售点的目标黑客攻击，本可以通过使用[芯片和引脚](https://web.archive.org/web/20230325153854/http://en.wikipedia.org/wiki/Chip_and_PIN)技术来防止……这种技术在发达世界的其他地方*非常普遍，并且已经在*使用了很多年*。在英国，芯片和 PIN 于 2003 年开始试点，并于 2004 年在全国推广。那是整整十年前的*。但美国的银行和零售商一直拖拖拉拉——现在，直接的结果是，他们是桶里的鱼。**

 *当然，芯片和密码对在线信用卡交易没有帮助，因为:

https://twitter.com/pmarca/status/447654946100375552
https://twitter.com/pmarca/status/447817504652402688

公平地说，我们已经看到了一些朝着正确方向的举措。脸书——它似乎有令人印象深刻的安全性，在一个由黑客领导的公司里也许并不奇怪——上个月发布了一个新工具[来使 Android 应用程序更安全](https://web.archive.org/web/20230325153854/http://arstechnica.com/security/2014/02/facebook-releases-conceal-a-lightweight-tool-to-make-android-apps-safer/)。在[“金发女孩”管理程序级别](https://web.archive.org/web/20230325153854/http://www.wired.com/business/2014/02/casado-vmware-goldilocks-layer/)有一个通用服务器安全平台的说法。美国联邦贸易委员会开始关注并列举违规者，包括 Fandango 和 Credit Karma:

但在一个安全意识淡薄的企业中，这些只是生命中的几个亮点。与此同时，我们正在进行一场军备竞赛，当进攻者在少林寺接受训练并在法国外籍军团获得宝贵的工作经验时，防御者却在懒洋洋地喝着啤酒，因为公爵和公爵夫人们告诉他们排空护城河，支撑城门打开，并丢掉武器和盔甲，这一切都是为了鼓励贸易。我敢肯定，这似乎总是一个非常好的主意…直到有一天成吉思汗骑着马上路。

* * *

(1)对于那些在 GnuTLS 发布之前指责苹果的 ifs-无括号代码风格导致了 bug 的编码人员:

* * *

*形象信用:* [不安全感](https://web.archive.org/web/20230325153854/http://www.insecuritymovie.com/)。*