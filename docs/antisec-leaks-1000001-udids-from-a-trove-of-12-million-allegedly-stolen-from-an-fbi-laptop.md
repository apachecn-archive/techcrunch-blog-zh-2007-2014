# Antisec 泄露了 1，000，001 个 UDIDs，据称这些 UDIDs 是从一台 FBI 笔记本电脑中窃取的

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/09/04/antisec-leaks-1000001-udids-from-a-trove-of-12-million-allegedly-stolen-from-an-fbi-laptop/>

# Antisec 泄露了 1，000，001 个 UDIDs，据称这些 UDIDs 是从一台 FBI 笔记本电脑中窃取的，价值 1，200 万英镑

黑客组织 [Antisec](https://web.archive.org/web/20221006115420/http://en.wikipedia.org/wiki/Operation_AntiSec) 发布了 1，000，001 条与苹果 UDID 身份识别计划相关的数据。这些数据，如果与苹果的开发者资源交叉引用，可能会识别出一个独特的用户的地理位置和其他具体信息。事实上，数据库确实包含设备名称(例如，一个 UDID 指向一个设备名称“hobamain”，并出现在名称“Obama”的搜索中)。

这次泄露据称来自 1200 万个 UDIDs，据称是从监管特别探员克里斯托弗·k·斯坦格尔的戴尔笔记本电脑中窃取的，他出现在[的这段视频](https://web.archive.org/web/20221006115420/http://www.facebook.com/video/video.php?v=512364171294)中，呼吁更多人考虑从事网络安全职业。

你可以在这里阅读关于[黑客以及如何找到数据的详细信息](https://web.archive.org/web/20221006115420/http://pastebin.com/nfVT7b0Z)。

安赛克写道:

在 shell 会话期间，从他的桌面文件夹中下载了一些文件，其中一个名为“NCFTA _ iOS _ 设备 _ 英特尔. csv”的文件变成了 12，367，232 个苹果 iOS 设备的列表，包括唯一设备标识符(UDID)、用户名、设备名称、设备类型、苹果推送通知服务令牌、邮政编码、手机号码、地址等。涉及人员的个人详细信息字段多次显示为空，使得整个列表的许多部分不完整。

你可以使用[这个工具](https://web.archive.org/web/20221006115420/http://kimosabe.net/test.html)查看你的 UDID 是否在列表中，或者你可以从 Antisec 的一个镜像中下载文件。该组织删除了他们拥有的任何识别信息，声称“我们删除了其他个人数据，如全名、手机号码、地址、邮政编码等。”目前，数据相当干净，只提供了 UDID、[推送通知](https://web.archive.org/web/20221006115420/http://developer.apple.com/library/mac/#documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ApplePushService/ApplePushService.html)服务 ID 和设备名称。我已经能够使用快速社交媒体搜索根据这些数据来识别个人，但他们仍然不是直接的一对一标识符。

这些数据很有趣，因为它不一定来自苹果，它在 FBI 机器(或任何地方)上的存在的含义也不清楚。简而言之，所有这些数据都会定期出现在 iOS 应用开发者数据库中，并用于发送推送通知。因此，这似乎最有可能是一个应用程序庞大用户群的数据库转储。因此，任何拥有超过 1200 万用户的应用都会受到质疑。

同样不清楚的是这些数据的安全含义。这是一份客户名单，因此可能包含潜在的破坏性信息。这是坐在，未加密，在任何硬盘驱动器是一个讽刺。它是从联邦调查局的硬盘上被偷的，甚至据称，这是一种暴行。

这能有多糟？程序员和安全大师奥尔多·科特西写道:“我查看了 IOS 上的所有游戏社交网络——基本上是 OpenFeint 及其竞争对手——发现几乎所有人都存在灾难性的管理不善。这些漏洞包括去匿名化、接管用户的游戏社交网络账户，以及仅使用 UDID 就能完全接管用户的脸书和推特账户。”

到底有多糟糕？我们还是不清楚。我们给苹果和其他专家发了电子邮件，但会随着故事的进展关注更新。