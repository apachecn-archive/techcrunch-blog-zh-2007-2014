# LibreOffice 和 OpenOffice.org:分裂一年后

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/10/07/libreoffice-and-openoffice-org-one-year-after-the-schism/>

早在上个世纪，当我第一次开始使用 Linux 时，最大的挑战之一是缺乏每个 Windows 用户都熟悉的那种像样的生产力套件。唯一真正的选择是 StarOffice，它可以工作，但加载速度慢得令人难以忍受，而且使用起来很麻烦。1999 年，太阳微系统公司收购了 StarOffice 的制造商 StarDivision，并于 2000 年 7 月发布了该套件的源代码。OpenOffice.org 就是这样诞生的，他的意图是提供一个可行的开源软件来替代微软 Office。Sun 于 2010 年被甲骨文收购，此后不久的商业开发正式终止。

对于一个传统的闭源应用程序来说，甲骨文的放弃可能已经是穷途末路了。但是 OpenOffice.org 是在 LGPL 下发布的，即[宽松 GNU 公共许可证](https://web.archive.org/web/20230312035249/http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)。本自由软件许可证明确声明:

> 您可以修改您的库副本或库的任何部分，从而形成基于库的作品，并根据上述第 1 节的条款复制和分发此类修改或作品，前提是您还满足以下所有条件:
> 
> a)修改的作品本身必须是软件库。
> b)您必须使被修改的文件带有显著的声明，说明您已经修改了文件以及任何修改的日期。
> c)您必须根据本许可证的条款将整个作品免费许可给所有第三方。
> d) …

因此，当 Oracle 宣布退出时，OpenOffice.org 社区的热心成员汇集了他们的资源，建立了文档基金会，为 OpenOffice.org 使用的开放源代码的持续开发提供结构和领导。

> 文件基金会是一个开放、独立、自治的精英组织，建立在 OpenOffice.org 社区 10 年的专注工作基础上。TDF 是在这样的信念下创建的，即由独立基金会产生的文化能激发出企业和志愿者贡献者的最大潜能，并将提供最好的免费办公套件。

新产品被称为图书馆办公室。当时，这是现有代码库的一个简单、直接的分支。将执行一个简单的查找和替换操作，用“LibreOffice”替换“OpenOffice.org”的所有实例。

Document Foundation 很快开始将自己与之前的项目治理区分开来。你知道，太阳微系统公司一直要求 OpenOffice.org 的贡献者将他们贡献的版权转让给太阳。从许多方面来说，这是有意义的，并不是什么大不了的事情:它允许一个单一的实体来控制和保护整个作品的版权。但是在许多方面，这种版权的重新分配对于开源合作来说是一种诅咒。此外，作为项目生命周期的唯一仲裁者，Sun 有权以任何理由拒绝贡献。因此，文档基金会明确拒绝了版权再分配的需要，为所有来者敞开了大门，并建立了一个严格的精英模式来评估贡献。

所以文档基金会成立已经一年了。开发活动非常活跃，300 多名开发人员提交了 25，000 多项变更。主要的商业贡献者包括 SuSE、Red Hat 和 Canonical。数百名开发人员贡献了自己的力量，希望改善他们重视的项目。

LibreOffice 的首次稳定发布是在 2011 年 1 月 25 日。从那以后，它已经被下载了 600 多万次，其中 90%是在 Windows 电脑上下载的。LibreOffice 现在是大多数 Linux 发行版的默认生产力套件。Document Foundation 估计，Linux、Mac 和 Windows 操作系统上大约有 2500 万人在使用它。

