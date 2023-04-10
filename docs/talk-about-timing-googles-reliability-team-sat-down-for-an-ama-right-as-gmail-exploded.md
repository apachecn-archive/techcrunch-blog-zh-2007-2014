# 谈谈时机:就在 Gmail 爆炸之前，谷歌的可靠性团队坐下来参加了一次 AMA

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/01/24/talk-about-timing-googles-reliability-team-sat-down-for-an-ama-right-as-gmail-exploded/>

# 谈谈时机:就在 Gmail 爆炸之前，谷歌的可靠性团队坐下来参加了一次 AMA

呵。最差。时机。永远不会。

大约一个小时前，一群负责维持谷歌生存的工程师坐下来回答 reddit 上的问题。

知道一小时前还发生了什么吗？Gmail 和 Google+ [在全球范围内关闭](https://web.archive.org/web/20230131015128/https://techcrunch.com/2014/01/24/gmail-goes-down-across-the-world/)。

根据他们一年前的[前任 AMA 的说法，这个团队(谷歌称之为‘网站可靠性’团队，或 SRE)“负责 Google.com 的 24×7 运营，以及许多其他谷歌产品背后的技术基础设施，如 GMail、地图、G+和其他你知道和喜欢的东西。”](https://web.archive.org/web/20230131015128/http://www.reddit.com/r/IAmA/comments/177267/we_are_the_google_site_reliability_team_we_make)

几乎可以肯定是巧合。但是非常有趣。可靠性团队只有四名成员在 AMA 工作，你可以确信谷歌雇佣了超过四名员工来保护他们数百万的服务器不着火。正如你所料，帖子顶部的评论(以及页面下方的其他几十条评论)嘲笑了这一不幸的时机。

令人印象深刻的是，该团队似乎并没有流多少汗。团队的每个成员都在这个帖子中贡献了答案，然而事情在 50 分钟内就有所进展，许多用户报告说事情在一个小时内就恢复了。这个来自 AMA 的问题给了我们一点启示:

> Reddit 用户 notcaffeinefree 问:“这么快…当一个谷歌服务关闭时，那里是什么样的？到底有多抓狂？”
> 
> 谷歌的 Dave O'Connor 回应道:
> 实际上，我们对此有一个很好的流程，所有服务都使用——我们使用完整记录的事件管理程序，所以人们清楚地了解他们的角色，可以非常迅速地采取行动。作为污垢测试的一部分，我们还会定期执行这一流程。定期进行特定服务的演练也是确保一旦出现问题，我们能够直接解决的重要组成部分。

看起来这个过程确实非常顺利(尽管大卫·s·佩克可能对此印象不深)。