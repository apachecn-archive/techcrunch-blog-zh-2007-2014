# 网络设备的拙劣软件更新导致了 GitHub 有史以来最严重的中断之一 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/12/27/botched-software-update-to-networking-gear-caused-one-of-githubs-all-time-worst-outages/>

# 对网络设备拙劣的软件更新导致了 GitHub 有史以来最严重的一次中断

一次拙劣的网络设备软件更新导致 GitHub 上周末出现有史以来最严重的中断之一，这是这个流行的社交编码平台的客户在过去几周内遭受的第二次重大中断。

在一篇博客文章中，GitHub 的[马克·因布里亚科](https://web.archive.org/web/20221203004244/https://github.com/imbriaco)解释说，12 月 22 日的中断发生在 Github 的未具名网络供应商推荐的聚合交换机软件更新期间。这次更新本来是为了解决导致[公司在 11 月下旬发生的最后一次大停电](https://web.archive.org/web/20221203004244/https://github.com/blog/1346-network-problems-last-friday)的问题。

随后对文件服务器的影响进一步加剧了这一问题，再加上其他问题，迫使该公司将服务置于维护模式。服务中断持续了大约 19 个小时。GitHub 并没有一直中断，但是延迟和无法访问确实持续了很长一段时间。

数据中心网络可以有各种交换机来保持数据流动。GitHub 使用接入交换机连接到服务器。这些设备依次连接到一对聚合交换机，这些交换机“使用一种称为 [MLAG](https://web.archive.org/web/20221203004244/http://en.wikipedia.org/wiki/MC-LAG) 的功能，对接入交换机表现为单个交换机，用于[链路聚合](https://web.archive.org/web/20221203004244/http://en.wikipedia.org/wiki/Link_aggregation)、[生成树](https://web.archive.org/web/20221203004244/http://en.wikipedia.org/wiki/Spanning_Tree_Protocol)以及其他希望拥有单个主设备的第 2 层协议。”

有一对就有出错的空间。这意味着应该有备份。但是在升级过程中，出现了一个定时错误，导致两台交换机之间出现混淆。这导致了大量的客户流失和服务中断。

Imbriaco 是这样解释的:

> 这就是事情开始变糟的地方。当其中一台交换机上的代理被终止时，对等方有 5 秒钟的超时时间等待再次收到代理的消息。如果它没有收到对等方的消息，但仍然看到它们之间的活动链路，它会认为另一台交换机仍在运行，但处于不一致的状态。在这种情况下，它无法安全地接管共享资源，因此默认情况下，它会恢复为独立的交换机，用于链路聚合、生成树和其他第二层协议。

文件服务器也受到网络交换机混淆的困扰。在这个过程中，出现了我们经常看到的涉及主要服务的中断。在混乱中，机器试图获得控制权，这给客户带来了更多的问题和持续的问题。

GitHub 的中断对那些正在成长的初创公司和企业商店来说是一个教训，它们正在探索保持扩展服务稳定的方法。但它也显示了当重大停机发生时不可避免会发生什么。系统开始转发不正确的信息，从而导致连锁反应，影响客户及其使用服务的能力。