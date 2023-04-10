# 终于！Bitcasa 首席执行官解释加密的工作原理 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/09/18/bitcasa-explains-encryption/>

TechCrunch Disrupt 决赛入围者 [Bitcasa](https://web.archive.org/web/20230205021323/http://www.bitcasa.com/) ，一家新的云存储提供商，上周[宣称能够提供“无限存储”时，遭到了适度的质疑它是怎么做到的？它做不到承诺的事！加密不是这样工作的！诸如此类。风险投资公司安德森·霍洛维茨(Andreessen Horowitz)以及首轮资本(First Round Capital)、Pelion Venture Partners 和 TechCrunch 创始人迈克尔·阿灵顿的 CrunchFund 已经在这项技术上投资了 130 万美元，这似乎表明，这家初创公司过于宽泛的廉价、无限和安全存储承诺背后有宝贵的知识产权。](https://web.archive.org/web/20230205021323/https://techcrunch.com/2011/09/12/with-bitcasa-the-entire-cloud-is-your-hard-drive-for-only-10-per-month/)

我在[对这家初创公司的最初评价](https://web.archive.org/web/20230205021323/https://techcrunch.com/2011/09/12/with-bitcasa-the-entire-cloud-is-your-hard-drive-for-only-10-per-month/)总体上是积极的，因为从各方面来看，它正在做一些创新和新的事情。我们提出了一些一般性的问题(这会让你慢下来吗？，它会扩展吗？)，不去动手很难复习到东西。就此而言，描述这项技术的工作方式可能过于简化了。对于那些对更深层次的技术细节感兴趣的人来说，它们就在这里(好吧，至少这是一个开始……)。

作为决赛选手，比特卡萨接受了包括罗恩·康韦、哈迪·帕托维、玛丽莎·梅耶、罗洛夫·博塔、马修·科勒和阿林顿在内的知识渊博的评委的训练。

哈迪·帕托维是“告诉我”和“我喜欢”的创始团队成员。作为天使投资人和创业顾问，哈迪的投资组合包括[脸书](https://web.archive.org/web/20230205021323/http://www.crunchbase.com/company/facebook)、 [Zappos](https://web.archive.org/web/20230205021323/http://www.crunchbase.com/company/zappos) 、 [Dropbox](https://web.archive.org/web/20230205021323/http://www.crunchbase.com/company/dropbox) 、 [OPOWER](https://web.archive.org/web/20230205021323/http://www.crunchbase.com/company/opower) 、 [Flixster](https://web.archive.org/web/20230205021323/http://www.crunchbase.com/company/flixster) 、 [Bluekai](https://web.archive.org/web/20230205021323/http://www.crunchbase.com/company/bluekai) 等众多。

像你一样，他想知道 Bitcasa 的加密是如何工作的。

要了解 Bitcasa 首席执行官托尼·高达是如何回答这些问题的，请滚动至帖子底部视频的第 11:48 分钟。但他的主要解释是，Bitcasa 利用了一种称为收敛加密的技术，他在被切断之前对这种技术进行了解释。

这是谈话相关部分的记录。

*T3【惠普】T4:您在加密或安全方面做什么？*

***TG** :我们对客户端的所有内容进行加密。我们对所有数据使用 AES-256 哈希、SHA-256 哈希。*

***惠普**:所以所有的数据都在客户端加密了，你不能在服务器端查看吗？*

***TG** :没错。*

***惠普**:如果我上传一个文件，玛丽莎上传同一个文件，你会存储这个文件的两个不同副本还是一个？*

***TG** :不，我们在服务器端进行重复数据消除。所以我们实际上在服务器端确定它是否在那里，如果它已经在那里，我们就不用再上传它了。*

***HP** :但如果加密了又没有钥匙，该怎么做呢？*

***TG** :有一篇学术论文叫做收敛加密。这实际上是加密社区中已知多年的事情。但是我们实际上做的是…我们没有按照你认为的方式加密它…还有其他方法可以做到。*

***气血，诡异一瞥**:好。*

*(观众笑声)。)*

保罗·卡尔(保罗·卡尔)( T42 ):我想观众会想知道更多关于这个的信息……这是什么意思？

***TG** : OK，所以收敛加密…当你加密数据时，我有一把钥匙，你也有一把钥匙。假设这些完全不同。假设我们都有相同的文件。我用我的钥匙加密，你用你的钥匙加密。现在数据看起来完全不同，因为加密密钥不同。那么，如果您实际上是从数据本身获取密钥，会发生什么呢？现在，我们都拥有完全相同的加密密钥，可以在服务器端进行重复数据消除。*

*(麦克风在最后会变得很响)。*

***TG** :看看有多强大？太强大了！*

*(观众笑)。*

***TG** :这是收敛加密。这不是我们发明的。我们发明了各种各样的东西来让这个东西变得令人敬畏。有很多关于“嘿，你怎么做到的？”巨魔们将会出现在 Slashdot 上……*

*保罗·卡尔好了，停止投球。*