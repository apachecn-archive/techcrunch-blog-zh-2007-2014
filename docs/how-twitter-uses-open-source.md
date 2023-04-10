# Twitter 如何使用开源技术

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/08/30/how-twitter-uses-open-source/>

# Twitter 如何使用开源

Twitter 的 Chris Aniszcyk 今天早上在 CloudOpen 做了一个主题演讲，谈到了 Twitter 是如何使用开源的。

他的演讲深入探讨了开源技术如何在企业环境中扩展基础设施。这是企业界的一个新兴话题。

Aniszcyk 回顾了 Twitter 管理其服务所依赖的开源技术:

*   [MySQL](https://web.archive.org/web/20221124184251/http://dev.mysql.com/) 被大量用于 tweets 的主要存储。该公司公开开发了自己的[MySQL fork](https://web.archive.org/web/20221124184251/http://engineering.twitter.com/2012/04/mysql-at-twitter.html)来与上游社区合作。MySQL 是一个开源的关系数据库。
*   [Cassandra](https://web.archive.org/web/20221124184251/http://cassandra.apache.org/) ， [Hadoop](https://web.archive.org/web/20221124184251/http://hadoop.apache.org/) ， [Lucene](https://web.archive.org/web/20221124184251/http://lucene.apache.org/) ， [Pig](https://web.archive.org/web/20221124184251/http://pig.apache.org/) 和各种 Apache 项目在 Twitter 基础设施中被用来支持分析和搜索等服务。该公司也对这些项目作出了贡献。Twitter 是 Apache 软件基金会的赞助商。卡珊德拉是一个 NoSQL 数据库。Hadoop 是一种分布式文件系统，通常与高级语言一起使用，例如 Pig 是一个用于大数据分析的高级平台。Lucene 是一种开源搜索技术。
*   公司的缓存基础设施大量使用 Memcached 来扩展其不断增长的流量。该公司最近开源了 Twemcache，其灵感很大程度上来自 Memcached 代码库。Memecached 通过减轻数据库负载来帮助加速动态 web 应用程序。

Twitter 也为自己的目的开发软件，并通过开源提供:

*   Iago 是一个负载生成器，创建它是为了在服务遇到生产流量之前帮助测试服务。
*   Zipkin 是一个分布式跟踪系统，该公司创建该系统是为了帮助收集服务的计时数据，这些服务涉及管理对 Twitter API 的请求。本质上，它有助于让 Twitter 更快。
*   [burning](https://web.archive.org/web/20221124184251/https://github.com/twitter/scalding)是一个 Scala 库，它使得在 Hadoop 中编写 MapReduce 作业变得很容易。burning 是为 Cascading 开发的，Cascading 是一个框架，旨在让 Java 开发人员在 Hadoop 的基础上构建大数据应用程序。众所周知，它能够抽象出 [MapReduce](https://web.archive.org/web/20221124184251/http://en.wikipedia.org/wiki/MapReduce) 的复杂性，并使 Hadoop 集群更易于管理。MapReduce 最初由 Google 开发，用于处理搜索数据。Scala 是一种通用编程语言。它表达了常见的编程模式。

脸书和谷歌也开源了他们的技术。结果在企业中显而易见。例如，Hadoop 主要是由雅虎开发的。它现在是我们在整个企业市场看到的大数据推动的基石。

(感谢 L [inux Foundation](https://web.archive.org/web/20221124184251/http://linuxfoundation.org/) 的 Jen Cloer 分享了 Chris 计划在主题演讲中谈论的内容摘要。)