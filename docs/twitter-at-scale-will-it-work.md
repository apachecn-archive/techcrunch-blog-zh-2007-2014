# 大规模推特:有用吗？

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/05/22/twitter-at-scale-will-it-work/>

![](img/5a26e3dae58b9566bece86b6ed194091.png)

仅在两天前联系人消息应用 [Twitter](https://web.archive.org/web/20230220053135/http://www.twitter.com/) 遭遇了又一轮宕机，这让一些用户感到沮丧，也有人问为什么[平台](https://web.archive.org/web/20230220053135/http://www.techmeme.com/080522/p93#a080522p93)继续遭遇问题。

我最近与一位熟悉 Twitter 技术问题以及这家初创公司面临的挑战的人进行了交谈。他重申了自己的观点，认为问题不在于[布雷恩·库克](https://web.archive.org/web/20230220053135/http://romeda.org/blog/)(被扫地出门的前[工程主管)，也不在于~~乔伊特~~ NTT(他们的东道主)，而是在于他们早期对问题的复杂性缺乏理解。](https://web.archive.org/web/20230220053135/https://techcrunch.com/2008/05/15/blaine-cook-joins-todays-gillmor-gang-talks-twitter/)

问题是群发信息很难大规模实现。其他大型网站如 [WordPress](https://web.archive.org/web/20230220053135/http://www.crunchbase.com/company/wordpress) 和 [Digg](https://web.archive.org/web/20230220053135/http://www.crunchbase.com/company/digg) 大多是在处理已知的问题，比如如何服务大量的页面或大量的图片。Twitter 的独特之处在于，它需要解析大量的消息，并将它们传递给多个接收者，每个用户都与其他用户有唯一的联系。

社交网络也有类似的复杂性问题，但它们通常只需要将消息发送给单个用户(或至多发送给一个定义的组)。即便如此，像 Friendster 这样的社交网络多年来一直在技术和规模问题上苦苦挣扎。Twitter 专门处理文本消息，在大多数情况下，活跃用户的这些消息非常频繁，会发送给数百个联系人(Twitter 中称为关注者)。每一个新的 Twitter 用户和每一个新的连接都会导致成倍增长的计算需求。

一些最好的 web 应用程序能够有效地解决非常复杂的问题，为用户提供简单的结果(例如 Google)。这些应用程序的成功归功于开发人员为解决大型技术挑战所做的创新努力，他们经常不得不为解决方案开辟新天地。为了让 Twitter 达到类似的可靠性，他们也需要一个非常全面的、突破性的解决方案。

与我交谈的消息来源还评论了 Twitter 团队对于他们当前和未来的挑战准备不足的情况。这个小团队包含一些工程师，只有一两个人致力于基础设施和架构。他接着指出，在 Digg，仅网络和系统团队就比 Twitter 的整个工程团队还要大，而且在 Digg，他们由著名的“一线摇滚明星”领导。

Twitter 的问题通常归咎于他们使用了 web 开发框架 [RubyOnRails](https://web.archive.org/web/20230220053135/http://www.rubyonrails.org/) 。Twitter 几乎可以肯定是运行在 Rails 上的最大的网站，所以这个框架的粉丝和它的开发者已经[迅速转移了批评](https://web.archive.org/web/20230220053135/http://www.loudthinking.com/arc/000608.html)并把矛头指向 Twitter 的工程师。利用一个从未征服大规模领域的框架肯定会增加寻找解决方案所需的风险和工作量。作为一个开箱即用的框架，Rails 当然不适合大规模的应用程序开发，但这是 Twitter 能够试验并尽早发布的一个重要原因。

Rails 让 Twitter 能够快速原型化，快速发布，然后轻松迭代新功能。但是古老的格言“好、快、便宜——选择两个”当然适用；Rails 承认它不是一个能在密集型任务上与 Java 或 C 竞争的平台，这对自己没有坏处。Twitter 作为一个应用程序正处于十字路口，Rails 迄今为止很好地完成了它的使命，但你不太可能在近期内看到用 Ruby 在 [Apache](https://web.archive.org/web/20230220053135/http://apache.org/) 构建的计算集群。

我们今天在 Twitter 上看到的是一个非常有用和受欢迎的服务，但有非常复杂的潜在技术挑战需要克服。Twitter 不仅需要一个新的架构方法和他们能找到的最好的头脑的大量注入([、1500 万美元可以帮助](https://web.archive.org/web/20230220053135/https://techcrunch.com/2008/05/22/twitter-closes-third-round-of-financing-from-spark-capital/))，还需要用户和我们这些观察者的一点耐心。