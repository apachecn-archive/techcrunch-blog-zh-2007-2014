# Digg 表示，Diggbar 并不邪恶，它让独立访客增加了 20%

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/04/09/digg-says-diggbar-is-not-evil-and-is-lifting-visitors-by-20-percent/>

# Digg 表示，Diggbar 并不邪恶，并且提升了 20%的独立访客

在关于[网址缩写是否是邪恶的](https://web.archive.org/web/20221006024039/http://www.beta.techcrunch.com/2009/04/06/are-url-shorteners-a-necessary-evil-or-just-evil/)的争论中，一项服务被特别挑了出来:Digg 的[新 Diggbar](https://web.archive.org/web/20221006024039/http://www.beta.techcrunch.com/2009/02/26/digg-is-working-on-a-toolbar-to-go-after-stumbleupon-tinyurl-and-all-the-rest/) 。Diggbar 不仅仅是一个网址缩短器，但这是它的主要功能之一。然而，与其他将人们重定向回被缩写的原始链接(通常是为了发推特)的缩写不同，Diggbar [将流量重定向回 Digg.com。](https://web.archive.org/web/20221006024039/http://www.beta.techcrunch.com/2009/04/02/diggbar-keeps-all-digg-homepage-traffic-on-digg/)

这引起的担忧是，如果很多人开始使用 Diggbar 和它的特殊缩写 URL，Digg 将有效地从被链接的原始网站窃取链接汁液，这将不会从搜索引擎获得他们应得的适当信用。用技术术语来说，Diggbar 产生了一个 200 服务器代码，而不是 301 重定向(丹尼·沙利文[解释了这里的区别)](https://web.archive.org/web/20221006024039/http://searchengineland.com/analysis-which-url-shortening-service-should-you-use-17204)，从表面上看，这似乎不太合适。

但是在今天的一篇帖子中，Digg 工程副总裁 John Quinn 向所有人承诺，Digg 并没有试图窃取任何链接，并且已经采取了额外的措施来确保搜索引擎和其他人对原始链接的信任。何[写](https://web.archive.org/web/20221006024039/http://digg.com/d1oKtU):

*我们采取了几个步骤来确保搜索引擎继续统计原始来源，而不是将 DiggBar 注册为新内容。我们在 Digg 页面上只包含源 URL 的链接，以允许蜘蛛看到源站点的未修改链接。对于有这种偏好的用户，这些链接在 JavaScript 中被改写为短 URL。*

本周早些时候，我们发布了一些额外的更新，以解决 SEO 和出版界对臭名昭著(有时甚至是神秘的)搜索引擎“juice”的一些挥之不去的担忧。我们总是将源 URL 表示为搜索引擎首选的 URL 版本，并使用 meta noindex 标签将 DiggBar 页面排除在搜索索引之外。对于那些对技术细节感兴趣的人，我们还包括 link rel="canonical "信息，以表明原始 URL 是真实的(规范的)版本。附加的 URL 属性，如 PageRank 和相关信号，也会被传输。

因此危机得以避免:网络的链接结构保持完整。咻，现在我可以继续使用 Diggbar 了。我不会孤单。奎因还指出，自从 Diggbar 推出以来，“我们已经看到独立访问者增加了 20%，许多内容提供商在过去的一周里也经历了类似的流量波动。”如果 Diggbar 可以持续这样做，没有人会再抱怨它了——即使网址缩写仍然是邪恶的。

**更新**:也许危机还没有避免。一些[严重的问题](https://web.archive.org/web/20221006024039/http://www.3dogmedia.com/truth-about-diggs-diggbar/)仍然被提出，许多人认为除了 URL 重定向问题，诬陷网站本身就是邪恶的。Daring Fireball 的 John Gruber 非常生气，他[发布了这个代码](https://web.archive.org/web/20221006024039/http://daringfireball.net/2009/04/how_to_block_the_diggbar)来阻止任何网站的 Diggbar。