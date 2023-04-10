# 研究:一些互联网服务提供商仍在劫持搜索结果(诉讼随之而来)

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/05/study-some-isps-still-hijacking-search-results-lawsuit-follows/>

试试这个:打开一个新标签，在地址栏输入“kindle”。它很可能会把你带到谷歌搜索结果页面。也就是说，除非 ISP 拦截此类恶意查询，并对其进行任意处理。加州大学伯克利分校的两位计算机科学家发现，[至少有十几家互联网服务提供商仍在做这种事情](https://web.archive.org/web/20230203135901/http://www.newscientist.com/article/dn20768-us-internet-providers-hijacking-users-search-queries.html)，结果是，例如，当有人在地址栏中键入“kindle”时，它不会转到你首选的搜索结果，而是直接转到亚马逊的 Kindle 页面。

在某种程度上是无害的，但事实上，当检查这些条件时，会有很深的侵害性。这些互联网服务提供商正在使用第三方承包商，他们将这种错误或意外的查询货币化。大量的搜索项目，如“kindle”、“apple”和“bloomingdales”正在被监听、记录和拦截，用户的意图被忽略。似乎这还不够，一家被怀疑是这一活动背后的公司 Paxfire 已经申请了一项出于广告目的在 ISP 层面跟踪用户的专利。

说实话，这有点小题大做，但是有充分的理由。每天都有像这样的骗局被 ISP、网络运营商、内容提供商、运营商和所有其他人推出。虽然大规模的东西，如代理谷歌和略读结果往往会得到注意，有大量的灰色区域的做法正在执行，可能是指在 EULAs 等。像“服务质量”目的的数据包检查，实际上是很少监督的数据挖掘。但是，即使这个问题的实际规模不是全国性的，让我们睁大眼睛关注这些事情也很重要。

研究人员 Christian Kreibich 和 Nicholas Weaver 分析了来自 ISP 的流量，发现有 165 个术语被捕获并导致干扰，通常通过附属程序将用户导向相关网站。有可能(尽管看起来不太可能)第三方正在独立做这件事，[如 Charter 向 VentureBeat](https://web.archive.org/web/20230203135901/http://venturebeat.com/2011/08/05/isp-search-redirect/) 描述的那样；他们声称(从经验来看),受雇做一件事的服务(例如，为损坏的网址提供标准页面)可能会变得野心勃勃，决定兼职赚点小钱。

谷歌之前注意到了这一点，并让互联网服务提供商停止篡改他们的结果，但尽管很容易判断你的查询何时被触及，但要判断它们是否被嗅探却不那么容易。ISP 也可以将包分析部分的工作外包给 Paxfire 这样的公司，通过它们路由搜索查询，以便进行记录和可能的数据库建设。

闻到水中的血腥味，纽约律师事务所 Reese Richman 和 Milberg 对 Paxfire 和 RCN 提起了集体诉讼，这是一家总部位于弗吉尼亚州的 ISP，被该研究所指控的不正当行为。与许多以互联网为中心的诉讼一样，这起诉讼在真正评估之前可能会经过几个司法管辖区——尽管 Paxfire 也位于弗吉尼亚州，但该州为诉讼提供了一个自然的起点。

我和 TechDirt 的 Mike Masnick 有着相似的想法:公司认为他们可以做这种事情并侥幸逃脱，这让我感到惊讶。对互联网服务提供商等服务的审查水平只会越来越高，像这样的技术已经被裁定为非法和不道德的。他们以为没人会注意到吗？

* * *

以下是研究发现的 ISP 列表:

cavalier–辛辛那提贝尔–Cogent–Frontier–Hughes–IBBS–Insight Broadband–mega path–pa ETEC–RCN–Wide Open West–XO 通信

如果你认为你可能会受到这种做法的影响，试着运行 Berkeley 的 [Netalyzr](https://web.archive.org/web/20230203135901/http://netalyzr.icsi.berkeley.edu/) web 应用程序，看看是否会有任何可疑的事情出现。