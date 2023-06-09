# 一个女人、一个纸杯蛋糕、一家银行和一个广场:为什么信用卡公司害怕变革

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/22/a-woman-a-cupcake-a-bank-and-a-square-why-credit-card-companies-are-scared-of-change/>

在俄亥俄州昏昏欲睡的哥伦布郊区，运河温彻斯特有一家制作纸杯蛋糕的商店。这些不是普通的纸杯蛋糕；这些蛋糕太棒了。事实上，这家店的名字——[梦幻纸杯蛋糕](https://web.archive.org/web/20230205035241/http://fantasycupcake.com/)——并不是吹嘘，可以很容易地支持炒作(相信我，我吃过一个，非常好吃)。Fantasy Cupcake 是由 Leah Dotson 拥有和运营的一家相对较新的企业，在建立接受信用卡的交易机制时，它选择了[广场](https://web.archive.org/web/20230205035241/https://squareup.com/)作为其处理器。

然后有趣的事情发生了。不知是不是巧合，几家银行和加工商与 Leah 接洽，希望与他们一起建立商户服务，而不是依赖 Square。

大多数来访的商家服务代表看了 Leah 制定的 Square 费率计划，承认她做了一笔好交易，事实上，Square 将是她的最佳选择。

但是有两次进行得不太顺利。

一家主要银行的代表拿着一份报价和一份传单走了进来——“如果我们不能超过你目前的商业利率，我们会给你 300 美元，另外给你 100 美元让你转用我们的服务。”Leah 告诉销售代表她的平方费率(2.75% +没有额外费用)，她说主要的银行销售代表“有点慌”，然后可笑地尽快离开了(留下了一张传单，但留下了 300 smackeroos)。搞笑。

[第一数据](https://web.archive.org/web/20230205035241/http://www.firstdata.com/en_us/home.html)代表？这就是奇怪的地方。那位代表(实际上是亨廷顿银行的代表)给了她一堆关于 Square 的信息(实际上是错误的信息)，并建议她转到第一数据/亨廷顿服务公司，以保护自己。虽然 Leah 认为她很专业，但她承认大量关于 Square 的负面信息并没有让她感到害怕。事实上，这让她非常害怕…足以打电话给她姐夫，他首先帮助她建立了 Square(他也是一名支付专家)。我就是这样得到风声的。

那么这个错误信息是什么呢？第一位数据代表向 Leah 指出:

*   Square 未加密
*   Square 将信用卡信息存储在她使用的原生 iPad 应用程序中
*   Square 与 [PCI 不兼容](https://web.archive.org/web/20230205035241/http://en.wikipedia.org/wiki/Payment_Card_Industry_Data_Security_Standard)
*   商家可能会因为使用它而被起诉

第一个数据代表试图向她推销他们的商业服务程序，尽管它对 Leah 的大部分业务——小额采购不太友好。

明细比较如下:

![](img/79b2325f4d8c7512ab57cc883c8eb87e.png "FDrate")

![](img/85affcbff61d641d8ff73128dba93068.png "squareRate")

最终，Leah 与 Square 简单的 2.75%费率结构和无额外费用相比，第一份数据商户协议的额外费用约为每年 800 美元。忘记 POS 硬件购买和声明费用，只考虑 0.15 美元的交易费用。这是每笔交易的 1.2%加 0.15 美元，而 Square 的统一费率为 2.7%。当你考虑到 Leah 的大部分销售额都在 3 美元以下的事实时，它真的增加了。相对于使用 Square 的 0.08 美元，3.00 美元订单的费用约为 0.21 美元。

那么关于 Square 的所有加密和 PCI 合规性声明呢？如果这是真的，这足以让任何人有第二个想法。

我联系了 First Data 进行评论，但他们不愿对 Square 发表评论，也不知道他们的代表是否向 Leah 表明了这一点。

所以我联系了 Square。他们的发言人没有告诉我更多细节，但表示没有任何卡号、磁条数据或安全码数据存储在任何授权使用 Square 服务的设备上。她还说，Square 的服务是 100% PCI 兼容的，所有通过的数据都是加密的，超过了要求。然后她发给我一个[链接，链接到他们的安全页面](https://web.archive.org/web/20230205035241/https://help.squareup.com/customer/portal/articles/7764-security-and-data-encryption-)。

但是真正的读者呢——可以说是广场。加密了吗？技术上来说不是。几个月前我采访 App Ninja 的首席执行官约翰·沃尔德伦时，他说了很多。我向[墨卡托咨询集团](https://web.archive.org/web/20230205035241/http://www.mercatoradvisorygroup.com/index.php?doc=team)新兴技术咨询服务总监乔治·皮博迪证实了这一点。乔治告诉我，Square reader 实际上是一个非常有效的卡套，有流氓应用程序可以这样使用它。公平地说，如果你去寻找一个套卡器，套卡器是很容易得到的，而且还有比滥用方块更复杂和隐蔽的方法来检索卡信息(还记得不久前[这个戏剧性的故事](https://web.archive.org/web/20230205035241/http://www.wreg.com/news/wreg-electronic-pickpocketing-story,0,5636726,full.story))吗？

**这一切意味着什么**

因此，Square 实际上是一个加密的软件解决方案，符合 PCI 合规性的规则，它不会在使用它的设备上存储任何数据。这是一个接受信用卡的安全解决方案，因此第一个与 Leah Dotson 交谈的 Data/Huntington 代表是错误的。然而，根据人们如何定义加密，Square 不使用硬件加密的说法目前实际上是正确的。但实际上，在数据到达 Square 的软件之前，很难拦截在 Square 读卡器上刷过的卡数据。更有可能促进这种浏览的方式是，狡猾的商家在他们越狱或未经授权的移动设备上使用流氓应用程序，代替 Square 的软件来收集卡数据。但是，一个人劫持一个正方形阅读器来浏览卡片，可以很容易地操纵另一个解决方案来做同样的事情。所以一个消费者真正应该问的问题不是*“这个商家是不是在用 Square”*，而是*“等等，首先这个商家是谁？它们是否成立、合法，我还能再找到它们吗？”*

但是回到我们的小戏剧。一家公司试图利用错误信息来争夺业务，这当然不足为奇——这在当代商业世界中是正常的。让我有点震惊的是，这一行动可能意味着什么。无论是否得到公司的批准，像这样的行动是否表明大银行/加工商有点害怕 Square？一年前，Square 似乎还处于大银行的边缘，但实际上，它所代表的威胁比之前想象的要大一些。也许光是每年损失 800 美元费用的威胁就足以让一些加工商和银行有点紧张了？

这听起来像是经典的大卫对抗歌利亚的故事，对吗？像 First Data 这样的“大家伙”处理器，甚至像银行这样的地区性参与者都开始有点恐慌，这种机构恐惧正在蔓延到他们商业服务销售计划的所有领域——这是一个合乎逻辑的结论，对吗？

嗯……可能不会。

首先，我们来客观看待成交量。Square 每天完成 400 万美元的交易。这听起来很多，但请记住，像 Chase Paymentech(First Data 最大的国际竞争对手之一)这样的处理器在 Q2 2011 年实现了大约 1370 亿美元的交易额[。这相当于每天 15 亿美元，轻松超越 Square 的交易量。第一个数据的量似乎差不多。](https://web.archive.org/web/20230205035241/http://www.paymentsnews.com/2011/07/jpmorgan-chase-card-services-2q2011-financial-results.html)

这样的体量差异意味着，从制度上来说，Square 可能根本不在 First Data 的关注范围内。他们是围绕第一数据公司众多九头蛇之一飞行的小昆虫。不，这个故事与其说是大卫对抗歌利亚，不如说是大卫对抗大卫。

啊？

你可能知道支付领域非常复杂。至少在美国，关于商业账户有如此多的参与者和如此多的关系，至少可以说，从宏观角度来看这是令人生畏的。然而，你可能知道也可能不知道的是，像 First Data 和 Paymentech 这样的主要加工企业通常不会为较小的夫妻店设立商户账户，即使这些交易在他们的轨道上进行。与这些大公司之一直接做生意是可能的，但这很昂贵，所以你自己也必须是一家大公司才能与他们合作。对于小型零售商来说，商家账户通常是由独立销售组织(ISOs)设立的，这些组织隶属于大型加工企业，专门为小型企业销售和设立支付和商家账户。这些可能是银行，但也可能是小型专业企业。这个 ISO 基础设施的视野是广阔的，我并不假装是这方面的专家。为了快速总结这些 iso 与大型支付处理商的关系，我再次向乔治·皮博迪寻求解释。

> “这真的是一个销售渠道……一个世界上第一批数据和付费用户拥有的巨大处理能力的销售渠道……你必须站在街上才能销售它。美国大约有 800 万传统意义上的商户，其中绝大多数都希望能够使用信用卡，因为使用信用卡对他们的收入有很大影响。所以这是一个倒卖加工能力的链条。一些[ISO]经销商是银行。有大的 iso 和小的 iso，甚至有独立的销售人员为 iso 工作，实际上是向夫妻店销售产品。”

因此，我的理论解释了为什么这位第一数据代表(可能作为 ISO 工作或与 ISO 合作)会错误地告诉 Leah Dotson，如果她使用 Square 处理她的卡交易，她可能会被起诉。Square 不是与支付处理领域的大公司竞争，而是与这些较小的 iso 和独立代表竞争，他们希望每年获得 800 美元的额外交易相关费用。Square 正在打破这种销售模式，并引起 ISOs 的注意，变得更具竞争力。我向乔治·皮博迪提出了这个想法，他表示同意。“这是典型的互联网去中介化”，事实上，小型和大型的 iso 都可能开始感受到压力，至少会注意到 Square 及其颠覆性的服务。

所以 Square 是赢家，对吗？他们以低得多的管理费用和没有“现场”销售人员的运营服务占据高地？

也许吧，但有一件事是肯定的，他们仍然需要比每天 400 万美元多得多的交易量才能获得立足点。信贷利润率很低，这肯定是一场交易量游戏。支付的标准基础设施仍然是嵌入式的。

我还认为，他们最终将不得不解决“硬件加密”问题。

咻。想到这出戏，我胃口大开。一个纸杯蛋糕肯定能减轻我的痛苦。也许我应该开车去运河温彻斯特吃点安全的小吃。我会确保带上我的信用卡。

[![](img/23652c2950c67383a90b1f429b72def2.png "cupcake2")](https://web.archive.org/web/20230205035241/https://techcrunch.com/wp-content/uploads/2011/08/cupcake2.jpg)