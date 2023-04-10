# IBM 开源是不是在吹毛求疵？–

> 原文：<https://web.archive.org/web/http://techcrunch.com/2010/04/08/is-ibm-splitting-hairs-with-open-source/>

众所周知，我是一个超级自由软件迷。众所周知，IBM 是一家巨擘，其资金之多超乎我的想象。因此，2005 年，当 [IBM、](https://web.archive.org/web/20191222140050/https://crunchbase.com/organization/ibm) 以明显的公关噱头与开源社区建立伙伴关系，发表了[声明，声明不对 OSS](https://web.archive.org/web/20191222140050/https://beta.techcrunch.com/wp-content/uploads/2010/04/pledgedpatents.pdf) 使用指定专利，表面上说它将允许开源项目使用这些专利所涵盖的任何项目，而没有被罚款或起诉的风险时，我感到非常高兴。耶！最后，BigCo *得到它*并且做正确的事情！但五年是很长的时间，人来人往，承诺可以忘记。IBM 最近威胁要起诉某人侵犯了许多 IBM 专利，包括至少两项包含在非断言声明中的专利。

为了更好地了解这种情况，请查看 Ars Technica 的 [IBM 打破 OSS 专利承诺，瞄准大型机仿真器](https://web.archive.org/web/20191222140050/http://arstechnica.com/open-source/news/2010/04/ibm-breaks-oss-patent-promise-targets-mainframe-emulator.ars)。对 IBM 来说，事情看起来相当暗淡:他们正在使用他们承诺不会使用的两项专利。但这是板上钉钉的事吗？

Ars 文章称 IBM 正在起诉 [TurboHercules](https://web.archive.org/web/20191222140050/http://www.turbohercules.com/) ，提供*支持*的人在 [Hercules 模拟器](https://web.archive.org/web/20191222140050/http://www.hercules-390.org/)上。我想我们都同意，这与针对模拟器本身是非常不同的事情。

Florian Mueller 发表了一篇很长的博客文章， [IBM 打破了禁忌，背叛了它对 FOSS 社区的承诺](https://web.archive.org/web/20191222140050/http://fosspatents.blogspot.com/2010/04/ibm-breaks-taboo-and-betrays-its.html)，他在文章中提出了一些合理的观点，并认为 IBM 的非断言声明完全是一派胡言。

Linux 基金会的执行董事吉姆·泽姆林决定向 IBM 的开放系统开发副总裁丹·弗莱请教这个问题。在一篇名为 [IBM 的开源专利保证](https://web.archive.org/web/20191222140050/http://www.linux-foundation.org/weblogs/jzemlin/2010/04/07/ibms-open-source-patent-pledge/)的博客文章中，泽姆林分享了弗莱的回复，这让我对事情有了更进一步的了解。根据弗莱的说法，

> 这一承诺将有利于任何开源软件。开放源代码软件是任何计算机软件程序，其源代码已经发布，可供任何人检查和使用，并根据许可协议提供，许可协议允许接受者复制、修改和分发程序的源代码，无需支付费用或版税。截至 2005 年 1 月 11 日，所有由 opensource.org 认证并在其网站上列出的许可证都是出于本承诺目的的开源软件许可证。

我认为，IBM 的声明提到了在特定时间点上批准的许可证的外部列表，而不是包括当时批准的许可证的当前列表，这在一定程度上说明了问题。那份文件中列举的*五百*项专利又有什么十几二十行呢？我认为很明显，IBM 在为自己打造某种出路。

查看 Hercules 页面，它似乎是根据 [Q 公共许可证](https://web.archive.org/web/20191222140050/http://www.hercules-390.org/herclic.html)授权的，也称为“Qt 公共许可证”。 [QPL](https://web.archive.org/web/20191222140050/http://www.opensource.org/licenses/qtpl.php) 包含在 [OSI 批准的许可证](https://web.archive.org/web/20191222140050/http://www.opensource.org/licenses/alphabetical)列表中，尽管我真的很难找到那个许可证是什么时候被 OSI 批准的。如果 QPL 在 2005 年 1 月 11 日之后被 OSI 承认，那么 IBM 将有权利用非声明协议中列出的专利。虽然他们有权利这么做，但这仍然是一个愚蠢的举动。

更有可能的是，我认为这里正在发生的是两件事之一。要么是律师们在创建用来威胁 TurboHercules 的非排他性专利清单时有点过于兴奋，包括了非断言声明所涵盖的两项专利；或者 IBM 认为他们可以起诉*公司*侵犯专利，而不是开源项目本身。我猜是后者。