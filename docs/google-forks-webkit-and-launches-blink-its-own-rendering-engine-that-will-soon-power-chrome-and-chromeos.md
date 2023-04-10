# 谷歌派生出 WebKit，并推出了 Blink，这是一个新的渲染引擎，很快将支持 Chrome

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/04/03/google-forks-webkit-and-launches-blink-its-own-rendering-engine-that-will-soon-power-chrome-and-chromeos/>

谷歌刚刚[宣布](https://web.archive.org/web/20230324232059/http://blog.chromium.org/2013/04/blink-rendering-engine-for-chromium.html)它正在分叉 [WebKit](https://web.archive.org/web/20230324232059/http://www.webkit.org/) 并推出这个分叉为 [Blink](https://web.archive.org/web/20230324232059/http://www.chromium.org/blink) 。正如 Google [描述的那样](https://web.archive.org/web/20230324232059/http://www.chromium.org/blink/developer-faq)，Blink 是“一个包容性的开源社区”和“一个基于 WebKit 的新渲染引擎”，随着时间的推移，它将“自然地向不同的方向发展。”谷歌称，Blink 将是速度和简单的代名词。它将很快从 Chrome 进入各种 Chrome 发布渠道，因此用户将在不久的将来看到第一个 Blink-powered 版本的 Chrome 出现在他们的台式机、手机和平板电脑上。

### “合作太棒了”

正如谷歌的工程副总裁 Linus Upson 和谷歌开放网络平台团队的产品经理 Alex Komoroske 昨天告诉我的那样，fork WebKit 的决定完全是由工程团队推动的，并且完全是基于这样一个事实，即工程师们感到受到 WebKit 生态系统内工作的技术复杂性的限制。Komoroske 指出，在与参与 WebKit 项目的其他公司合作时，“合作非常好”

这个决定显然不是轻易做出的。事实上，正如厄普森在我昨天与他交谈时所强调的那样，关于这一举措，“管理层问了很多尖锐的问题”，但最终做出这一决定是为了降低谷歌渲染引擎朝着团队希望的方向发展的技术复杂性。

### 眨眼:速度和简单

具体来说，Komoroske 指出，Chromium 的多进程架构与 WebKit 的其他部分非常不同(Chromium 是 Chrome 和 Chrome OS 背后的开源项目)。Komoroske 说，必须将谷歌的做事方式与 WebKit 以及 WebKit 其他合作伙伴的所作所为整合在一起，这“让所有人都慢了下来”。

作为一个开源项目，Chromium 和 Blink 都向外部提交者开放，尽管作为这类项目的典型，它们必须被[提名](https://web.archive.org/web/20230324232059/http://dev.chromium.org/getting-involved/become-a-committer)才能成为项目成员。

目前，WebKit 和 Blink 看起来非常相似，但谷歌预计，随着时间的推移，它们将朝着非常不同的方向发展。例如，Komoroske 希望在不同的进程中运行[iframe，但是现在用 WebKit 很难做到这一点。](https://web.archive.org/web/20230324232059/http://www.chromium.org/developers/design-documents/oop-iframes)

不过现在，开发人员不会注意到太多的不同，因为大部分工作将集中在内部架构的改进上。例如，谷歌表示，它将能够“立即删除 7 个构建系统和超过 7000 个文件，包括超过 450 万行。”谷歌表示，随着时间的推移，这将导致“更健康的代码库”，并导致“更稳定和更少的错误”

WebKit 项目是由苹果公司在为其 Safari 浏览器分叉 KDE 项目的开源 [KHTML 引擎](https://web.archive.org/web/20230324232059/http://en.wikipedia.org/wiki/KHTML)后启动的。经过 KHTML 团队和苹果公司的反复讨论，苹果公司在 2005 年宣布将开放 WebKit 源代码，谷歌随后将其应用于 Chrome 浏览器，这是一个不同寻常的举动。有趣的是，在 Chromium 的早期，谷歌实际上使用了 WebKit 的分叉版本，但后来[将其分叉](https://web.archive.org/web/20230324232059/https://groups.google.com/forum/?fromgroups#!topic/chromium-dev/tq6-2Hu_YgE)与项目的其余部分进行了调和。

在这种情况下，值得记住的是，目前构建基于 WebKit 的浏览器的所有不同供应商已经以非常不同的方式实现了它(并且经常使用他们自己的 JavaScript 引擎)。

### Google 在当今 WebKit 开发中的角色

目前，大多数 WebKit 评论者来自谷歌(95 人)，苹果位居第二(59 人)，其次是其他一些公司，包括黑莓、英特尔、诺基亚、三星、Adobe 和网飞。Google 目前还负责 WebKit 存储库的大部分提交，所以看看 Google 退出这个项目会对 WebKit 整体产生怎样的影响会很有趣。正如谷歌发言人今天告诉我的，Blink 团队成员仍然可以“如果他们愿意的话”为 WebKit 做贡献，尽管他们中很少有人会有时间和精力这样做。

### 刚刚转到 WebKit 的 Opera 呢？

几周前，Opera [宣布](https://web.archive.org/web/20230324232059/http://my.opera.com/ODIN/blog/300-million-users-and-move-to-webkit)将停止开发自己的引擎，转而使用[的 WebKit](https://web.archive.org/web/20230324232059/http://my.opera.com/ODIN/blog/300-million-users-and-move-to-webkit) ，采用 Chromium 作为其浏览器的基础。目前还不清楚今天的声明会对 Opera 产生什么影响，但我们已经联系了该公司，要求发表声明。

当 Opera 做出这一举动时，许多开发者担心我们很快会面临 WebKit 单一文化(尤其是在移动网络上)。既然谷歌正在开发 Blink，我们或许可以期待创新的步伐再次加快。事实上，Komoroske 告诉我，鉴于谷歌自己对引擎的实现与其他供应商的实现非常不同，谷歌预计它从 WebKit 的转移也将有助于其他供应商更快地开发 WebKit。

**更新** : *Opera 刚刚给我们发来了以下声明:“我们很高兴看到网络变得越来越开放，越来越易于开发者使用。它是一个快速移动的平台，需要持续快速的更新。在与谷歌的同行进行了一些讨论后，我们期待着为 Blink 这个开源项目做出贡献，就像我们会为任何其他我们认为可以使用我们的投入的开源项目做出贡献一样。”*

### 为什么“眨眼？”

Google 为什么把新的渲染引擎叫做 Blink？厄普森告诉我，这显然意味着这里的重点是速度和简单性。然而，浏览器开发者也倾向于对他们的名字开一点玩笑。例如，Chrome 就是让“chrome”尽可能地消失，他告诉我，blink 是为了让人们想起 90 年代网景导航器推出的古老而令人讨厌的 Blink 标签。