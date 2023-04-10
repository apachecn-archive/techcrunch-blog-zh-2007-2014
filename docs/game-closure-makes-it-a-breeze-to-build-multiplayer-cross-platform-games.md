# 游戏关闭使构建多人、跨平台游戏变得轻而易举 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/02/17/game-closure-makes-it-a-breeze-to-build-multiplayer-cross-platform-games/>

可以公平地说，大多数人喜欢玩实时多人游戏的互动体验，然而令人惊讶的是，今天 App Store 上的大多数游戏都是单人游戏。即使是脸书上流行的社交游戏也无法提供像《光环》这样的经典多人主机游戏的丰富体验。这似乎很大程度上是由于编写多人游戏所需的编码、同步和调试是困难的、耗时的和昂贵的。多平台、多人游戏也是如此。

进入[游戏关闭](https://web.archive.org/web/20221209130756/http://www.gameclosure.com/index.html)。Game Closure 今天在 AOL 的 [SSE Labs 的](https://web.archive.org/web/20221209130756/http://www.crunchbase.com/financial-organization/sse-labs)演示日发布，它是一个智能的新游戏开发环境和 SDK，可以轻松创建、托管和部署基于 HTML5 的跨平台多人游戏，从 iOS、Android 和脸书开始。

Game Closure 本质上是 [Heroku](https://web.archive.org/web/20221209130756/http://heroku.com/) 和 [Appcelerator](https://web.archive.org/web/20221209130756/http://www.appcelerator.com/) 的游戏版本，允许游戏开发者用纯 JavaScript 编写游戏，并使用标准的 HTML5 APIs。初创公司的 SDK 然后编译、部署和加速游戏。不需要插件，只需要一个网页浏览器，任何老浏览器都可以。当你的游戏在移动设备和平板电脑等非浏览器平台上运行时，SDK 会使用 OpenGL 等 API 创建一个实际的原生应用。像他们的竞争对手一样，Game Closure 为开发者提供了他们以极快的速度构建、托管和部署游戏所需的一切。

传统上，游戏玩家在玩游戏时习惯于体验平台锁定。你有你在 Android 上玩的游戏，你在桌面上玩的游戏，还有你的 iPad。开发者也是如此:在编写游戏时，他们通常需要使用根本不同的技术为每个平台创建单独的版本。Game Closure 最酷的地方在于，它允许玩家将实时运行的游戏无缝传输到几乎任何设备上，并为开发者提供了所有工具来快速轻松地跨平台分发。

游戏关闭是米迦勒·卡特、马丁·亨特和汤姆·费尔菲德的项目，他们都有游戏开发的经验。卡特为 HTML5 设计了最初的 WebSocket 协议，亨特之前在 [Meebo](https://web.archive.org/web/20221209130756/http://www.crunchbase.com/product/meebo) 工作，在那里他领导了“Meebo Bar”的开发。亨特目前正在斯坦福大学攻读计算机科学博士学位，研究人机交互。卡特告诉我，尽管这家初创公司目前资金紧张，但由于 SSE 实验室与美国在线的合作，他们最近已经将业务从“地下室壁橱”转移到了帕洛阿尔托的“豪华的美国在线办公室”。我怀疑游戏关闭目前占用了美国在线为 TechCrunch 预留的办公室空间，所以我很高兴看到它得到了很好的利用。

TechCruncher 的同事 MG Siegler [上周写了一篇关于本地应用的整体用户体验如何远远超过基于 HTML5 的应用的帖子](https://web.archive.org/web/20221209130756/https://beta.techcrunch.com/2011/02/09/html5-versus-native-apps/)。卡特告诉我，他同意这一评估；在手机上运行 HTML5 游戏的初步测试中，他发现这些游戏“运行速度比浏览器慢 30 倍”。然而，因为 HTML5 有更丰富的工具和优化，在 HTML5 中开发这些游戏并不复杂。为了解决这个问题，GC SDK 包含了 HTML5 APIs 的本机(非浏览器)实现，为在移动设备上使用而加速，所以正如他们所说，您可以拥有自己的蛋糕并吃掉它。

根据卡特的说法，所有工作室需要做的就是学习如何使用标准的 HTML5 技术，Game Closure 将在每个相关的平台上托管和部署他们的游戏。相当酷。

【YouTube = http://www . YouTube . com/watch？v=k3FPJn26Kqk&w=510&h=385]