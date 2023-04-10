# AWS 服务器问题搞垮了 Instagram、Vine、Airbnb 和 IFTTT 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/08/25/instagram-vine-and-ifttt-went-dark-thanks-to-amazon-web-services-issues/>

# AWS 服务器问题搞垮了 Instagram、Vine、Airbnb 和 IFTTT

那些想在今天余下的时间里看着人们在 Instagram 或 Vine 上做其他事情的人，可能刚刚经历了一段艰难的尝试。这两项服务都离线了一个多小时，很可能是因为亚马逊网络服务的问题。

Instagram 是两者中第一个在 Twitter 上公开承认问题的，半小时后【Vine 紧随其后。

伴随着服务最初中断的大量推文最早开始于美国东部时间下午 4 点左右，随着用户发现他们无法分享自己的食物图片或精心制作的视频片段，推文的强度越来越大。在 Twitter 和其他地方的进一步调查显示，其他一些已知依赖 AWS 的服务——网飞、 [IFTTT](https://web.archive.org/web/20230327191406/http://www.ifttt.com/) 、 [Heroku](https://web.archive.org/web/20230327191406/https://status.heroku.com/incidents/548) 和 [Airbnb](https://web.archive.org/web/20230327191406/https://twitter.com/Airbnb/status/371731869647532032) 等——今天也遇到了类似的问题。在这一点上，Instagram 和 Vine 在大多数情况下都慢慢恢复了在线，哀叹网飞停电的推特也慢慢枯竭了，但 IFTTT 的网站仍然无法运行。

快速浏览一下 [AWS 的健康仪表板](https://web.archive.org/web/20230327191406/http://status.aws.amazon.com/)可以发现，该公司的北弗吉尼亚数据中心存在一些问题，这些问题可能是所有问题的核心(Airbnb 在今天下午早些时候的一条推文中确认了这种情况[)。在过去的两个小时里，该公司一直在尽职尽责地报告其 EC2、关系数据库和负载平衡服务的问题，尽管最近的更新表明，他们已经设法锁定了根本问题，目前正在清理剩余的混乱。亚马逊首先发现了 EC2 的问题:](https://web.archive.org/web/20230327191406/https://twitter.com/Airbnb/status/371731869647532032)

> 下午 2:21 PDT 我们已经确定并修复了性能问题的根本原因。EBS 支持的实例启动现在运行正常。大多数以前受影响的卷现在都正常运行，我们将继续处理性能仍然下降的实例和卷。

然后转到负载平衡问题:

> 下午 2:45 PDT 我们已经确定并修复了影响单个可用性区域中负载平衡器的连接问题的根本原因。对于在多个可用性区域中具有后端实例的负载平衡器，连接性影响已得到缓解。我们继续致力于仍然存在连接问题的负载平衡器。

无论如何，最糟糕的情况似乎已经过去，但我们暂时会继续关注形势。我希望你远离这些服务的时间花得明智(即不只是在 Twitter 上抱怨)。