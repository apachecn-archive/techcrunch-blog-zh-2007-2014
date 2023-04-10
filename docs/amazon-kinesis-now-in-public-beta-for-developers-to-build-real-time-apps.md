# 亚马逊 Kinesis 现已进入公测阶段，供开发者构建实时应用 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/12/17/amazon-kinesis-now-in-public-beta-for-developers-to-build-real-time-apps/>

# 亚马逊 Kinesis 现已进入公测阶段，供开发者构建实时应用

该公司的新数据流分析平台亚马逊 Kinesis 现已进入公测阶段。它允许开发人员构建实时应用，而无需管理多个集群的复杂性。但是，尽管它被宣传为一种新型的实时应用平台，但它也有一些缺点，这些缺点自其在 AWS Re:Invent 的[发布](https://web.archive.org/web/20221206202151/https://beta.techcrunch.com/2013/11/14/amazon-kinesis-a-new-aws-service-to-process-real-data-streams/)以来就已经出现了。

AWS Kinesis 每秒传输数千个数据流。它允许开发人员从任意数量的来源提取任意数量的数据，并根据需要进行缩放。AWS Re:Invent 的亚马逊首席技术官沃纳·威格尔表示，在传感器以任何方式传输信息的世界里，该平台的力量来自于它处理数据的能力。沃格尔斯指出，将会越来越多地使用传感器来记录数据。有了 Kinesis，建筑商可以查看数据并确定在地基中浇注混凝土的最佳时间。

Kinesis 跨多个可用性区域工作，这也是为了实现高可用性而复制的。该服务将数据分成数据流，每个数据流处理 1，000 个写事务和多达 20 个读事务。

这是上周由戴尔云管理企业解决方案高级主管[伯纳德·戈尔登](https://web.archive.org/web/20221206202151/http://ht.ly/rR4pp)制作的关于新 Kinesis 服务的视频入门。

【YouTube = http://www . YouTube . com/watch？v=jXljE9Rh4ZQ&w=640&h=360]

AWS 将 Kinesis 定位为 Hadoop 的替代产品，Hadoop 传统上使用批处理数据来进行分析。但这只是故事的一部分。Hadoop 背后有一个多样化的生态系统，其中有一些新产品，如 [Yarn](https://web.archive.org/web/20221206202151/https://hadoop.apache.org/docs/current2/hadoop-yarn/hadoop-yarn-site/YARN.html) ，它提供了实时处理能力，并为构建实时应用程序奠定了基础。

在最近的一篇博客文章中， G 戈登沃利三世写道 Kinesis 与 [Storm](https://web.archive.org/web/20221206202151/http://storm-project.net/) 相比，后者是 Twitter 开源的另一个数据处理工具。

在他的测试中，Worley 发现 Kinesis 是有弹性的，能够根据负载自动扩展，这消除了管理 EC2 集群的一些复杂性。他写道，如果它像宣传的那样工作，它将大大简化集群操作，而不是用 Storm 设置。

沃利写道，与 Hadoop 批处理相比，AWS 的准入门槛更低。但总的来说，Kinesis 不是为复杂的数据流集成而构建的。

> 然而，缺点是每个 Kinesis 应用程序只包含一个过程，所以你不能像 Storm 那样进行复杂的流处理，除非你将多个 Kinesis 应用程序连接在一起。自然，我对此有些担心。

Kinesis 凭借其数据流功能标志着分析世界的一个新时代。但是 AWS 并不是第一个到达现场的，也不一定是领导者。开源社区有越来越多的选项可以替代 AWS 及其专有基础设施。