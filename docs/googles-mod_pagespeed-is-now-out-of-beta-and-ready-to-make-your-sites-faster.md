# 谷歌的 Mod_Pagespeed 现已退出测试，准备让你的网站更快 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/10/10/googles-mod_pagespeed-is-now-out-of-beta-and-ready-to-make-your-sites-faster/>

# 谷歌的 Mod_Pagespeed 现已退出测试，准备让你的网站更快

谷歌刚刚[发布了](https://web.archive.org/web/20221209104100/http://googlewebmastercentral.blogspot.com/2012/10/make-web-faster-with-modpagespeed-now.html)第一个稳定版本的 [mod_pagespeed](https://web.archive.org/web/20221209104100/http://code.google.com/p/modpagespeed/) ，该公司的[开源模块](https://web.archive.org/web/20221209104100/https://developers.google.com/speed/pagespeed/mod)用于 [Apache](https://web.archive.org/web/20221209104100/http://www.apache.org/) 可以自动优化你的网页以提高下载和渲染速度。随着这一版本的发布，谷歌宣布这一工具已经为更广泛的采用做好了准备，尽管值得注意的是，许多大型主机提供商，如 DreamHost，Go Daddy 和内容交付网络 EdgeCast 已经在生产中使用它很长时间了。

Mod_pagespeed 是谷歌让网络更快的众多举措之一。该模块应用多达 40 种不同的优化过滤器。例如，它可以通过自动压缩和调整图像来优化图像。其他优化包括域共享和重写，CSS 和 JavaScript 连接和缩小，以及图像和 JavaScript 的延迟加载。

该公司在 2010 年末推出了模块[，并一直致力于此。谷歌称，使用 mod-pagespeed 通常可以将大型网站的下载时间减半。据谷歌称，mod_pagespeed 目前为大约 120，000 个网站提供支持。](https://web.archive.org/web/20221209104100/http://googlecode.blogspot.com/2010/11/make-your-websites-run-faster.html)

正如 PageSpeed 团队成员乔舒亚·马兰兹和伊利亚·格里戈利克在今天的公告中所指出的，“页面速度是搜索排名和广告质量评分的信号之一”，所以希望在谷歌搜索结果页面上排名靠前的在线出版商应该尝试一下。

顺便说一下，Google 还提供了一个 Google 托管的 CDN 网络的混合体，它也使用 mod_pagespeed 来优化它所服务的网页。然而，PageSpeed 服务目前只接受邀请。

如果你有一个小时的时间可以消磨，下面是对 mod_pagespeed 复杂性的深入探究:

[YouTube http://www.youtube.com/watch?v=6uCAdQSHhmA]