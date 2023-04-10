# 开源搜索引擎 Apache Lucene/Solr 获得重大更新

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/10/12/open-source-search-engine-apache-lucenesolr-gets-big-update/>

# 开源搜索引擎 Apache Lucene/Solr 获得重大更新

今天，阿帕奇基金会发布了对开源搜索引擎构建工具 Lucene 和 Solr 的重大更新。版本 4.0 增加了几个新特性，旨在使 Solr 更易于使用，更具可伸缩性和可定制性。

尽管它们是联合开发的，Lucene 和 Solr 实际上是两码事。Lucene 只是一个 Java 库，不是一个独立的搜索引擎。Solr 是以 Lucene 为核心构建的搜索引擎服务器。

Lucene 由 Doug Cutting 于 1999 年创建，他更出名的名字是 [Apache Hadoop](https://web.archive.org/web/20230315100804/http://hadoop.apache.org/) 的创造者，并被 AOL 和 LinkedIn 这样的公司用来增强搜索功能。Solr 由 Yonik Seeley 于 2004 年创建。它可以作为一个定制的搜索引擎，或用于一个单独的应用程序的动力搜索。

根据[搜索引擎中心](https://web.archive.org/web/20230315100804/http://searchhub.org/dev/2012/10/12/apache-solr-and-lucene-4-0-0-released/)的说法，可伸缩性是 Solr/Lucene 团队今天发布的最大焦点——特别是向外扩展而不是向上扩展。

像谷歌和 Amazon.com 这样的网络公司近年来已经普及了横向扩展。过度简化:当您纵向扩展时，当您需要更多容量时，您会用更强大的服务器替换现有的服务器。横向扩展时，您需要向环境中添加更多服务器来增加容量。这种方法通常被视为物有所值，但是服务器集群可能难以设置和管理，并且跨集群分发数据会带来许多挑战。

为了解决这些问题，4.0 版引入了一系列工具，旨在简化 Solr 服务器集群的构建和管理，包括一个新的索引系统，旨在分布式环境中提供近乎实时的搜索结果。

这些特性将有助于 Solr 与 ElasticSearch 竞争，elastic search 是一个开源的、基于 Lucene 的搜索引擎服务器，长期专注于分布式环境。

4.0 中的其他新特性包括一个新的基于 web 的 UI，一个拼写检查器和对空间数据的更好支持(这对任何进行地理搜索的人都很有用)。新版本也将给予用户更多的定制和控制。

Seeley 创办的 LucidWorks 公司为 Solr 提供商业支持。

![Apache Solr 4.0 admin screenshot](img/23cf5828df393d7d1392a7ce37178f0d.png "Apache Solr 4.0 admin screenshot")