鉴于大量开发人员从 OpenOffice.org 涌向 LibreOffice，Oracle 最近决定[将 OpenOffice.org 代码捐赠给 Apache 软件基金会](https://web.archive.org/web/20230312035249/http://www.marketwire.com/press-release/statements-on-openofficeorg-contribution-to-apache-nasdaq-orcl-1521400.htm)，这样 ASF 就可以将其作为一个真正的开源项目来管理。老 OpenOffice.org 现在是“[阿帕奇 OpenOffice.org(孵化)](https://web.archive.org/web/20230312035249/http://incubator.apache.org/openofficeorg/)，是[阿帕奇孵化器](https://web.archive.org/web/20230312035249/http://incubator.apache.org/)的一员。

除了甲骨文没有真正捐赠代码，至少不是通常意义上的捐赠；他们也没有转让任何版权。据 Apache Software Foundation 社区开发副总裁 Ross Gardler 称，Oracle“已经授予 Apache 足够的许可，允许其以完全不受阻碍的方式向前发展。在 http://www.apache.org/licenses/software-grant.txt[的](https://web.archive.org/web/20230312035249/http://www.apache.org/licenses/software-grant.txt)我们的标准软件授权协议中描述了本许可证的条款。”

孵化器是一个 Apache 项目，用于确保新项目发展生存所必需的社区牵引力。根据孵化器网站，“所有来自外部组织的代码捐赠和希望加入 Apache 的现有外部项目都通过孵化器进入。”这就是为什么在已经很麻烦的“Apache OpenOffice.org”项目名称上加上“(孵化中)”后缀的原因。OpenOffice.org 域也捐赠给了 Apache，并将在某个时候转移到 Apache 硬件上。目前，它仍然驻留在 Oracle 硬件上。

关于 Apache 项目需要注意的一件重要事情是，它们都使用 [Apache 软件许可证](https://web.archive.org/web/20230312035249/http://www.apache.org/licenses/LICENSE-2.0)。这是一个许可许可证，不包含 GNU 许可证的“版权所有”条款。这意味着阿帕奇 OpenOffice.org 现在是根据美国手语授权，而不是 LGPL。

如果 Sun 没有要求版权转让，那么更改许可证的过程将是一场噩梦:每个个人贡献者都将保留其贡献的版权，并且需要同意许可证的更改。几乎可以肯定的是，对于许可变更至少会有一些阻力，这实际上意味着不会发生许可变更。

不过，这种转变很容易实现，特别是因为 Sun 以前要求对所有贡献进行版权转让:当 Oracle 收购 Sun 时，他们立即获得了所有代码的完整和不受约束的版权所有权，并且版权所有者可以在任何时候重新许可该作品。

今天，尽管他们还没有发布任何东西，但是 Apache OpenOffice.org 项目仍然存在，并且运行良好。他们仍在改进构建过程，并在 Apache 中构建必要的基础设施。他们还参与了知识产权清理:寻找可能与旧 OpenOffice.org 捆绑在一起的第三方 GPL 许可的代码和库，并用 Apache 许可的(或兼容的)代码和库替换它。考虑到 OOo 代码库的规模和复杂性，这是一个令人惊讶的重要任务。

我问 Gardler Apache 是否有任何计划试图在主要的 Linux 发行版中恢复默认生产力套件的地位。他回答说“我们不希望与 LibreOffice 或任何其他开源项目直接竞争。Apache OpenOffice.org 社区有兴趣尽我们所能创建最好的许可个人生产力工具套件。”

“许可授权”条款是关于 LibreOffice 和 Apache OpenOffice.org 讨论中的一个重要条款。LibreOffice 仍然使用 LGPL，尽管该许可证比普通 GPL 更宽松，但仍比 Apache 许可证宽松。加德勒继续澄清道:

> 这意味着 Apache 许可的代码可以在任何下游项目中重用。希望有机会在核心组件上进行合作，以促进 OOo 和所有其他寻求使用 ODF 文档的项目之间的文档交换。

像文档基金会一样，Apache 软件基金会也是一个精英组织，根据参与者贡献的质量给予奖励。

希望参与 Apache OpenOffice.org 的新手可能想看看维基上的[招聘](https://web.archive.org/web/20230312035249/https://cwiki.apache.org/confluence/display/OOOUSERS/Help+Wanted)页面。

图片[Flickr](https://web.archive.org/web/20230312035249/http://www.flickr.com/photos/kmk7702/5979828683/)d