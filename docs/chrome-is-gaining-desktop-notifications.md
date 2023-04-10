# Chrome 获得桌面通知

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/09/01/chrome-is-gaining-desktop-notifications/>

# Chrome 正在获得桌面通知

在 Chromium 的世界里，事情真的开始变得忙碌起来。昨天，我们注意到 Chrome 最新的开发者版本已经为雪豹做好了准备。今天带来了一些其他有趣的消息。

看起来 Chrome 即将获得一个名为桌面通知的新内置功能。一份[概述文件](https://web.archive.org/web/20230314205029/http://dev.chromium.org/developers/design-documents/desktop-notifications)最近被放在 Chromium 开发者网站的设计文件中。基本上，听起来好像有一个 API 允许开发者在用户的桌面区域弹出小消息。我想象这将看起来像 FriendFeed 通知，但那些是通过 Adobe AIR 运行的，这将完全在 WebKit 中运行。

有趣的是，文档指出，对于 Mac OS 用户来说，将会有与这些通知的咆哮集成。它指出:“*在 Mac OS 上，如果安装了 Growl*，图标/标题/文本格式的桌面通知将被路由到 Growl 进行显示。”显然，在 Linux 上，通知同样会通过 DBus 路由。

默认情况下，这些通知现在是关闭的，但是可以使用命令行开关打开。仅仅从这些文档中读到它们，很难确切知道它们将如何被使用，但这可能是网站可以使用的一个潜在的很酷的新功能——或弹出广告 2.0。

*【感谢[赛](https://web.archive.org/web/20230314205029/http://twitter.com/sinkercat)*