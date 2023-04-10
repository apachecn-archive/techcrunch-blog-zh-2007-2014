# Hadoop 和初创公司:开源与业务数据相遇的地方 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/07/17/hadoop-startups-where-open-source-meets-business-data/>

*这篇客座博文由 [Weebly](https://web.archive.org/web/20230205045340/http://www.weebly.com/) 的分析主管[科瓦斯·博古塔](https://web.archive.org/web/20230205045340/http://crunchbase.com/person/kovas-boguta)撰写。2009 年，Kovas 写了一篇关于可视化实时社会结构的[客座博文](https://web.archive.org/web/20230205045340/https://techcrunch.com/2009/09/22/techcrunch50-visualizing-real-time-social-structures/)。*

十年前，开源的 [LAMP (Linux，Apache，MySQL，PHP/Python)](https://web.archive.org/web/20230205045340/http://en.wikipedia.org/wiki/LAMP_(software_bundle)) 栈开始改变 web 创业经济学。随着新的开源网络服务器、数据库和网络友好编程语言将开发者从专有软件和大型硬件中解放出来，启动成本大幅下降。这降低了进入门槛，改变了创业投资游戏，并导致了当前天使/种子投资生态系统的出现。当然，除此之外，还要实现我们每天都在使用的新一代网络应用。

同样的过程现在正在大数据领域展开，以 [Hadoop](https://web.archive.org/web/20230205045340/http://en.wikipedia.org/wiki/Apache_Hadoop) 为中心的开源生态系统取代了昂贵的专有解决方案。因此，创业公司正在创造更智能的业务和更智能的产品。或许更重要的是，这场技术运动有可能模糊传统商业和传统网络创业之间的界限，极大地扩大创新的竞技场。

**问题，遇到解决方案**

即使是一家不太成功的初创公司，其用户数量也可与民族国家相媲美。由此产生的大量用户数据带来了问题和机遇。因为理解每个用户和交易的价值变得更加复杂。机会，因为人们的集体智慧可以被用于更好的用户体验。

直到一两年前，分析这种规模的数据还需要 LAMP 所避免的同一种企业解决方案。与 IBM、甲骨文和 Teradata 这样的公司达成了数年、数百万美元的交易。当然，几乎没有一家初创公司能负担得起这样的费用。此外，这些解决方案的闭源技术谱系使它们与创业工程知识和文化不兼容。

进入 Hadoop。Hadoop 解决这些数据处理问题的方式既兼容启动，又在技术上更胜一筹。作为一个由工程师开发并为工程师服务的开源项目，它非常实用，并且是创业工程实践的主流。它的架构[跨越一个商品节点集群的 map-reducing](https://web.archive.org/web/20230205045340/http://en.wikipedia.org/wiki/MapReduce) 比传统的数据仓库更加灵活和经济。

考虑到被压抑的需求，Hadoop 爆炸也就不足为奇了。要了解一个开源项目做得如何，首先要做的是查看开发者邮件列表流量。如果您收集所有与 Hadoop 相关的邮件列表，并绘制邮件数量，您会得到经典的曲棍球杆增长曲线:

在当今世界，可以毫不夸张地说，技术的未来是由开发人员的采用决定的。随着越来越多的工程师和创业公司采用 Hadoop，它的功能正在成为设计未来产品和业务的默认假设。

**当今初创公司中的 HADOOP**

在高层次上，Hadoop 在当今的初创公司中有 3 个应用领域:1)客户行为分析，2)支持新的面向用户的功能，3)实现以前无法实现的全新业务线。

[Eventbrite](https://web.archive.org/web/20230205045340/http://www.eventbrite.com/) 是 Hadoop 支持面向用户的新特性的一个例子。快速增长的活动服务让组织者管理和推广他们的活动，并帮助用户找到相关的活动来参加。为了帮助公司更快地发展，他们的数据服务团队正在使用 Hadoop 将智能植入产品的各个部分。例如，推荐系统帮助用户找到相关事件，自动分类系统帮助减少用户创建新事件的摩擦。

在 [Weebly](https://web.archive.org/web/20230205045340/http://www.weebly.com/) ，我们部署了 Hadoop 来衡量客户价值——哪些用户将带来最多的收入，我们如何最有效地锁定他们？这是一个相当复杂的计算，涉及很多因素和数据来源。有了 Hadoop，我们可以说“让我们计算一下吧。”

最后一类用途是在 Hadoop 基础上从头开始构建的创业公司。营销智能平台 Backtype 或许是 Hadoop 可能带来的新创业类型的原型。由三名工程师组成的团队运行其操作，包括超过 25tb 的数据和 60 台用于数据处理的服务器，为仪表板 UI 提供服务，并向其他公司提供数据 API。行业现任者在摇摇欲坠的旧架构上投入巨大，几乎没有机会匹配 Backtype 的迭代周期。

**HADOOP:一场运动，而不仅仅是一项技术**

尽管 Hadoop 很实用，但[可预见的反弹](https://web.archive.org/web/20230205045340/http://blogs.forrester.com/james_kobielus/11-06-09-hadoop_when_will_the_inevitable_backlash_begin)声称它被夸大了，指出了诸如易用性、处理实时数据的能力、社交图数据的 map-reduce 的局限性等缺点。但这就像在 [Ruby on Rails](https://web.archive.org/web/20230205045340/http://en.wikipedia.org/wiki/Ruby_on_Rails) 登台之前批评 LAMP 的丑陋，或者在 [Memcached](https://web.archive.org/web/20230205045340/http://en.wikipedia.org/wiki/Memcached) 回避它们之前批评 MySQL 的可伸缩性问题。

理解 Hadoop 的重要性的关键是，它不仅仅是一项特定的技术，而是开发人员试图集体解决其组织的大数据问题的运动。正如 Hadoop 增长曲线所示，面向数据的开源生态系统的技术基础已经奠定，一系列相关技术正开始出现。Rails、Memcached 甚至可以说是[云](https://web.archive.org/web/20230205045340/http://en.wikipedia.org/wiki/Cloud_computing)都是以同样的方式从 LAMP 运动中出现的。

作为一个实时处理系统， [HBase](https://web.archive.org/web/20230205045340/http://en.wikipedia.org/wiki/HBase) 已经迅速赢得了人们的信任，而像 [Spark](https://web.archive.org/web/20230205045340/http://sna-projects.com/blog/2011/03/spark/) 这样的努力指向了能够处理网络分析等任务的通用架构。在可用性方面， [Cloudera](https://web.archive.org/web/20230205045340/http://www.cloudera.com/) 已经做了很多工作来简化安装和管理，尽管还有更多机会。

最引人注目的是创业世界是如何共同创造这个生态系统的:[雅虎](https://web.archive.org/web/20230205045340/http://developer.yahoo.com/hadoop/)、[脸书](https://web.archive.org/web/20230205045340/http://www.facebook.com/notes/facebook-engineering/looking-at-the-code-behind-our-three-uses-of-apache-hadoop/468211193919)、[推特](https://web.archive.org/web/20230205045340/http://engineering.twitter.com/2010/04/hadoop-at-twitter.html)、 [LinkedIn](https://web.archive.org/web/20230205045340/http://sna-projects.com/sna/) 以及一大批早期公司都非常积极地为这个工具链做出贡献。这说明了一个从硅谷出现的新论点或集体智慧:如果一项技术不是你的核心附加值，它应该是开源的，因为这样其他人可以改进它，潜在的未来员工可以学习它。涨潮抬高了所有的船只，而这才刚刚开始。

**企业王国的钥匙**

在当今的技术世界中，有一个铁幕将 startupland 与企业分隔开来。两种技术生态系统，工程实践，以及最终关于什么样的商业是可能的假设。但有了 Hadoop，初创公司现在可以在本质上是商业数据的基础上创造实质性的创新，创建一个与两个世界高度相关的公共平台。

Hadoop 是企业 IT 领域的终极特洛伊木马。它击中了业务的核心——数据，以一种立即增加价值的方式，同时为未来的病毒式增长奠定了基础，连接了两个生态系统以及技术和文化水平。潜在的最终结果是:未来创业公司的竞技场大大扩展，企业的解决方案更便宜、更灵活、更相关。

从计算开始，企业 IT 最终都与数据有关。但是，卡夫卡式的专有解决方案和解决方案的解决方案的激增使得商业数据创新几乎不可能。你可能有一个更好的捕鼠器，但如果它不能“整合”，你就完了。

那么谁来在企业中集成 Hadoop 呢？令人惊讶的是，这是供应商自己。部分是因为大肆宣传，部分是因为在非结构化数据处理等领域的实际优势，供应商们正在努力将 Hadoop 品牌的解决方案推向市场。例如，参见 EMC 的 Hadoop 数据设备系列[，以及 IBM 的 Hadoop 化](https://web.archive.org/web/20230205045340/http://gigaom.com/cloud/emc-hadoop/) [Big Insights](https://web.archive.org/web/20230205045340/http://developer.yahoo.com/blogs/hadoop/posts/2011/05/eric14-talks-ibmbigdata/) 平台。一场 [Hadoop arm 的竞赛](https://web.archive.org/web/20230205045340/http://www.informationweek.com/news/software/info_management/229403178)似乎正在进行中。

现在的关键点是:Hadoop 在企业中的采用为开源生态系统的其余部分提供了一个钩子，从数据分析到 web 和移动技术，再到工程人才库。有了标准化的 Hadoop 集成点，人们只需从 Github 下载 [Yahoo 潜在的 Dirichlet 分配](https://web.archive.org/web/20230205045340/https://github.com/shravanmn/Yahoo_LDA)代码，就可以开始对客户支持电子邮件进行数据挖掘。或者为业务分析师定制 [Hive](https://web.archive.org/web/20230205045340/http://hive.apache.org/) 前端。或者使用 HBase 来协调部门之间的实时数据流。或者将数据后端连接到任意数量的 web 或移动应用程序。这个庞大的开源软件目录和才华横溢的开发人员可以通过 Hadoop“集成”。

简而言之，通过从数据开始，然后扩展到家谱的其他部分，从 web 到云，到移动设备，到软件工程管理的最佳实践，Hadoop 有可能使企业与整个开源和创业世界兼容。因为一旦你能系统地处理数据，你就拥有了通往这个王国的钥匙。

![](img/b650b434b126fb849ef43d1112c8d723.png)