# 证实:Snapchat 黑客不是骗局，460 万用户名和号码被公布

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/12/31/hackers-claim-to-publish-list-of-4-6m-snapchat-usernames-and-numbers/>

一个名为 [SnapchatDB.info](https://web.archive.org/web/20230326025834/http://www.snapchatdb.info/) 的网站保存了 460 万个账户的用户名和电话号码，并提供下载。在给我们的一份声明中，SnapchatDB 表示，它通过最近发现并修补的 Snapchat 漏洞获得了这些信息，并提供这些数据，以努力说服这款即时通讯应用加强其安全性。我们还接触了 Snapchat。

SnapchatDB 说:

> 我们发布的动机是提高公众对这一问题的认识，并向 Snapchat 施加公众压力，以修复这一漏洞。科技初创公司资源有限是可以理解的，但安全和隐私不应成为次要目标。安全性和用户体验一样重要。
> 
> 我们使用了 gibsonsec 漏洞/方法的修改版本。Snapchat
> 本可以通过回复 Gibsonsec 的私人通信来轻松避免这一披露，但他们没有这么做。即使在那次披露之后很久，Snapchat 也不愿意采取必要的措施来保护用户数据。一旦我们开始大规模刮，他们决定实施非常小的障碍，这仍然远远不够。即使现在，这种利用仍然存在。大规模刮这个数据还是有可能的。他们最近的变化仍然不难规避。
> 
> 我们希望最大限度地减少垃圾邮件和滥用可能会出现在这个版本。我们的主要目标是让公众意识到许多互联网公司对用户信息是多么不顾后果。对他们来说，这是次要目标，不应该如此。你不会想去一家花费数百万装修，却几乎不注重清洁的餐厅吃饭。

早些时候，我们猜测 SnapchatDB 可能是一个恶作剧，旨在引起人们对该应用安全问题的关注，但事实证明，这是真的——至少我们编辑团队的一名成员受到了影响。一位读者还告诉我们，他在列表中找到了自己的号码，以及几个朋友和 Snapchat 创始人埃文·斯皮格尔的号码。在[黑客新闻](https://web.archive.org/web/20230326025834/https://news.ycombinator.com/item?id=6993968)上，有几个人在下载数据文件时遇到了麻烦(我刚刚收到了他们两个的错误信息，但那可能是因为高流量)，但一位看到列表的[越狱 subreddit](https://web.archive.org/web/20230326025834/http://www.reddit.com/r/jailbreak/comments/1u53oh/off_snapchat_got_hacked_all_username_and_phone/) 用户表示，迄今为止只有美国部分地区的数字被公布。如果你还没能下载名单，你可以[使用这个由开发者](https://web.archive.org/web/20230326025834/http://robbiet.us/snapchat/) [Robbie Trencheny](https://web.archive.org/web/20230326025834/https://twitter.com/Robbie) 创建的网站来看看你的用户名是否被包括在内。

SnapchatDB 表示，它“审查了电话号码的最后两位数”，以“最大限度地减少垃圾邮件和滥用”，但它仍可能发布未经过滤的数据，包括数百万个电话号码。

Next Web 在 SnapchatDB 的域名上做了 WHOIS 查询，发现它是昨天 12 月 31 日创建的。注册人的姓名受到保护，但其邮寄地址和联系电话都列在巴拿马。

该网站似乎是为了应对最近发现的 Snapchat 安全漏洞而创建的。上周， [ZDNet 发表了一篇文章](https://web.archive.org/web/20230326025834/http://www.zdnet.com/researchers-publish-snapchat-code-allowing-phone-number-matching-after-exploit-disclosures-ignored-7000024629/)，讲述了白帽 Gibson 安全研究人员如何试图提醒 Snapchat 黑客将用户名与电话号码联系起来进行跟踪的方法，但都被忽视了。Gibson Security 然后[在平安夜](https://web.archive.org/web/20230326025834/http://gibsonsec.org/snapchat/fulldisclosure/)上公开了这个漏洞。

该公司表示，黑客可以利用两个漏洞，通过 Snapchat 的 Android 和 iOS API 获取用户的个人数据，包括他们的真实姓名、用户名和电话号码。Snapchat 确实发表了一份公开声明，但正如 TechCrunch 的 Josh Constine 所写的那样，这并不令人满意，因为它没有提供其对策如何工作的细节，如速率限制、不良 IP 阻止或扫描可疑活动的自动系统。Snapchat 表示:

> “从理论上讲，如果有人能够上传大量的电话号码，比如区号中的每个号码，或者美国的每个可能的号码，他们就可以创建一个结果数据库，并通过这种方式将用户名与电话号码匹配起来。在过去的一年里，我们实施了各种保护措施，使之变得更加困难。”

Gibson 安全报告和 SnapchatDB 都提醒人们，即使是在短暂的信息服务中，对你用应用程序存储的信息产生安全感也是错误的。SnapchatDB 在网站上表示:“人们倾向于在网上使用相同的用户名，所以你可以使用这些信息来查找与脸书和推特账户相关的电话号码信息，或者只是找出你希望联系的人的电话号码。”。