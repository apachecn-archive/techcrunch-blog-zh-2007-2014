# Android(终于)向 WebKit 和 Chromium 迈出了步伐 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/22/android-webkit-chromium/>

# Android(终于)向 WebKit 和 Chromium 迈出了步伐

[为什么 Chrome 不是安卓](https://web.archive.org/web/20230205031516/https://techcrunch.com/2011/05/17/google-chrome-android/)的一部分？这是一个和时间一样古老的问题。或者至少几岁。但是考虑到这两种产品都是由同一家公司谷歌生产的，这就没什么意义了。现在他们终于开始采取措施解决这个问题了。一点点。也许吧。

今天，一群谷歌人[在 WebKit-Dev 小组上宣布了](https://web.archive.org/web/20230205031516/https://lists.webkit.org/pipermail/webkit-dev/2011-August/017738.html)(由谷歌的 Peter Beverloo[转播](https://web.archive.org/web/20230205031516/http://peter.sh/2011/08/download-extension-api-composited-canvas-filling-and-pulseaudio/))，Android 团队现在致力于与 WebKit 社区更紧密地合作。是的，这有点奇怪，一个如此致力于“开放”的产品以前并没有真正与开源社区合作——但是，嘿，迟到总比不到好。

安德烈·波佩斯库写道:

> 我们想给一个关于 Android 上的 WebKit 的更新。不久前，我们开始了 WebKit 的 Android 端口的上游工作。由于各种原因，这项工作比预计的时间要长，而且从未完成。我们意识到，WebKit ToT 中存在的不完整的 Android 端口已经给整个项目带来了相当多的混乱和不便，我们对此感到非常抱歉。

整个故事比表面上看起来要复杂一些。虽然 Android 有自己独立的浏览器，但没有“Chrome”的商标，两者确实共享一些代码。但是它们是不一样的，两个独立的团队在研究每一个。不管出于什么原因，谷歌选择不将 Android 浏览器命名为 Chrome，现在这样做可能会引起一些混乱，因为已经有了 Chrome OS——谷歌开发的另一个与 Android 无关的操作系统。

所以现在发生的事情是这样的:谷歌的 Android 团队将开始提供另一个略有修改的 Android 浏览器版本，这将是完全开源的。可以把它想象成谷歌 Chrome 的 Chromium。特定于 Android 的代码将被删除，想必任何人都可以使用这些代码来构建一个新的基于 WebKit 的移动浏览器。

这些都是科技术语:

> 我们计划首先建立一个 webkit.org 构建机器人，它将使用 Android NDK、SDK 和工具链编译 Chromium 的 Android DRT。我们期望对 Chromium 端口进行合理的小范围修改来实现这一点。我们完全致力于维护 WebKit 的 Chromium 端口的这种新风格，尽快建立并运行一个构建机器人将使这一任务变得更容易。同时，我们将删除现有的不完整的 Android 端口。这包括 WebCore/platform/android 中的 Android 特定代码，以及 PLATFORM(ANDROID)宏守护的任何代码。

让人特别难以理解的是，听起来好像谷歌也计划将这款开源版本的安卓浏览器命名为 Chromium。这将是一种新的口味。也许这并不是那么糟糕，因为已经有了 Windows、OS X 和 Linux 版本(鉴于它们共享的底层操作系统技术，Android 版本将非常接近 Linux 版本)——但所有这些操作系统的成品都被称为 Chrome，在 Android 上它仍然不会被称为 Chrome(至少可以这么认为)。

明白了吗？

是的，这仍然令人困惑，但不管怎样，这是朝着正确方向迈出的可喜的一步。

*【感谢杰森的精彩图片】*