# 比特币交易所 Mt. Gox 是怎么回事？TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/02/10/whats-going-on-with-bitcoin-exchange-mt-gox/>

比特币最初的交易网站之一 Mt. Gox 已经关闭了其提款系统，理由是与[交易延展性](https://web.archive.org/web/20221015160530/http://en.bitcoin.it/wiki/Transaction_Malleability)有关的问题(稍后会有更多内容)。

Mt. Gox [在他们的网站](https://web.archive.org/web/20221015160530/https://www.mtgox.com/press_release_20140210.html)上写道，这个问题已经迫使他们关闭了取款服务:

“我们对突然接到通知表示歉意。所有比特币提款请求将暂停，系统中的提款将返回到您的 Mt Gox 钱包中，并可在问题解决后重新启动。”

发生了什么事？

简而言之，Mt. Gox 一直在遭受一种黑客攻击，这种攻击使其交易消失，让受害的客户回来再次要求他们的钱。然而，事实上，这些消失的交易得到了适当的处理，客户得到了两次付款。

简单解释一下，交易可延展性意味着交易——例如，从 Mt. Gox 发送给用户 A 的 1 个比特币——可以被更改，这样 Mt. Gox 就无法跟踪到转账的发生。目前的转账被添加到区块链，所有比特币交易的分类账，用户 A 获得 BTC。BTC 转移实际上是数据链，可以追溯到有问题的最初硬币的“诞生”每个交易都有自己的 ID 或散列，它基于交易内部的数据，在大多数情况下是接收方和发送方。这些 id 是唯一的。

叛离节点可以修改事务，只要它看到某些数据通过网络。这个修改后的事务仍然说 Mt. Gox 发送给用户 A 1 BTC，仍然是一个有效的传输，但是有一个完全不同的散列。这个新的、修改后的事务实质上取消了以前的事务(如果叛离节点足够快地将其数据传播到确认节点)，Mt. Gox 没有任何方法来证明事务发生过，因为它是基于散列记录事务的。用户 A 回到 Mt. Gox，抱怨他们没有得到他们的现金，交易所没有追索权，只能发送另一笔付款…又一笔…又一笔。至少理论上是这样的。

在实践中，没有绝对的方法来判断这是否是普遍的滥用。Mt. Gox 肯定在赔钱——你不能心血来潮就关闭客户的账户——但比特币社区强烈反对，称 Gox 没有保持自己独特的识别自己转账的方法是愚蠢的。一位 Reddit 用户写道[“所有这些笨蛋需要做的就是将他们特定于 gox 的 tx id 作为一条消息写入事务中。他们已经知道收款人地址，因此如果有人试图说他们没有收到他们的资金，查看收款人地址，并在他们的系统说他们发送 tx 时找到附有 gox 特定 tx id 的交易将是完全无关紧要的。”总之 Mt. Gox 应该有更好的核算体系。许多主要玩家称 Mt. Gox 的声明](https://web.archive.org/web/20221015160530/http://www.reddit.com/r/Bitcoin/comments/1xieb9/keep_calm_transaction_malleability_is_not_double/cfbmwg8)[往好里说是伪造的](https://web.archive.org/web/20221015160530/https://twitter.com/aantonop/status/432883341465899008)，往坏里说是危言耸听。

由于这次关闭，交易所追踪者已经将 Mt. Gox 从他们的列表中删除，理由是 Mt. Gox 管理员传播了恐惧、不确定性和怀疑。比特币最低跌至 572 美元，今日反弹至 670 美元左右。

没人对 Mt. Gox 满意。

“比特币正处于转型期，Mt.Gox 代表着市场遗留下来的那种不堪重负的遗留基础设施。像这样不必要的和令人困惑的恐慌每年都会发生，Mt.Gox 所追求的是势头和知名度，”[LetsTalkBitcoin.com 主编亚当·莱文说。这个名字的认知度还能有多少价值还不确定，这种情况已经持续了一年多](https://web.archive.org/web/20221015160530/http://letstalkbitcoin.com/)

目前，该交易所是否能恢复到满负荷运转仍是个问题。最古老和最奇怪的比特币交易所之一可能刚刚拔掉了自己的插头。

延伸阅读
[为什么没人能从比特币最大的交易所之一提取比特币/Quartz](https://web.archive.org/web/20221015160530/http://qz.com/175565/why-nobody-can-withdraw-bitcoins-from-one-of-the-currencys-largest-exchanges/)
[Mt. Gox 指责比特币——核心开发者 Greg Maxwell 回应/ CryptocoinsNews](https://web.archive.org/web/20221015160530/http://www.cryptocoinsnews.com/2014/02/10/mt-gox-blames-bitcoin-core-developer-greg-maxwell-responds/)