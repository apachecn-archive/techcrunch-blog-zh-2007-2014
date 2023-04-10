# Gmail 现在真的停机了-我能要回我的邮件吗(更新:它回来了)

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/09/01/gmail-now-really-down-can-i-get-my-email-back-please/>

![picture-3](img/4e1f95ae627a39f87a44f9e946a50576.png "picture-3")

我们[今早](https://web.archive.org/web/20230214102102/https://techcrunch.com/2009/09/01/gmail-hitting-some-turbulence/)报道了 Gmail 遭遇的一些动荡，但现在看来它已经完全崩溃并消失了。域名应用程序和普通消费者 Gmail 服务都完全瘫痪了。谷歌似乎在修复这个问题上倒退了，今天早上他们发出警告说:

`September 1, 2009 8:18:00 AM PDT
Google Mail service has already been restored for some users, and we expect a resolution for all users in the near future. Please note this time frame is an estimate and may change.`

我使用 Domain 的应用程序做任何事情——我的联系人、我的电子邮件、我的待办事项、我的聊天、我的文档，最近还有我的手机。它一倒下，不到一秒钟我就注意到了。几个月来，我对如何在谷歌上运行我的整个生活印象深刻，但现在我完全陷入了困境。
 不仅仅是前端宕机，后端 IMAP 和 POP 服务器也宕机了(**更新**:它们都在运行，但速度很慢)。这对谷歌来说是一个巨大的失败，考虑到他们为扩展应用程序而在内部建立的所有技术是多么令人钦佩。

**更新**:谷歌应用状态[仪表盘显示，目前电子邮件出现“服务中断”。](https://web.archive.org/web/20230214102102/http://www.google.com/appsstatus#di=1&hl=en)

**更新**:停电立即成为推特上的[热门话题，成千上万的用户注意到并抱怨停电。我们今天早上报告的中断并不普遍，但可能指出了一个潜在的根源。](https://web.archive.org/web/20230214102102/http://search.twitter.com/search?q=gmail)

**更新**:还在往下。我想知道有 SLA 的域名用户的付费应用是否也在下降？

**更新**:新状态信息:
 `September 1, 2009 12:53:00 PM PDT
We're aware of a problem with Google Mail affecting a majority of users. The affected users are unable to access Google Mail. We will provide an update by September 1, 2009 1:53:00 PM PDT detailing when we expect to resolve the problem. Please note that this resolution time is an estimate and may change.`

他们一小时后回来(工程师们肯定出去吃午饭了)。

更新:显然 IMAP/POP 已经在某些网站上发布了。正在设置 IMAP …

**更新** : [来自谷歌 Twitter 账户的新消息](https://web.archive.org/web/20230214102102/http://twitter.com/google/status/3695795937):

> 我们知道人们在访问 Gmail 时遇到了问题。我们正在修复它。抱歉给您带来不便

**更新**:对于那些使用网络界面的人来说，如果他们也想用 IMAP 或 POP 获取电子邮件，请参考[或 Rajeev](https://web.archive.org/web/20230214102102/https://techcrunch.com/2009/09/01/gmail-now-really-down-can-i-get-my-email-back-please/#comment-2961079) 的说明。仅在停机前启用了 IMAP/POP 的情况下有效。

> SMTP:smtp.google.com
> (TLS，端口 557，启用认证)
> 
> IMAP:imap.gmail.com
> (启用 SSL，端口 993)
> 
> 登录:user@domain.com

**更新:**现在用 IMAP 下载我的邮件。很慢，但是有点效果。

**更新(太平洋标准时间下午 2:06):**新的更新消息。仍在下降，现在还不知道恢复的预计时间:

> 2009 年 9 月 1 日下午 1:02:00 PDT
> 我们正在继续调查这个问题。我们将在 2009 年 9 月 1 日下午 2:16:00 PDT 之前提供更新，详细说明我们预计解决问题的时间。

**更新**:谷歌已经将[发布到他们的博客:](https://web.archive.org/web/20230214102102/http://gmailblog.blogspot.com/2009/09/todays-gmail-problems.html)

> 我们知道你们中的许多人现在访问 Gmail 有困难——我们也是，我们确实感受到了你们的痛苦。我们通常不会在这里发布小问题(应用状态面板和 Gmail 帮助中心通常是这类信息的去处)。因为这影响到你们中的许多人，我们想让你们知道我们目前正在研究这个问题，并希望不久能有更多的信息在这里分享。如果您已经设置了 IMAP 或 POP，您应该能够同时以这种方式访问您的邮件。对于给您带来的不便，我们深表歉意，并将尽快恢复 Gmail 的运行。