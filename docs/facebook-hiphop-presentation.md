# 来自脸书 HipHop 技术品尝会的现场直播 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/02/02/facebook-hiphop-presentation/>

# 脸书 HipHop 技术品尝会现场直播

我现在在脸书技术品尝会上，这个社交网络展示了他们新的开源 PHP 技术， [HipHop](https://web.archive.org/web/20221209173641/http://developers.facebook.com/news.php?blog=1&story=358) 。这项新技术有效地将 PHP 转换成 C++，从而大大节省了 web 服务器的 CPU 周期。脸书正在直播这次活动，我们在下面嵌入了直播流。

脸书高级开放项目经理 David Recordon 为活动拉开了序幕，他带领观众了解了脸书面临的一些挑战，特别是它必须生成的动态页面。他谈到了各种编程语言的一些好处，以及每种语言的 CPU 成本。随着规模的扩大，脸书遇到了 PHP 的问题，包括高 CPU 和内存成本，以及开发人员在构建扩展时面临的困难。但是脸书有很多有才华的 PHP 开发人员，重写网站没有意义。

脸书提出的解决方案是 HipHop for PHP，这是一个名为赵的开发人员的黑客马拉松项目(尽管随着项目的进展，他也有一些团队成员)。该技术将 PHP 转换为 C++，使用 g++进行编译。

脸书发现，在 web 层流量相同的情况下，该技术使用的 CPU 减少了 50%，在 API 层流量翻倍的情况下，该技术使用的 CPU 减少了 30%。

脸书在六个月前开始部署 HipHop(最初只在内部服务器上)。现在，脸书 90%的生产服务器都采用了这种技术。

赵上台做了一个技术性很强的演示，介绍了这项技术的好处(详情请看下面的视频)。

脸书开源开发者倡导者 Scott MacVicar 展示了开源项目的未来路线图。脸书的目标之一:
-赶上 PHP 5.3
-支持 Apache 作为 web 服务器选项
-基于 FB 之外的使用进行发展。

Ustream 的视频聊天室