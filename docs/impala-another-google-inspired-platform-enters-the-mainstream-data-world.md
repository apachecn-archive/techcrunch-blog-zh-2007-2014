# Impala:另一个受谷歌启发的平台进入主流数据世界 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/12/15/impala-another-google-inspired-platform-enters-the-mainstream-data-world/>

亚马逊网络服务[增加了对](https://web.archive.org/web/20221222050301/http://aws.typepad.com/aws/2013/12/analyze-large-data-sets-with-impala.html)[黑斑羚](https://web.archive.org/web/20221222050301/http://blog.cloudera.com/blog/2012/10/cloudera-impala-real-time-queries-in-apache-hadoop-for-real/)的支持，这是由大数据初创公司 [Cloudera](https://web.archive.org/web/20221222050301/http://cloudera.com/) 开发的谷歌启发的查询工具。它为大量数据提供实时、并行处理。有了 Impala，开发人员可以加载新数据或访问现有数据，在 AWS Elastic MapReduce 集群上使用类似 SQL 的语言运行查询。它更快，更容易访问，并显示了 SQL 在分布式计算的开源系统 Hadoop 中的使用越来越多。从更广泛的角度来看，Impala 反映了谷歌如何深刻影响市场及其发明者，以创建新的数据平台和潜在的更丰富的应用生态系统。

去年推出的 Impala 基于[谷歌 Dremel](https://web.archive.org/web/20221222050301/http://research.google.com/pubs/pub36632.html) ，是这家搜索公司在大数据分析领域的开创性工作的继承者，该公司开发了 [MapReduce](https://web.archive.org/web/20221222050301/http://research.google.com/archive/mapreduce.html) ，这是谷歌开发的一项技术，用于查询其庞大的云宇宙中存储的数据。正如谷歌首席产品经理 William Vambenepe 所说，Dremel 也是谷歌自己的数据分析平台 [Big Query](https://web.archive.org/web/20221222050301/https://developers.google.com/bigquery/) 的基础。[阿帕奇演练](https://web.archive.org/web/20221222050301/http://incubator.apache.org/drill/)基于谷歌 Dremel。 Hortonworks 已经宣布 [Tez](https://web.archive.org/web/20221222050301/http://hortonworks.com/hadoop/tez/) ，这是其 [Stinger Initiative](https://web.archive.org/web/20221222050301/http://hortonworks.com/labs/stinger/) 的一部分，旨在与 [Hive](https://web.archive.org/web/20221222050301/http://hive.apache.org/) 一起工作，后者是用于查询 Hadoop 的数据库。Hortonworks 表示，Stinger 通过熟悉的 SQL 语义提供了“100 倍的 Pb 级性能提升。”

Citus Data 有自己的基于 Google Dremel 的分析数据库。它的创新在于 PostgresSQL 核心中的并行计算来执行查询。 [MapR](https://web.archive.org/web/20221222050301/http://www.mapr.com/support/community-resources/drill) 也在支持 Drill 提供自己的能力。 JethroData 是一家基于 Hadoop 的分析数据库公司，利用了 Google Dremel 项目的原则。

Hadapt 先于所有这些公司推出了其“自适应分析平台”，为 Apache Hadoop 开源项目带来了 SQL 的原生实现。

# 为什么 Dremel 是新的灵感？

对于像 Twitter 这样处理数 Pb 数据的互联网公司来说，Hadoop 是一项重要的技术。对于现在也必须处理前所未有的信息量的传统组织来说，Hadoop 也变得越来越重要。正是针对这部分新一代用户，Impala 才有用武之地。它为他们提供了一种查询数据的方法，而这在以前需要深厚的技术知识。

Hadoop 在过去是一项复杂的任务，需要具有多种才能的人来释放其潜力。这些人是最初的数据科学家，他们学习了编程艺术、集群管理和数据分析。他们来自互联网公司，这些公司需要发明自己的方法来处理和分析他们服务的大量数据。例如，杰夫·哈默巴赫尔离开脸书，成为 Cloudera 的联合创始人之一。Doug Cutting 在雅虎工作时创造了 Hadoop。在那里，他用它来帮助开发一个基于 Lucene 的开源搜索引擎，这也是 Cutting 最初创建的。切割现在在 Cloudera 也有效。

谷歌以 MapReduce 领先，它将一组节点视为并行处理数据的集群。它跨集群映射数据，然后减少数据以回答问题。

除了 MapReduce 之外，Google Dremel 代表了下一代 Hadoop 技术的一个支柱，由不断增长的开源项目生态系统加强，如 [Hive](https://web.archive.org/web/20221222050301/http://hive.apache.org/) 和[Pig](https://web.archive.org/web/20221222050301/http://pig.apache.org/)——所有这些都旨在用更高级的语言抽象 MapReduce 的复杂性。

Dremel 的优势在于它的即时分析。但它主要是用来查询的，而它的对手 Google F1 是一个巨大的关系数据库，最初是用来管理 Google 的在线广告的。

Impala 的价值来自于它的分析能力。这就是为什么它被视为 Tableau(数据可视化技术)等商业智能工具的自然补充。分析师可以使用 Impala 快速查询数据，然后在他们选择的商业智能工具中运行。

Hadoop 在很大程度上并未被视为一个应用开发平台。但是随着 Impala 越来越广泛的使用，以及新的组件被添加到 Hadoop 环境中，这种情况可能会改变。这一点在今年早些时候最新版本的 Hadoop 中变得很明显。在新版本中出现了 [Yarn](https://web.archive.org/web/20221222050301/http://hadoop.apache.org/docs/stable/hadoop-yarn/hadoop-yarn-site/WritingYarnApplications.html) ，它将 MapReduce 抽象为一个调度器和一个资源管理器。它允许扩展到 Hadoop 以前无法实现的范围之外。

Hadoop 带来的应用生态系统在 Impala 和 Yarn 中都很明显。两者都简化了 Hadoop，并为最终用户提供了更深入的功能。然后是 Hadoop 的应用框架 Cascading， [Concurrent](https://web.archive.org/web/20221222050301/http://www.concurrentinc.com/) 已经将其商业化。它把 [Twitter](https://web.archive.org/web/20221222050301/http://www.concurrentinc.com/case-studies/twitter/) 、 [Etsy](https://web.archive.org/web/20221222050301/http://www.concurrentinc.com/case-studies/etsy/) 和 [Airbnb](https://web.archive.org/web/20221222050301/http://www.concurrentinc.com/case-studies/airbnb/) 算作客户。

长期以来，谷歌一直领先于市场。但 Hadoop 和平台层的创新表明，谷歌与其同行之间的差异正在开始缩小。

*专题图片由[电动绵羊](https://web.archive.org/web/20221222050301/http://sheep.arces.net/generation-243/dead.cgi?id=14933)通过知识共享提供)*