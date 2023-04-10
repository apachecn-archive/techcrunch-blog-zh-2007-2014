# ARM 驱动的云来到 OpenStack | TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/07/18/the-arm-powered-cloud-comes-to-openstack/>

# ARM 驱动的云来到 OpenStack

苹果在其 iPhones 和平板电脑上的芯片组使用 ARM 架构。现在，我们看到 ARM 架构在服务器上首次用于支持云环境。

[OpenStack](https://web.archive.org/web/20230328231634/http://openstack.org/) 的贡献者在 TryStack.org[，](https://web.archive.org/web/20230328231634/https://trystack.org/)开发了第一个 ARM 驱动的 OpenStack 云，作为探索和测试 OpenStack 的免费沙盒。这一消息于今天在俄勒冈州波特兰市的 T4 OSCON 宣布。

后果在几个方面显而易见:

*   它显示了 OpenStack 生态系统的深度，它能够吸引 ARM 生态系统的工程师来实现该项目。撰稿人包括来自 [Calxeda](https://web.archive.org/web/20230328231634/http://www.calxeda.com/) 、思科、Core NAP、戴尔、Equinix、惠普、NTT 和 Rackspace Hosting 的工程师，
*   它展示了 OpenStack 发展其社区并使其可以运行的架构多样化的动力。例如，开发 TryStack cloud 是为了在 OpenStack 支持的架构上测试软件。根据 OpenStack 的说法，用户现在可以选择在两个 TryStack 区域中启动实例:一个运行标准硬件的 x86 区域和一个新的 ARM 驱动的区域，这两个区域都运行最新的 OpenStack Essex 软件版本。
*   它标志着 ARM 驱动的基础设施在这里说，这可能是对英特尔及其 x86 技术市场主导地位的威胁。

管理高能耗服务器的高成本将推动 ARM 的采用。电力和冷却成本在服务器的拥有成本中占主导地位。它比硬件本身的成本高出七倍。据 ARMdevices.ne 报道，IDC 报告称，2010 年全球所有服务器消耗了 445 亿美元的电力，并需要建造 10 个额外的千兆瓦发电厂。

Calexeda 博客很好地框定了这个问题:

> 在当今的云架构中，虚拟化被用作提供弹性、动态工作负载管理和多租户安全性的手段，同时共享相同的底层物理系统(往往是非常大的服务器)。然而，如果我们采取相反的方法，并能够通过使用许多更小的服务器来提供相同的好处，会怎么样呢——一些人创造了这个短语作为*物理化*。突然，我们回到了专用托管和有保证的性能的模式，但仍然采用客户习惯的按需访问和基于云的定价。只要终端用户能够访问计算资源，并且基础设施的经济性对云提供商有意义，这最终可能是云计算的双赢前景。

OpenStack 正在对这些裸机服务器进行实验。这项工作表明了 ARM 驱动的云的崛起，以及未来远离高端服务器主导的云。