# Epic 与 Mozilla 合作将虚幻引擎 4 移植到网络上 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/03/12/epic-partners-with-mozilla-to-port-unreal-engine-4-to-the-web/>

Epic 和 Mozilla 今天[宣布](https://web.archive.org/web/20221205234145/https://blog.mozilla.org/blog/2014/03/12/mozilla-and-epic-preview-unreal-engine-4-running-in-firefox/)他们正在将虚幻引擎 4 移植到网络上。

在去年的游戏开发者大会上，Mozilla [向](https://web.archive.org/web/20221205234145/https://blog.mozilla.org/blog/2013/03/27/mozilla-is-unlocking-the-power-of-the-web-as-a-platform-for-gaming/)展示了运行在浏览器中的虚幻引擎 3 的一个端口，这是许多 AAA 游戏的基础。这对许多开发者来说是一个警钟，因为就在几年前，这种无需插件的浏览器游戏体验似乎是不可能的。

使这一切成为可能的 Mozilla 工具是 [asm.js](https://web.archive.org/web/20221205234145/http://asmjs.org/faq.html) ，该组织的 JavaScript 的[高性能子集，以及能够将 C/C++代码转换成可以在任何浏览器上运行的 asm.js 代码的](https://web.archive.org/web/20221205234145/https://beta.techcrunch.com/2013/03/21/firefox-nightly-now-includes-odinmonkey-brings-javascript-performance-closer-to-running-at-native-speeds/) [Emscripten 编译器](https://web.archive.org/web/20221205234145/https://github.com/kripken/emscripten)。当然，如果没有 WebGL，这些都无法实现。Firefox 现在在其稳定版本中提供了 asm.js 优化[，可以以大约](https://web.archive.org/web/20221205234145/https://beta.techcrunch.com/2013/06/25/firefox-22-launches-with-built-in-asm-js-and-webrtc-support/)[1.5 倍的本机速度](https://web.archive.org/web/20221205234145/https://beta.techcrunch.com/2013/12/21/mozillas-asm-js-gets-another-step-closer-to-native-performance/)运行这段代码(与编译后的 C++代码相比)。

正如 Mozilla 的工程总监和 WebGL 的发明者 Vladimir Vukicevic 告诉我的那样，一年前虚幻引擎 3 演示只是一个技术演示。现在，随着虚幻引擎 4 的推出，Epic 超越了演示，并使网络成为使用其引擎开发游戏的开发者的核心平台。虽然 Epic 和 Mozilla 目前只是展示了在浏览器中运行的引擎演示，但根据 Epic 为开发人员提供的标准条款，它很快就会推出。

Mozilla 首席技术官兼工程 SVP 布伦丹·艾希(Brendan Eich)在今天的一份声明中表示:“这项技术已经达到了这样一个地步，用户可以通过网络链接跳转到的游戏现在几乎与他们可能不得不等待下载和安装的游戏没有什么区别。”。“使用 Emscripten 将 C 和 C++交叉编译为 asm.js，开发人员可以以接近本地的速度运行他们的游戏，因此他们可以像对待任何其他平台一样对待网络。”

这是灵魂和摇摆忍者史诗的视频，这两个演示史诗在今年的游戏开发者大会上展示:

[https://web.archive.org/web/20221205234145if_/https://www.youtube.com/embed/c2uNDlP4RiE?feature=oembed](https://web.archive.org/web/20221205234145if_/https://www.youtube.com/embed/c2uNDlP4RiE?feature=oembed)

视频

当 Mozilla 第一次公开展示 asm.js 时，它的运行速度大约是原生速度的两倍(而且它只在 Firefox 的实验性夜间频道中可用)。Vukicevic 指出，从那时起，该团队改进了编译器，但也增加了缓存，以确保大型应用程序的启动时间不会太长。毕竟，这些应用程序往往依赖于大量的图形和声音资源，而这些必须在游戏运行之前下载。

![soul_ninja](img/726f92fb10a92537acc19d148bae707f.png)展望未来，Mozilla 游戏平台策略师 Martin Best 告诉我，该团队还计划专注于为移动设备优化 asm.js。他认为，开发者需要工具来构建跨平台的应用。“在移动领域，我们和一年前在台式机上的情况差不多，”他说。例如，他承认，对火狐操作系统的支持仍然有些欠缺。然而，他相信随着接下来几周 1.4 版本的发布，该团队将会让 asm.js 和 WebGL 在 Firefox OS 上至少达到最低可行状态。现在移动设备的性能也接近 1.5 倍的本地速度，尽管移动设备的本地速度确实有点慢。不过，该团队为移动设备所做的所有优化也往往会回流到桌面。

新潮娱乐(Trendy Entertainment)的 NomNom games 是一家早期押注 asm.js 的游戏开发商，该公司在 2013 年 12 月展示了其[怪物疯狂](https://web.archive.org/web/20221205234145/http://www.monstermadness.com/)游戏[的首个网络演示。这使它成为第一家发布基于 asm.js 和 WebGL 的商业游戏的公司，该公司的首席技术官杰里米·斯蒂格利茨告诉我，从那以后，它决定将网页版作为其未来战略的核心部分。一半的用户现在都在玩网络版的《疯狂怪物》。](https://web.archive.org/web/20221205234145/https://beta.techcrunch.com/2013/12/12/nomnom-launches-first-plugin-free-commercial-game-based-on-asm-js-and-unreal-engine-3/)

他告诉我，在将游戏从其 C++代码库移植到 asm.js 的过程中，团队遇到的问题与编译器关系不大，而是将图形移植到 WebGL。即便如此，将游戏移植到网络上也花了一周多一点的时间。

他还指出，尽管 Firefox 是目前唯一支持 asm.js 的浏览器，但该团队发现其游戏在 Chrome 上的运行速度约为 60%。这足以使它具有可玩性，鉴于大多数休闲游戏并不使用 100%的处理器能力，也不总是以每秒 60 帧的速度运行，该团队认为网络平台的影响力值得性能权衡。

通过[的本地客户端](https://web.archive.org/web/20221205234145/http://www.chromium.org/nativeclient)，谷歌也在致力于一个旨在为浏览器带来高端 3D 图形的项目。不过，它的方法不同。当 Mozilla 将赌注压在 JavaScript 上时，Google 给了开发者在浏览器中运行他们的原生代码的能力。然而，到目前为止，其他浏览器供应商还没有实现这项技术，即使在 Chrome 中，它也仍然是默认关闭的。