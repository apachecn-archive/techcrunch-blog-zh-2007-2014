# 谷歌将原生客户端引入 Chrome，下一代网络应用将紧随其后？

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/08/11/chrome-native-client/>

# 谷歌将原生客户端引入 Chrome，下一代网络应用将紧随其后？

一年多来，谷歌一直在大肆宣传一种名为 Native Client 的东西。这是一项开源技术，允许网络浏览器运行编译后的本地代码。换句话说，这是本地应用和网络应用之间潜在的缺失环节。现在它终于被烤成了铬。

正如谷歌[今天在他们的 Chrome 博客上提到的](https://web.archive.org/web/20230204115845/http://chrome.blogspot.com/2011/08/building-better-web-apps-with-new.html)，Chrome 的最新测试版(版本 14)内置了原生客户端。它们的实现允许在浏览器内部执行 C 和 C++代码，同时保持像 JavaScript 这样的 web 技术提供的安全性。

谷歌写道:

> Native Client 应用程序使用 Pepper，这是一组提供 HTML5 功能的 C 和 C++绑定的接口。因此，开发人员现在可以利用他们的本地代码库和专业知识来交付可移植的高性能 web 应用程序。

这项工作已经进行了很长时间。2010 年 5 月，谷歌在谷歌 I/O 大会上首次开始讨论原生客户端的潜力。今年二月，谷歌[注意到](https://web.archive.org/web/20230204115845/http://blog.chromium.org/2011/02/native-client-getting-ready-for-takeoff.html)Native Client 已经接近现实，他们宣布了一个新的 SDK 供开发者试用。在今年的 I/O 上，[该公司重申了他们的希望](https://web.archive.org/web/20230204115845/https://techcrunch.com/2011/05/11/future-of-chrome/),即它将在今年准备就绪，迎来 Chrome 的未来。

虽然 Native Client 是一个开源项目，但它一直受到 Google 的大力推动。他们不仅自己完成了大量的原生客户端工作，还在 Pepper Plugin API (PPAPI)上做了大量工作，这是大多数当前 web 浏览器使用的 Netscape Plugin API (NPAPI)的演变(IE 除外，它自然有自己的技术)。PPAPI 提供了比 NPAPI 更好的性能，这是让 Native Client 工作的关键。

如果开发者充分利用 Native Client 的优势，所有这些都可以成为下一代网络应用。密集型代码现在可以在本地机器上运行(带有本地代码),同时可以被浏览器实时访问。这将带来更好的网络游戏、媒体等。

谷歌还指出，网络音频 API 也是 Chrome 14 测试版的一部分。这也将有助于通过浏览器开发沉浸式游戏。