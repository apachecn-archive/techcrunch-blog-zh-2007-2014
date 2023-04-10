# Chrome OS:代码线索就在那里 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/09/01/chrome-os-the-code-clues-are-out-there/>

![screen-shot-2009-09-01-at-50522-am](img/f83bba200c2b816ee2b875b80b1befb1.png "screen-shot-2009-09-01-at-50522-am")一个[雪豹上工作的 Chrome](https://web.archive.org/web/20221006090348/http://www.beta.techcrunch.com/2009/08/31/builds-of-chrome-get-updated-to-show-off-their-snow-leopard-spots/)和 [Chrome 桌面通知](https://web.archive.org/web/20221006090348/http://www.beta.techcrunch.com/2009/09/01/chrome-is-gaining-desktop-notifications/)都很有趣，但是说实话，大家真正想了解的 Chrome 相关信息是 [Chrome OS](https://web.archive.org/web/20221006090348/http://www.beta.techcrunch.com/2009/07/07/google-drops-a-nuclear-bomb-on-microsoft-and-its-made-of-chrome/) 。今天有新闻，因为看起来操作系统可能刚刚向世界展示了自己，如果只是轻微的。

不，我们不是在谈论那些[大图标截图](https://web.archive.org/web/20221006090348/http://www.beta.techcrunch.com/2009/08/31/more-alleged-screenshots-of-google-chrome-os-my-what-big-icons-you-have/)，相反，这种揭示隐藏在代码提交中。

正如你在[这个目录](https://web.archive.org/web/20221006090348/http://src.chromium.org/viewvc/chrome/trunk/src/chrome/browser/chromeos/compact_navigation_bar.cc?view=log)中看到的，有几处提到了“chromeos”几天前，一个@chromium.org 地址的“brettw”写了这样一段话:

> 将紧凑导航栏移动到 chromeos 目录。
> 
> 概括 chromeos 规则，这样我们就不必列出排除的每个文件。

鉴于 Chromium 虽然是开源的，但在很大程度上仍然是谷歌的一个项目，一个@chromium.org 电子邮件地址似乎表明这是谷歌的一名员工。快速浏览一下他一直在做的[工作](https://web.archive.org/web/20221006090348/http://code.google.com/u/brettw@chromium.org/updates)就会发现，它一直都是 Chrome。快速的谷歌搜索显示他是[布雷特·威尔逊](https://web.archive.org/web/20221006090348/http://www.google.com/profiles/brettw)，他是谷歌的一名软件工程师，你可以在谷歌输入输出[这里](https://web.archive.org/web/20221006090348/http://www.youtube.com/watch?v=IiN9fxwjcL0)看到他在工作。

就在那条消息之前，Wilson 更详细地描述了“紧凑导航栏”:

> 修正和增强了紧凑的导航条和状态区域。
> 
> 这使得紧凑的导航栏在 Nicolas 的要求下默认关闭。可以在命令行上使用–compact-nav 来启用它。当此功能启用时，它还添加了
> 不同的标签打开选项。它们可以从状态区的应用菜单中访问
> 。按钮现在延伸到
> 屏幕的顶部，以便于点击。
> 
> 无论紧凑导航栏是否启用，状态区域都会启用。我
> 修复了背景，所以当窗口失去焦点时它会显示为未选中，
> 我还修复了时间格式，使分钟总是 2 位数。
> 
> Chrome 按钮现在已经连接上了，并且只打开了一个占位符页面的标签。

里面有些有趣的东西。看起来 Chrome OS 可能会有一些紧凑的导航栏，有各种标签打开选项(包括点击“Chrome 按钮”)。似乎在所谓的“状态区”中有一个应用程序菜单，其中显然包含了当前时间。

现在，当然这些东西可能与正在开发的新版 Chrome 有关，而不是 Chrome 操作系统。但请记住上面的最新更新(“将紧凑导航栏移动到 chromeos 目录”)，然后看看它之前的那个更新:

> 在紧凑的地址栏和状态栏中添加首次尝试。状态栏
> 包含一个时钟、一个应用菜单和一个非工作电池指示器。
> 紧凑地址栏可以通过 browser_window_gtk.cc 中的 COMPACT_NAV_BAR 进行切换

因此，这个状态栏显然有一个时钟，应用程序菜单，和电池指示器。当然，这些都是 Chrome 操作系统的味道，而不是网络浏览器 Chrome。我在这里只是推测，但似乎有理由假设这个状态栏可能是 Chrome OS 的主上层 dock 的名称。

这很难确定，考虑到所有的代码名和嵌套目录，试图通过 Chromium.org 目录挖掘更多信息就更难了。以下是我挖掘到的更多信息:

本页讨论了与 Chrome 操作系统相关的 cookies。值得注意的是:

> [Chrome OS]增加了启动时注入公司 cookies 的支持
> 
> 为了支持 Chrome OS 的单点登录，我们需要一种将 cookies 注入 Chrome 的方法。
> 
> 最终，我想用 DBus 的适当用法来取代这种管道阅读，但是 Chrome OS 还没有出现。

所以，是的，看起来 Chrome OS 的工作进展顺利，但“还没有”

**更新**:正如评论员 [Daniel Gasienica](https://web.archive.org/web/20221006090348/http://twitter.com/gasi) 指出的，克里斯·梅西纳[昨天自己做了一些调查](https://web.archive.org/web/20221006090348/http://twitter.com/chrismessina/status/3674628722)，似乎已经在谷歌的服务器上找到了[一个可以开发 Chrome 操作系统的区域](https://web.archive.org/web/20221006090348/http://code.google.com/p/chromium-os/?redir=1)。现在你得到一个“403 禁止”，意味着有东西在那里。

*【感谢[赛](https://web.archive.org/web/20221006090348/http://twitter.com/sinkercat)*

*【图片:华纳兄弟】*