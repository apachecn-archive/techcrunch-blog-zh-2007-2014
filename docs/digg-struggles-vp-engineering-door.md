# 当 Digg 苦苦挣扎时，工程副总裁被扫地出门 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/09/07/digg-struggles-vp-engineering-door/>

# 当 Digg 苦苦挣扎时，工程副总裁被扫地出门

![](img/61702df7c66b489cd178c94835743e85.png)

自从 Digg [推出了新的网站设计](https://web.archive.org/web/20230213025514/https://techcrunch.com/2010/08/25/new-digg-launch/)，它就被[各种各样的麻烦困扰着](https://web.archive.org/web/20230213025514/https://techcrunch.com/2010/08/30/broken-is-repaired/)，尤其是它的[持续下降](https://web.archive.org/web/20230213025514/https://techcrunch.com/2010/08/26/digg-fail-ox/)。新架构的问题如此严重，以至于工程副总裁约翰·奎因已经离开，我们已经从接近 Digg 的消息来源处得到证实。

在今天的 Diggnation 视频中，首席执行官[凯文·罗斯解释了](https://web.archive.org/web/20230213025514/https://techcrunch.com/2010/09/07/kevin-rose-responds-to-digg-criticism-on-diggnation-mostly-tells-users-to-chill/)该网站正在处理的一些技术问题，以及为什么它不能简单地回滚到以前的架构。Digg 的新版本 v4 基于一个名为 [Cassandra](https://web.archive.org/web/20230213025514/http://cassandra.apache.org/) 的分布式数据库，取代了网站之前运行的 MySQL 数据库。Cassandra 非常先进——它应该更快，规模更大——但也许它仍然太具实验性。或者这只是 Digg 实现它的方式( [Twitter 使用 Cassandra](https://web.archive.org/web/20230213025514/http://nosql.mypopescu.com/post/407159447/cassandra-twitter-an-interview-with-ryan-king) ，尽管[不是为了它的主要数据存储](https://web.archive.org/web/20230213025514/http://engineering.twitter.com/2010/07/cassandra-at-twitter-today.html)，正如[脸书](https://web.archive.org/web/20230213025514/http://www.facebook.com/note.php?note_id=24413138919)在某些地方所做的那样，但它显然没有经过必要的战斗考验)。Digg 的每个工程师目前都在努力保持网站的正常运行。

我们的消息来源称，奎因是搬去卡桑德拉的主要支持者。现在，该网站正遭受巨大的打击，至少在短期内，因为那个决定和/或它是如何实施的，奎因正在用他的工作为此付出代价。但是还不清楚 Digg 还应该做些什么。Digg 最初是建立在可靠的开源技术 [LAMP stack](https://web.archive.org/web/20230213025514/http://en.wikipedia.org/wiki/LAMP_(software_bundle)) (Linux，Apache，MySQL，PHP)之上的，但是它在 Digg 的流量负荷下已经不堪重负。用 Cassandra 替换 MySQL 应该有助于解决这个问题。相反，它带来了一系列更大的问题。

奎因大约三年前加入 Digg。在此之前，他是 SquareTrade 的工程副总裁和甲骨文的软件工程师。目前还不清楚谁会取代他在 Digg 的位置。