# Firefox 22 发布，内置 Asm.js 和 WebRTC 支持 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/06/25/firefox-22-launches-with-built-in-asm-js-and-webrtc-support/>

Mozilla 今天[发布了](https://web.archive.org/web/20221007092150/https://blog.mozilla.org/blog/2013/06/25/firefox-delivers-3d-gaming-video-calls-and-file-sharing-to-the-web/) [Firefox 22](https://web.archive.org/web/20221007092150/http://www.mozilla.org/en-US/firefox/22.0/releasenotes/) ，这是第一个支持 [WebRTC 协议](https://web.archive.org/web/20221007092150/https://hacks.mozilla.org/2013/06/webrtc-comes-to-firefox/)的流行浏览器的稳定版本，并包括对该组织的 [asm.js JavaScript 子集](https://web.archive.org/web/20221007092150/http://asmjs.org/)的支持，该子集为 web 应用提供了接近本地的性能。

在很大程度上，浏览器发布现在已经成为常规，特别是自从所有主要厂商——除了微软——都转向了快速发布时间表。然而，WebRTC 和 asm.js 都有可能改变开发人员创建 web 应用程序的方式，所以即使你通常忽略 Firefox 版本，这一个也绝对值得一看。

## 内置的 WebRTC 支持

[![Children_call](img/b1acce2109b3eeb9dac5e01755d9e4ce.png) ](https://web.archive.org/web/20221007092150/https://beta.techcrunch.com/wp-content/uploads/2013/06/children_call.png) WebRTC 允许开发人员创建内置视频和音频呼叫的 web 应用，以及文件共享，而无需任何插件或第三方软件。许多公司，例如包括 Tokbox 在内，已经在 WebRTC 上下了大赌注。然而，到目前为止，只有谷歌的 Chrome 在其主流浏览器版本中支持这一新兴标准。现在 Firefox 在其稳定的分支中也支持它，我们可能会看到大量的初创公司和老牌公司更密切地研究这项技术。到目前为止，微软仍然是唯一一个决定对相同功能采用不同标准的主要供应商，但是如果 Internet Explorer 在不久的将来也支持 WebRTC，我也不会感到惊讶。

## 汇编. js

Asm.js 是另一项有潜力改变游戏规则的技术。正如我们在 3 月的[中详细解释的，asm.js 是 JavaScript 的一个子集，在浏览器中以接近本地的速度运行。正如 Mozilla 的 CTO Brendan Eich 当时向我解释的那样，它是一种子语言，“有效地为内存不安全的语言(如 C 或 C++)描述了一种安全的虚拟机。”感谢像](https://web.archive.org/web/20221007092150/https://beta.techcrunch.com/2013/03/21/firefox-nightly-now-includes-odinmonkey-brings-javascript-performance-closer-to-running-at-native-speeds/) [Emscripten](https://web.archive.org/web/20221007092150/http://en.wikipedia.org/wiki/Emscripten) 这样可以编译 C 和 C++代码的工具，asm.js 开发人员也可以使用它来转换他们的 C 和 C++程序，以便在浏览器中运行。Asm.js 目前的性能是本机性能的 2 倍以内，该团队正在努力工作，以进一步加快速度。

你可以通过 Mozilla 的 [BananaBread](https://web.archive.org/web/20221007092150/https://developer.mozilla.org/demos/detail/bananabread) 游戏演示来测试所有这些新功能，该演示使用 WebGL、Emscripten、asm.js 和 WebRTC 来“展示你如何在提供高端 3D 多人游戏的同时，仍然保持快速和令人惊叹的体验。”

版本 22 中的其他小更新包括改进的 WebGL 渲染性能，Mac OS X 上 Dock 应用程序窗口中的下载进度条，以及对 Windows 上高分辨率显示器上显示缩放选项的支持。你可以在这里找到完整的发行说明。