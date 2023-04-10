# 收购 Citrix 后，Cloud.com 的 CloudStack 实现 100%开源 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/29/post-citrix-acquisition-cloud-coms-cloudstack-goes-100-open-source/>

# 收购 Citrix 后，Cloud.com 的 CloudStack 实现了 100%开源

在 7 月份被 Citrix Systems 以超过 2 亿美元的价格[收购后，](https://web.archive.org/web/20230205041138/https://techcrunch.com/2011/07/12/citrix-buys-cloud-com-for-more-than-200-million-redpoint-is-on-a-roll/) [Cloud.com 的](https://web.archive.org/web/20230205041138/http://www.cloud.com/) CloudStack 云管理框架正在开源。该软件目前支持超过 60 个大规模的生产云，包括由 GoDaddy、GreenQloud、KT、诺基亚、Tata Communications 和 Zynga 运营的云。在该版本中，CloudStack 还增加了对额外虚拟机管理程序的支持和对裸机配置的支持。

Cloud.com 于 2010 年 5 月推出，为公司提供了私有的类似 EC-2 的基础设施。然而，该公司承认，它经常将其名称(“Cloud.com”)与开源 CloudStack 项目互换使用，造成了很大的混乱。实际上，Cloud.com 之前维护了两个独立的代码库——一个面向付费用户，一个面向开源用户。截至上周，这两个代码库已经在 GPU GPL v3 许可下合并为一个。代码可以从 cloudstack.org 的[下载。](https://web.archive.org/web/20230205041138/http://www.cloudstack.org/)

此外，随着本周在拉斯维加斯举行的 VMworld 2011 大会上推出 CloudStack 2.2.10，该框架现在支持 VMware 新推出的 ESXi 5.0 虚拟机管理程序和 Oracle 的 VM 2。Xen 虚拟机管理程序的 x 个变体，以补充它已经支持的 VMware、KVM 和 Xen 虚拟机管理程序的范围。对微软 Hyper-V 的支持将在今年晚些时候到来。与之前的 CloudStack 一样，客户可以混合搭配多种虚拟机管理程序，包括专有的和开源的，并在高度可用的云计算实例中使用它们。

另一项新功能是裸机配置，它允许客户设置不运行虚拟机管理程序软件的裸机主机。这些可以在与虚拟实例相同的云中使用 CloudStack 管理服务器进行管理。

cloud 还表示，它正在努力将 IaaS 云计算项目 [OpenStack](https://web.archive.org/web/20230205041138/http://www.openstack.org/) 的功能融合到 CloudStack，Citrix 是该项目最重要的贡献者之一。未来，Citrix 和 CloudStack 工程师将把 OpenStack Storage (Swift)与 CloudStack 集成在一起，并努力让 CloudStack 管理服务器和 Web 界面能够管理 OpenStack 实例。