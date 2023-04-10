# 地狱矩阵和两个针对新兴不可知论云的开源项目 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/07/28/the-matrix-of-hell-and-two-open-source-projects-for-the-emerging-agnostic-cloud/>

DotCloud 联合创始人的应用容器服务 Docker 和 SaltStack 创始人的开放 DevOps 平台 [Salt](https://web.archive.org/web/20221003204231/http://saltstack.com/community.html) 上周在 OSCON 被称为最令人兴奋的两个新开源项目。

复杂性来自云及其与企业数据中心的契合度。Docker 团队将这个服务和设备的新世界称为地狱矩阵。Salt 的人认为速度是一种救赎——也许是为了将我们从需要大量资源的重量级系统带来的地狱中拯救出来，这些重量级系统由于是在分布式系统不像今天这样普遍的时候构建的，所以速度很慢。

这两个项目都与新[网站云](https://web.archive.org/web/20221003204231/http://dotcloud.com/)首席执行官 Ben Golub 和联合创始人 Solomon Hykes 描述的更深层次的复杂性有关，这个世界类似于一个矩阵，由无数可用服务的行和代表应用程序运行的任意数量设备的列来表示。DotCloud 支持 Docker 开源项目。

它们的出现也代表了可以被称为“不可知论者云”的新现实。当然，有一个关于云的信仰结构，但是没有一个万能的忠诚于它的力量。相反，有一种不可知论的趋势，即通过在任何地方运行的提供商和开源服务(无论是私有数据中心还是公共云服务)来实现内部部署和云服务。

# 码头工人

Docker 作为一个轻量级的 Linux 容器自动部署应用程序。该容器可以在笔记本电脑上构建和测试，并同步到任何地方运行。它可以在虚拟机、裸机服务器、OpenStack 集群、公共实例或内部和云产品的任意组合上运行。

Docker 既不移植虚拟机，也不移植操作系统，考虑到基础设施本身正在成为操作系统，这是有意义的。计算、存储和网络已经在云服务上就位，应用程序只是在那里运行。

该服务避免了移动虚拟机带来的问题，因为虚拟机不是为在云之间移动而设计的。因此，Docker 不是移动虚拟机，而是在虚拟机之间移动代码。大部分安全性由 Linux 内核管理。

Hykes 在上周的一次采访中说，开发者特别喜欢持续测试和集成应用容器的能力。这为构建可以在任何地方运行的应用程序提供了更简单、更快速的方法。例如，开发人员正在使用 Docker 构建下一代平台即服务(PaaS)产品。这是一个值得注意的发展。大多数 PaaS 提供商一直以来都提供单一平台来做尽可能多的事情。使用 Docker，可以构建平台，利用不同提供商的服务来创建用于构建和交付应用程序的轻量级环境。

关于 Docker 更多的技术描述，这里有一些好的资源[这里](https://web.archive.org/web/20221003204231/http://blog.docker.io/)、[这里](https://web.archive.org/web/20221003204231/http://www.activestate.com/blog/2013/06/solomon-hykes-explains-docker)和[这里](https://web.archive.org/web/20221003204231/http://www.infoq.com/news/2013/03/Docker)。

# 盐

Salt 是一个新的开放式 DevOps 平台，旨在提高速度。它旨在使用通用高速通信，通过并行数据处理将数据移动到节点。通用命令被发送到节点，反馈很快返回。哈佛大学将其用于他们的超级计算机集群。曾经需要 15 分钟的工作现在只需要 5 秒钟。

根据 SaltStack 网站的说法，Salt 可以通过一条通信总线扩展到数万台服务器，该总线可以协调、远程执行和配置管理以及其他任务。

Salt 正被用来取代 Chef 和 Puppet 这两个领先的 DevOps 平台。现在被 LinkedIn 和 Rackspace 使用。下面是[摘自](https://web.archive.org/web/20221003204231/http://www.lecloud.net/post/29325359938/salt-to-the-rescue) [Sebastian Kreutzberger](https://web.archive.org/web/20221003204231/http://www.kreutzberger.com/) 的精彩分析，他是 [RhodeCode](https://web.archive.org/web/20221003204231/https://rhodecode.com/) 的首席执行官，RhodeCode 是 Git 和 Mercurial 的开源软件配置和管理平台:

> Salt 就像是厨师/木偶(定义状态)的混合体，也是一种与机器直接通信的简单方式(比如 MQ)。与 Chef 的最大区别在于架构:从设备(称为 minion)不会每隔几分钟就进行更改，这可能会导致不可思议，但它与主设备有一个固定的连接，允许即时更改和命令。

关于 Salt 经常提到的是它的文档，这有助于社区进一步开发这个平台。以下是盐的创造者托马斯·哈奇对盐的介绍:

【YouTube = http://www . YouTube . com/watch？v=ZMrWF9d5Vbw&w=640&h=360]

# 结论

云和本地系统开始融合成一个紧密的整体。OpenStack 是一种使数据中心环境更具弹性的方法。像 Amazon Web Services 这样的云服务代表了公共云基础设施。PaaS 提供商正在成为向这些不同的基础设施提供应用的环境。这些不可知的提供商，如 Cloud Foundry，并不服务于一个云。它们帮助开发人员服务于多种云环境。

像 [CloudMunch](https://web.archive.org/web/20221003204231/https://www.cloudmunch.com/) 这样的服务也是如此，它提供了一个持续的集成平台，可以在不同的云服务之间移动代码。CloudMunch 创始人帕拉德普·帕布说，这个新的宇宙世界有三个主要特征:

*   对于任何 IaaS/云或内部/私有云，必须可以选择将任何开发人员或运营工具与任何 PaaS 配合使用。
*   它必须以工作负载为中心。任何对给定工作负载最有意义的东西，包括工具、模式和实践以及为该工作负载提供最佳结果/roi 的基础架构/云。
*   它能够定义一个可定制的软件交付进度，对应用程序代码和基础架构代码进行检查和平衡，而不局限于任何工具、方法或云。

类似的原则也适用于 Docker，它将应用程序容器视为将应用程序交付到云或任何其他基础架构的方式。盐也符合这种普遍的心态。

新世界不是万能系统中的普遍控制和信仰。像 Docker 和 Salt 这样的开源产品很受欢迎，因为它们符合云和数据中心宇宙的这种更灵活和不可知论的观点。

图片来源:[维基百科](https://web.archive.org/web/20221003204231/https://en.wikipedia.org/wiki/Heaven)