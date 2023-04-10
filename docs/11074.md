# Linux Foundation、Canonical 和 Red Hat 对安全启动进行了评估 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/10/28/linux-foundation-canonical-and-red-hat-weigh-in-on-secure-boot/>

最近有一些关于[安全引导](https://web.archive.org/web/20230205021016/http://en.wikipedia.org/wiki/Secure_boot#Secure_boot)的喧嚣，这是一个硬件验证的、无恶意软件的操作系统引导过程，旨在提高计算机的整体安全性。作为 [UEFI 规范](https://web.archive.org/web/20230205021016/http://en.wikipedia.org/wiki/UEFI)的一部分，安全引导可以禁止未签名操作系统的加载和执行，该规范旨在取代我们许多人熟悉的老化 BIOS。微软要求所有希望使用“专为 Windows 8 设计”徽标的 OEM 系统都必须激活并强制执行安全启动。该技术的性质以及微软推荐的实现方式可能会使最终用户失去对整个系统的控制，并且在这种配置下，安全引导可能会阻止自由软件操作系统的加载。

在对 [Slashdot](https://web.archive.org/web/20230205021016/http://linux.slashdot.org/story/11/09/21/062231/how-microsoft-can-lock-linux-off-windows-8-pcs) (还有哪里？)，更冷静的头脑占了上风，并已在一些细节上审查了 UEFI 安全引导规范。与旧的 BIOS 相比，这是一个非常显著的变化:公钥加密的使用使整个事情变得相当复杂。但是，表面上看，没有任何关于安全引导的东西专门锁定自由软件操作系统。

Linux 基金会发布了一篇名为“[让 UEFI 安全启动与开放平台一起工作](https://web.archive.org/web/20230205021016/http://www.linuxfoundation.org/publications/making-uefi-secure-boot-work-with-open-platforms)”的论文，作者是技术顾问委员会成员，Parallels 服务器虚拟化 James Bottomley 和 LWN.net 编辑 Jonathan Corbet。同时，Bottomley 与 Canonical 的技术架构师 Jeremy Kerr 和 Red Hat 的高级软件工程师 Matthew Garret 合作，开发了另一篇名为“ [UEFI 安全引导对 Linux 的影响](https://web.archive.org/web/20230205021016/http://blog.canonical.com/2011/10/28/white-paper-secure-boot-impact-on-linux/)”的论文。

前一份文件是对这种情况的高度分析(只有四页)，并就原始设备制造商如何销售能够与专有和自由软件操作系统兼容的硬件提出了一些总体建议。后一个文档技术性更强一点(八页！)，并为原始设备制造商提供了一些更加具体的建议。

如果您不熟悉公钥加密的一些基础知识，整个事情可能会有点混乱。平台密钥、密钥交换密钥、签名数据库。这是不是太麻烦了？我向 Linux 基金会提出了几个问题要求澄清，詹姆斯·博顿利作出了回应。

**TechCrunch** :首先也是最重要的一点，对最终用户的现实影响是什么？如果 SecureBoot 的文档让我感觉如此复杂，那么许多人会不会决定让他们的系统处于“设置”模式，从而避免整个过程呢？

**詹姆斯·博顿利**:让系统处于设置模式等同于当前状态(无安全引导)。然而，我们从微软博客中了解到，接受 Windows 8 预装的用户将无法选择，他们的系统将被锁定。对于希望安装开源软件的用户来说，他们可以选择转移到更安全的用户模式或者保持现状。安装模式的要点是，处理这种选择的复杂性成为操作系统安装或点火系统的工作，我们认为这是最好的地方。我们预计第一批安全引导可能导致的问题将随着时间的推移得到解决，安全引导的好处将超过最初的困难。

**TC** :支持一个完整的公钥基础设施是一个伟大的想法，但远远超出了许多硬件制造商的技术能力。这不是他们的核心竞争力，所以谁说他们会做得好呢？

JB :这不会由硬件制造商来做，实际上考虑到安全隐患，它应该外包给一个对它来说是核心竞争力的实体。微软 Windows 8 徽标提案的当前效果是，原始设备制造商需要管理一系列密钥交换密钥，这也不是他们的核心能力，因此将密钥管理卸载给一个以此为核心业务的实体应该会使整个过程更不容易出错。

正如 DigitNotar 公司最近指出的那样，我们知道认证机构不是不可妥协的。如果安全松懈的硬件制造商受到威胁，最终用户会有什么后果？

**JB** :所以这是个问题。UEFI 系统包含一个撤销证书的机制(与互联网中用于补救 DigiNotar 入侵的机制相同)。然而，依赖于信任路径中被撤销的密钥的系统将拒绝引导，并且将不得不切换出安全模式或者更新其 UFI 来补救这种情况。然而，这种妥协的可能性并不比 OEM 密钥被妥协的可能性更大(而且可能性更小，因为这是 CA 的核心业务利益),所以这个问题与没有 CA 的情况一样，或者麻烦更少。

“初期困难”的承诺听起来并不特别有趣，但正如任何新技术的采用一样，这在很大程度上是不可避免的。我很期待看到安全引导被证明是成功的。