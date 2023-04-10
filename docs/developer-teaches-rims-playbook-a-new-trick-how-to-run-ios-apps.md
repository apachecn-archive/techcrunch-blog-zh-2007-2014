# 开发者向 RIM 的 PlayBook 传授新技巧:如何运行 iOS 应用 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/06/13/developer-teaches-rims-playbook-a-new-trick-how-to-run-ios-apps/>

# 开发者教给 RIM 的 PlayBook 一个新技巧:如何运行 iOS 应用

【YouTube http://www.youtube.com/watch?v=NcQ_7ALmflE&w=640&h=480]

尽管 RIM 的黑莓 PlayBook 有很多缺点(主要是基于软件的),但作为一款平板电脑，它真的没有那么糟糕，即使 RIM 最终在其中一些产品上损失了一大笔钱。

过去的这个周末，一个名为 [BusinessCat2000](https://web.archive.org/web/20221208132213/http://forums.crackberry.com/news-rumors-f40/real-fake-ios-apps-running-playbook-729197/) 的用户在 CrackBerry 论坛上发布了一个视频(见上图),展示了他的 PlayBook 运行一系列 iOS 应用程序的情况。人们瞠目结舌，合法性受到质疑，各种建议被抛出，但这一壮举最终被证明是真实的。

[CrackBerry](https://web.archive.org/web/20221208132213/http://crackberry.com/developer-gets-ios-apps-running-blackberry-real) 编辑凯文·米查鲁克(Kevin Michaluk)跟进并做了尽职调查，让 BusinessCat 先生加载了其他几个应用程序——即 SketchMobile 和 iMore 应用程序——以证明事情实际上按照它们应该的方式运行，没有任何欺诈行为。开发人员通过了视频形式的测试，但在此之前，他提供了一些关于如何让它工作的见解:

> Playbook 上没有模拟 CPU(尽管它在 Windows 上)。它的工作方式与 WINE 在 Linux 上运行 Windows 应用程序的方式非常相似。app 二进制文件被映射到内存中，导入被解析为指向我自己所需的各种 API 的实现。iOS 实际上已经使用了一些开放的 API，Playbook 也支持这些 API(GL ES 和 OpenAL)。大部分工作是实现所有需要的 objective C 类。应用程序的 ARM 代码按原样运行–PB/I devices 上的 armv6/v7 支持几乎完全相同，代码设计为在 USR 模式下运行。没有 swi、GPIO 访问或任何此类诡计。

除了它自己的应用生态系统，PlayBook 还因其相对新发现的运行 Android 应用程序的能力而获得了一些恶名(只要它们被重新打包并提交给黑莓应用程序世界)，由此看来，这个小平板电脑似乎学会了一个新的精彩的新技巧。

当然，运行几个 iOS 应用程序并不能让 iPad 成功，所以任何人都希望设计出他们的 PlayBook，在 PlayBook 上安装并运行 iOS 应用程序的实际过程仍然需要大量的工作——用了不到一个小时就让 iMore 应用程序在 PlayBook 上运行，但这种过程不太可能被任何人采用，除非是最铁杆的 PlayBook 爱好者。尽管如此，这一新功能令人印象深刻，如果有足够的时间，它可能会成为一个真正的大众喜闻乐见。