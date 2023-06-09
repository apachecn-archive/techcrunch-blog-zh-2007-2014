# DotCloud 以 Docker 为支点并大获全胜，Docker 是现在 Red Hat OpenShift  的云服务的一部分

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/09/19/dotcloud-pivots-and-wins-big-with-docker-the-cloud-service-now-part-of-red-hat-openshift/>

# DotCloud 以 Docker 为支点并大获全胜，Docker 是现在 Red Hat OpenShift 的一部分的云服务

DotCloud 是一个创业成功的典范。一个新的合作伙伴关系证明了这一点，它将 T2 的开源应用程序可移植性项目与红帽和 T4 的平台即服务(PaaS)相结合。

Docker 是一个轻量级 Linux 应用程序容器，DotCloud 最初是为其多语言 PaaS 开发的。3 月份，DotCloud 推出了 Docker 作为开源项目。使用 Docker，应用程序基本上是由开发人员在虚拟容器中传输的，他们经常使用它们在笔记本电脑和云之间进行同步。

直到现在，Docker 和 Red Hat 都有不兼容的 Linux 内核版本。今天的合作伙伴关系解决了这一问题，使开发人员可以在 OpenShift 中使用 Docker 容器来轻松地在不同的基础设施之间移动代码，而无需满足在虚拟机和操作系统之间移动的沉重要求。

归结起来就是:虚拟机不是为在云之间移动而设计的。因此，相反，Docker 在虚拟机之间移动代码。Docker 既不移植虚拟机，也不移植操作系统。它不需要-计算、存储和网络已经在云服务上就位-应用程序只是被交付到那里运行。

Docker 最初将在 Red Hat Fedora 上提供给社区使用。到今年年底或 2014 年初，Docker 将完全集成到 OpenShift 和 Red Hat Enterprise Linux (RHEL)中。

# 它是如何工作的

乔·费尔南德斯是红帽公司 OpenShift 产品管理部门的负责人。在一封电子邮件中，他说开发人员通过 web 控制台、命令行界面或他们自己的 Eclipse 独立开发环境(IDE)访问 OpenShift。客户可以通过 Red Hat OpenShift 在线服务或他们的企业认证系统进行认证。或者，他们可以使用 OpenShift Enterprise 部署，使用他们自己的基础设施。

然后，开发人员可以访问 OpenShift 中提供的服务，包括各种编程语言和框架，如 Java、Ruby、PHP、Python 和 Node.js。他们还可以访问 Postgresql、MySQL 和 MongoDB 等数据库以及其他服务，如持续集成环境 [Jenkins](https://web.archive.org/web/20230403153044/http://jenkins-ci.org/) 。

Fernandes 说，所有这些都与 Red Hat 称为 OpenShift 的“盒式磁带”打包在一起，然后部署在一个或多个“齿轮”上，这些齿轮是运行在一个或多个 RHEL 操作系统实例上的 RHEL 容器。这就是 OpenShift 的基础。RHEL 操作系统实例可以是运行在虚拟机上的虚拟实例、私有或公共云实例(如 Amazon Web Services ),也可以直接运行在裸机物理服务器上。

Fernandes 表示，通过与 Docker 集成，Red Hat 正在为其 RHEL 设备带来新的功能，这将通过提供更好的便携性和可用性使 OpenShift 开发者受益。开发人员也可以使用 Docker(在 OpenShift 之外)直接将应用程序部署到那些容器中。客户也可以在 Red Hat Enterprise Linux、Fedora 和其他基于 Red Hat 的 Linux 平台(如 CentOS)上运行 Docker。

有了 Docker，这家初创公司及其知名投资者的未来看起来要乐观得多。罗恩·康韦和克里斯·萨卡是 DotCloud 种子轮投资的一部分。在首轮融资中，该公司获得了 Benchmark Capital 和 Trinity Ventures 的投资。伴随着融资，雅虎！联合创始人杨致远、苹果工程经理马克·瓦尔斯坦、Benchmark 的彼得·芬顿和 Trinity 的丹·肖尼克加入了 DotCloud 董事会。

有了 Red Hat，Docker 很快就可以打包用于一些世界上最大的基于 Linux 的企业部署。这不仅是出色的分销，也让 DotCloud 作为一家公司处于一个全新的位置。它现在可以成为整个云生态系统中轻量级应用程序可移植性的标准方法之一。

Docker 的挑战在于 IT，他们仍然习惯于使用虚拟机。移动虚拟机可能很麻烦，但 it 经理知道这是一个过程。但 Red Hat 拥有企业信誉，这将使 Docker 有机会吸引开发人员和运营团队，这意味着更深入地接触企业客户。