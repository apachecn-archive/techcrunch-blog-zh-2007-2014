# 世界上最大的生物识别数据库| TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/12/06/inside-indias-aadhar-the-worlds-biggest-biometrics-database/>

印度的[独特身份识别项目](https://web.archive.org/web/20230321025126/http://uidai.gov.in/)，也被称为 Aadhar，本周早些时候完成了对超过 5 亿居民的人口统计和生物特征数据的捕获——这是目前世界上同类项目中最大的生物特征识别项目。

这是一项多年的努力，在隐私和安全倡导者和其他人中间不乏批评者。本周的最新进展涉及 Aadhar 用来捕获、存储和管理数据的方法，以及美国一家名为 MongoDB 的初创公司可能在其中扮演的角色。

NoSQL 数据库初创公司 MongoDB 去年[从中央情报局支持的 In-Q-Tel](https://web.archive.org/web/20230321025126/http://gigaom.com/2012/09/18/in-q-tel-stakes-a-claim-in-mongodb-invests-in-10gen/) 获得了资金，这是一家由中央情报局和其他美国情报机构支持的独立非营利企业。

在过去的几天里，[印度媒体](https://web.archive.org/web/20230321025126/http://articles.economictimes.indiatimes.com/2013-12-03/news/44710564_1_uidai-chairman-nandan-nilekani-uid-data-in-q-tel)的几篇报道引用了政党和活动人士的话，提出了敏感数据是否被印孚瑟斯联合创始人[南丹·尼勒卡尼领导的 Aadhar 泄露的问题。](https://web.archive.org/web/20230321025126/http://en.m.wikipedia.org/wiki/Nandan_Nilekani)

一些报道将争议与 MongoDB 联系起来。

世界各国政府都在关注国家安全局的间谍活动，任何与美国政府情报机构有关的事情都足以引起轩然大波。此外，随着大选定于明年举行，印度的政治言论空前高涨。

尽管如此，这些指控的时机再糟糕不过了，至少对于雄心勃勃的身份识别项目来说是如此，该项目正在等待今年通过的议会法案，以建立一个完全符合宪法的权力机构。

我参观了 Aadhar 在班加罗尔的办公室，据我采访的官员说，事情的真相是，虽然一些人声称大型合同包括与 MongoDB 共享数据，但事实是 Aadhar 使用的是 MongoDB 开源代码，不涉及敏感数据。会议还提供了一个机会来了解地球上最大的生物识别数据库是如何运作的，以及如何处理安全和隐私问题。

此外，印度唯一身份认证机构(UIDAI)驳斥了与任何美国机构共享印度居民数据的指控。

**阿达尔对印度意味着什么**

让我们来看看 Aadhar 的背景，以及它对印度这样的国家意味着什么，超过 5 亿人没有任何形式的官方身份证，这使得他们无法接受政府援助，开设银行账户，获得贷款，获得驾驶执照，等等。该数据库项目现在每天注册 100 多万印度居民，计划到明年年底注册约 12 亿人，使其成为地球上最大的生物识别数据库。

拥有 12 位 Aadhar 号码的最大优势之一是，政府可以将该国穷人的银行账户与其联系起来，并直接转移现金福利和其他补贴。印度已经有近 4000 万个银行账户与 Aadhar 建立了联系。

[据研究公司 CLSA](https://web.archive.org/web/20230321025126/http://knowledge.wharton.upenn.edu/article/nandan-nilekani-on-what-it-takes-to-build-the-worlds-biggest-social-inclusion-program/) 称，在接下来的几年里，印度政府价值 2500 亿美元的补贴和其他福利中，超过 40%将因腐败而流失。Aadhar 将通过向需要政府补贴的人直接转移现金来消除中间商和遏制腐败。

但是几个智囊团和活动家，包括位于 T4 的互联网社会中心，已经开始关注隐私问题，甚至质疑整个项目的有效性。

**地球上最大的生物特征数据库**

我一直试图与 Aadhar 的官员会面，以了解安全方面的情况、迄今为止的进展以及他们对 MongoDB 指控的反应。

他们最终同意周五在班加罗尔南郊马路对面的总部会面，英特尔和思科的印度总部都在这里。从外面看，Aadhar 的技术中心存储了所有居民的数据(现在总共有 5pb 大小),看起来一点也不像政府大楼——它可能会被当作附近存放英特尔或思科的大楼之一。

在里面，当我走进一个中央有十几个电视屏幕的房间时，大约 20 名年轻的工程师狂热地看着前方，在他们的计算机键盘上打字，检查存储信息的数据包的移动，这种设置看起来像一个非常复杂的指挥中心。他们观看的电视屏幕显示了这些数据包(每个大小约为 5MB)从他们在全国 30，000 个注册中心之一登录开始，经过至少三个验证阶段的旅程。验证包括对每个档案进行重复检查，以确保同一个人不会有一个以上的 Aadhar 号码。

因此，对于每一个新的注册，都会针对所有现有的配置文件进行“重复数据消除”检查，目前现有的配置文件超过 5 亿个。

Srikanth Nadhamuni 是一名前英特尔工程师，他在 2010 年 9 月帮助建立了 Aadhar 的技术平台，现在正在班加罗尔运行 Khosla 实验室，他告诉我，这些数据包存储在 2048 位加密的背后，如果试图进行任何未经授权的访问，就会自我销毁。

**处理 MongoDB 争议**

那么，Aadhar 最初为什么要与 MongoDB 合作，它会继续与这家初创公司合作吗？

Aadhar 技术中心的助理总干事 Sudhir Narayana 告诉我，除了 MySQL、Hadoop 和 HBase 之外，MongoDB 是最初为运行数据库搜索而采购的几个数据库产品之一。与只能存储人口统计数据的 MySQL 不同，MongoDB 能够存储图片。

然而，Aadhar 在意识到 MongoDB 无法处理大量数据(数百万个数据包)后，已经慢慢地将其大部分数据库相关工作转移到 MySQL。

他们已经开始使用“数据库分片”:一种将数据包存储在不同机器上的过程，以确保系统不会随着数据量的增加而崩溃。

这帮助 Aadhar 减少了对 MongoDB 的依赖，转而使用 MySQL 来存储大部分数据。

技术中心副总干事 Ashok Dalwai 告诉我，MongoDB 无法访问任何生物特征数据。

“我们相信使用开源技术可以避免任何厂商锁定，但这并不意味着我们以任何方式损害安全性，”达尔维说。

当被联系时，MongoDB 的一位发言人重定向到[这个关于该公司涉及 In-Q-Tel 的资金的公告](https://web.archive.org/web/20230321025126/http://www.mongodb.com/press/10gen-announces-strategic-investment-iqt)。

更重要的是，在这家初创公司从 In-Q-Tel 获得任何资金之前，UIDAI 就开始使用 MongoDB 的开源软件。正如这个 [Crunchbase 条目所显示的，](https://web.archive.org/web/20230321025126/http://m.crunchbase.com/company/mongodb-inc) MongoDB 仅在 2012 年就获得了来自红帽、英特尔投资和 In-Q-Tel 的 770 万美元的风险轮融资。

那么，阿达尔的未来会是怎样的呢？

官员们补充说，尽管围绕它存在争议，但 Aadhar 有望在 2014 年底前招收超过 12 亿印度居民。这将创建一个大约 15pb 大小的数据库。

目前，该项目每天招收大约 100 万居民。纳拉亚纳告诉我，他有信心从明年开始每天实现约 200 万人的注册，这将有助于将剩余的 7 亿人纳入数据库。

[图片来源](https://web.archive.org/web/20230321025126/http://m.flickr.com/#/photos/juliancorrea/6096854427/)