# 读者:你的云战略是什么？

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/04/13/readers-whats-your-cloud-strategy/>

# 读者:你的云战略是什么？

我每周都会收到关于一些新的(或旧的！)公司和他们所谓的云解决方案。一些人显然滥用了“云”这个流行词汇，而其他人实际上正在利用分布式计算、基础设施和平台即服务、编排和相关技术做一些有趣的事情。亚马逊是 IaaS 的主要推动者，但 [OpenStack](https://web.archive.org/web/20221209062811/http://www.openstack.org/) 、 [CloudStack](https://web.archive.org/web/20221209062811/http://cloudstack.org/) 和 [Eucalyptus](https://web.archive.org/web/20221209062811/http://www.eucalyptus.com/) 都在该领域表现强劲。VMware 的 [Cloud Foundry](https://web.archive.org/web/20221209062811/http://www.cloundfoundry.com/) 和 Red Hat 的 [OpenShift](https://web.archive.org/web/20221209062811/https://openshift.redhat.com/) 正在推动开源 PaaS，而像 [Heroku](https://web.archive.org/web/20221209062811/http://www.heroku.com/) 、 [Engine Yard](https://web.archive.org/web/20221209062811/http://www.engineyard.com/) 和 [dotCloud](https://web.archive.org/web/20221209062811/https://www.dotcloud.com/) 等服务正在推动成为你的托管 PaaS 解决方案。

这并不奇怪，如此多的人正在寻找差异化的云解决方案，总的来说，我认为竞争是一件好事，最终会让最终用户受益。但就目前的情况来看，考虑到过多的选择，我觉得制定一个全面的“云战略”极其困难。

如果你非常关心开源，这有助于限制你的选择。VMware 的 Cloud Foundry 已经开源了相当一段时间，最近庆祝了它的[第一个生日](https://web.archive.org/web/20221209062811/http://blog.cloudfoundry.com/post/13481011539/a-year-of-cloud-foundry)。Red Hat 的 OpenShift 还不是开源的，但正在进行补救工作。显然，Red Hat 拥有成功开源其作品的悠久历史。红帽最近还宣布他们将成为新重组的 OpenStack 董事会的白金会员。另一方面，VMware 不是一家我很容易将开源文化或成功联系在一起的公司；我没有看到一个非常强大的生态系统围绕着云铸造。希望这种情况会有所改善。

还有 [Canonical](https://web.archive.org/web/20221209062811/http://www.beta.techcrunch.com/tag/canonical) ，T2【UbuntuLinux 发行版背后的人。Canonical 为 OpenStack 做出了真正的努力，但他们对 OpenStack 的实际贡献似乎并没有像[所说的那样](https://web.archive.org/web/20221209062811/http://www.internetnews.com/blog/skerner/red-hat-contributes-more-to-openstack-than-canonical-ubuntu.html)。Canonical 没有专注于直接为 IaaS 或 PaaS 产品做出贡献，而是忙于制作助手产品，如[金属即服务](https://web.archive.org/web/20221209062811/https://beta.techcrunch.com/2012/04/04/canonical-metal-as-a-service-not-quite-as-cool-as-it-sounds/)和他们新宣布的[“Any Web Service over Me”](https://web.archive.org/web/20221209062811/http://www.ubuntu.com/cloud/private-cloud/awsome)(缩写为 AWESOME)，旨在提供一个 API 抽象层，以方便在 Amazon 云和 OpenStack 云上运行工作负载。

所有这一切的最终结果是，对于希望部署云解决方案的客户和公司来说，存在许多模糊之处。如果您想要一个私有云，在我看来，如果不首先决定您最终是否需要使用公共云资源，您就无法做出决定。如果是这样，您对私有云技术的选择显然取决于您的预期公共云目标的长期可行性。如果你认为亚马逊在公共云方面处于领先地位，那么 Eucalyptus 似乎是你构建私有云的基础(除非你想摆弄更多的技术，实现 Canonical 的牛逼)。如果你认为 Rackspace 是它现在的位置，那么 OpenStack 对你来说是一个更有吸引力的选择。但是[如果您对公共云提供商的选择是错误的](https://web.archive.org/web/20221209062811/http://www.readwriteweb.com/cloud/2012/04/amazon-apis-industry-standard.php)该怎么办？

因此，我很想知道你——读者——目前在做什么。您做出技术决策了吗？你是孤注一掷，还是留有余地，以便在必要时转向不同的供应商？你去 IaaS 还是 PaaS？您是一家新公司，还是一家将现有工作负载迁移到新平台的老牌企业？最后，我特别想听听受监管行业(银行、医疗保健、保险等)的人们的意见，在这些行业中，您关于在哪里运行应用程序的决定可能会受到法律问题的影响。