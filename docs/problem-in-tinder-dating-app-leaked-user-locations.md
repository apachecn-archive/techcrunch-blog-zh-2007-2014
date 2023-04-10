# Tinder 约会应用泄露用户位置的问题 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/02/20/problem-in-tinder-dating-app-leaked-user-locations/>

Tinder 是最热门的约会应用之一，它的头条不仅仅是做媒。包括 Sec 在内的一家安全公司最近披露了 Tinder 应用程序中的一个重大问题，该问题可能允许黑客使用高中数学精确定位用户的地理位置。

Tinder 是用来寻找你所在地区想要见面、约会甚至勾搭的人的。尽管每个个人资料都有一个用户定制的页面，但用户主要根据长相来挑选潜在的匹配对象。它展示了一张 Tinder 用户的照片，位置相对较近。喜欢那个人？向右滑动她的照片，寻找潜在的约会对象。不感兴趣？向左滑动。同时隐藏每个人的确切位置。

[https://web.archive.org/web/20221209174149if_/https://www.youtube.com/embed/3E2DwdS_PvQ?feature=oembed](https://web.archive.org/web/20221209174149if_/https://www.youtube.com/embed/3E2DwdS_PvQ?feature=oembed)

视频

这类应用程序被设计为相对匿名，但经过一番挖掘后，这家安全公司发现，该应用程序正在释放遥测数据，当用于对用户进行三角测量时，可以显示该用户在 100 英尺内的位置。完整的利用在这里[解释](https://web.archive.org/web/20221209174149/http://blog.includesecurity.com/2014/02/how-i-was-able-to-track-location-of-any.html)，并在上面的视频中演示。这是第二次发现这样的漏洞。类似的漏洞出现在 2013 年 7 月。

根据 Tinder 公司昨天提供的一份声明，tinder 已经悄悄地修复了这个问题。Tinder 也不知道有人使用最新的漏洞。这就是问题所在。

任何人都可以成为黑客。一个 API 可以用来做的任何事情，它都会被用来做。实现该代码的工程师显然认为它是安全的。大大小小的公司显然不会推出可能被恶意利用的代码。公司的目标是让人们快乐，而不是悲伤。应用程序开发者有责任为其用户提供相对的安全性。如果你的应用仅仅基于你周围人的照片来认识他们，这一点尤其正确。

很可能 Tinder 为了挽回面子，没有公布这个漏洞和修复。该公司已经从去年夏天的[漏洞](https://web.archive.org/web/20221209174149/http://qz.com/107739/tinders-privacy-breach-lasted-much-longer-than-the-company-claimed/)中恢复过来，可能不希望用户再次质疑它的安全性。

Tinder 在这里并不孤单，尽管这种特殊的利用可能会特别糟糕地结束。从 Target 的[大规模数据泄露](https://web.archive.org/web/20221209174149/https://beta.techcrunch.com/2013/12/19/target-confirms-point-of-sale-data-breach-announces-it-exposed-40-million-credit-card-numbers/)到[向黑客开放 Belkin 的 WeMo 设备](https://web.archive.org/web/20221209174149/https://beta.techcrunch.com/2014/02/19/belkin-fixes-wemo-vulnerabilities-with-firmware-update/)的利用，数据安全将继续是一个滚动的问题。为了用户的利益，保护数据是公司的责任。当违规行为发生时，因为它们会继续发生，所以透明是最好的策略。

剩下的唯一问题是接下来哪个应用程序会泄露数据？

在 TechCrunch Disrupt Berlin(视频如下)，Tinder 创始人兼首席执行官肖恩·拉德没有透露确切的用户数量，但提到该应用程序每天有 350 万次匹配和 3.5 亿次点击。(其中大约 30%是表示感兴趣的右击。)该应用程序已经完成了 300 亿次点击和 3 亿次匹配。

## 廷德尔的声明

## 采访 Tinder 创始人兼 TechCrunch Disrupt Berlin 首席执行官