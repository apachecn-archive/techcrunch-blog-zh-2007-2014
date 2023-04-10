# Mac 用户推出自己的 Fusion Drive，并详细介绍您也可以这样做 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/10/31/mac-user-rolls-his-own-fusion-drive-and-details-how-you-can-too/>

# Mac 用户推出了自己的 Fusion Drive，并详细介绍了如何使用它

苹果[上周宣布了 Fusion Drive](https://web.archive.org/web/20221207054904/https://beta.techcrunch.com/2012/10/23/apple-re-introduces-the-hybrid-hard-drive-here-comes-the-fusion-drive/ "Apple Re-Introduces The Hybrid Hard Drive: Here Comes The Fusion Drive") 及其新的 MAC 电脑和 iPad mini，虽然它可能看起来像是一个只有苹果自己才能提供的简单硬件选项，但它实际上更多的是关于 OS X 如何在软件层面处理存储、启动和其他操作。这意味着，正如 Mac 开发者 Patrick Stein 在他的 Tumblr 上证明的那样(通过 [MacRumors](https://web.archive.org/web/20221207054904/http://www.macrumors.com/2012/10/31/apples-new-fusion-drive-works-on-older-macs/) ，你可以在家里用一些终端操作和现有硬件创建自己的 Fusion drive。

在他的测试中，Stein 使用了一个通过 SATA 连接到旧 Mac 电脑的内部 120GB 固态硬盘，以及一个通过 USB 插入的外部 750GB 硬盘。理论上，你也可以使用两个内置驱动器进行同样的设置，但是，如果你使用 OWC 的 data doubler 之类的东西，用第二种存储形式取代旧 MacBook Pro 上的光驱。你必须有一台能够运行 OS X Mountain Lion 的电脑，当然具体来说是 10.8.2 版本，但除此之外，任何类型的固态硬盘或硬盘组合在技术上都应该可以工作。虽然运行一个大的、长期的数据存储组件是通过 Thunderbolt 或 USB 连接的外部驱动器的融合设置不太实际，甚至也不明智(当你必须拔掉插头并移动时会发生什么？)，这可能是老款 IMAC(尽管这可能需要一些严重的手术)、Mac minis 或穷人的 Mac Pro 的一个很好的性能增强器。

关于如何完成这个魔术的全部细节，请查看[斯坦的 Tumblr 帖子](https://web.archive.org/web/20221207054904/http://jollyjinx.tumblr.com/post/34638496292/fusion-drive-on-older-macs-yes-since-apple-has)。请注意，这确实需要您深入终端并使用命令行输入，这对于大多数用户来说是一项非常冒险的任务，但是对于 DIY 类型(有足够的备份)来说，这并不那么具有挑战性。就你将看到的设置而言，OS X 应该会自动将定期访问的数据转移到 SSD，然后在一段时间没有被调用后，将其穿梭回 HDD 进行长期存储。如果你设法让它运行起来，一定要分享你的成果。