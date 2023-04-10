# Adobe 失败的原因以及初创公司可以从哪里入手 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/11/09/why-adobe-failed/>

***编者按**:特约撰稿人本·萨维奇(Ben Savage)是 [Spaceport.io](https://web.archive.org/web/20230203121542/http://spaceport.io/) 的创始人，这是一个面向手机游戏开发者的原生 Javascript 和 HTML5 [平台](https://web.archive.org/web/20230203121542/https://techcrunch.com/2011/04/27/sibblingz-launches-new-version-of-multi-device-social-gaming-platform/)。*

Adobe 已经停止为移动浏览器开发 Flash 播放器插件。

这是移动互联网历史上非常重要的时刻。自 1997 年以来，Flash Player 一直是 web 的重要组成部分。从 flash 游戏到流式视频，再到声音和插座，在线 web 体验中许多最重要和最核心的组件都利用了 Flash Player 技术。

然而，Flash-Player 未能成功过渡到移动网络。

怎么会发生这种事？一家拥有 Adobe 资源的公司怎么可能无法克服这个障碍呢？从 PC 到移动网络的过渡可以说是互联网历史上最重要的转折点之一，对 Adobe 的价值非常明显。答案就在 Flash 播放器本身的历史中。

正如史蒂夫·乔布斯所说:“Flash 是为使用鼠标的电脑设计的”——这是真的。当 Flash 在 90 年代创建时，它的目标平台是 PC。Flash 是为台式电脑设计的，这种电脑有快速的 CPU 和电源线。这是 Adobe 在移动领域遭遇困难的根本原因。

移动设备*不是*一直插着电源。他们不得不依靠小电池，一次需要持续几天。由于这个原因，手机的 CPU 速度更慢，耗电更少。最初的 iPhone 有一个 412 MHz 的 CPU。这大约是 1998 年台式机 CPU 的速度。这基本上是 CPU 速度倒退了 9 年，超过了 Adobe 的 Flash Player 的处理能力。

你看，在 Flash Player 中，*一切*都是在 CPU 中完成的，包括图形。这意味着，如果降低 CPU 速度，就会降低图形性能。

早在 1997 年，当 Flash Player 引擎被创建时，CPU 是所有可用的。直到 2000 年，普通的 PC 电脑才开始获得带有硬件加速转换和光照的 GPU。

GPU 的出现改变了一切。在硬件中进行图形计算比在软件中快几个数量级。除此之外，GPU 能够并行执行多个计算。最初的 iPhone 可以同时进行 16 次计算，新的 A5 芯片(iPad2 和 iPhone 4S)可以进行 128 次计算。最重要的是，GPU 使用更少的功率来完成相同数量的计算。

在过去的 10 年里，AAA 主机游戏开发商与 Nvidia 等公司密切合作，优化视频游戏图形的性能。他们共同创建了像 OpenGL 这样的标准，用于与 GPU 交互，并最大限度地提高系统的图形渲染能力。正是因为这种创新，iPhones 可以运行像“Infinity Blade”这样漂亮的 3D 游戏，而且运行速度很快。现代移动设备中的 GPU 真的很强大，如果你能利用它的话。

那么，为什么 Adobe 没能利用现代 GPU 的力量呢？答案是向后可计算性。Adobe 被历史压得喘不过气来。网络上有数百万个 SWF 文件，来自 Flash 播放器历史上的所有版本。要播放所有这些，Flash Player 需要能够播放 SWF 文件一直到版本 1(我们目前是版本 11)。同样的问题也困扰着 Windows。避免向后兼容问题的唯一方法是与过去决裂，停止支持旧版本，并采用新的格式。

Adobe 已经添加了可以利用 GPU 的新 API(如 stage 3D)，但为了确保旧代码的向后兼容性，他们的整个预先存在的 API 没有*而不是*利用 GPU。这意味着 Flash 开发者*仍然*需要重写他们现有的游戏以获得硬件加速图形。

现在，初创公司通过解决 Adobe 无法解决的问题而蓬勃发展。像为移动网络设计的渲染引擎这样的解决方案*利用 GPU 的能力，实现了高性能的硬件加速图形。初创公司有机会进入并提供与 Adobe 的 ActionScript 3 库相同的 API，因此被 Adobe 冷落的 Flash 开发人员现在有了一个可以称之为家的地方。通过与这些新公司合作，开发人员可以将他们的 Flash 知识和技能带到移动设备上。*

【Adobe 还能成功的地方

Adobe 可能在 Flash Player 插件上失败了，但是他们的艺术创作工具仍然是业界最好的。Photoshop、Illustrator 和 Flash Professional 是创作 2D 作品(矢量和光栅)和动画的最佳选择。全世界数以百万计的艺术家和设计师已经学会了使用这些工具的技能，他们不需要学习任何新的工具来为移动网络创建内容。初创公司将填补 Adobe 留下的空白，并允许开发人员使用这些工具来创建用户界面、角色、动画和其他资产。

Flash 播放器插件的终结是历史的必然结果。Flash 基于 CPU 的架构与移动设备发生了正面冲突。既然 Adobe 已经退出舞台左侧，让我们看看谁猛扑进来。

*图片来源:Flickr/ [亚当·塔特尔](https://web.archive.org/web/20230203121542/http://www.flickr.com/photos/tuttletree/4327201415/)，*