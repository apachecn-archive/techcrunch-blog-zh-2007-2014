# 谷歌敦促伊朗用户在遭受攻击后重新保护 Gmail 账户

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/09/09/google-urges-iranian-users-to-re-secure-gmail-accounts-after-attacks/>

在上周揭露针对伊朗用户的中间人攻击后，谷歌建议伊朗用户采取具体措施，以重新保护他们的 Gmail 账户。攻击者使用了由荷兰的根证书授权机构 DigiNotar 发布的欺诈性 SSL 证书。这些假证书让黑客可以冒充 Google.com 和其他人。

谷歌只是受攻击影响的域名之一。攻击者签署了数百个网站的证书，包括脸书，微软，雅虎！、Tor、Skype、摩萨德、CIA、MI6、LogMeIn、Twitter、Mozilla、AOL 和 WordPress。攻击发生后，荷兰政府发布了一份电子表格，列出了 531 个已知的不良证书。完整的名单在 Tor 网站上的[这里](https://web.archive.org/web/20230205044303/https://blog.torproject.org/blog/diginotar-damage-disclosure)。

尽管谷歌、Mozilla 和其他公司迅速将 DigiNotar 从其网络浏览器的可信权限中移除，但为时已晚，无法保护用户免受已经造成的损害。

谷歌在其博客文章中试图淡化这个问题，声称“Chrome 浏览器的用户受到了保护，免受这种威胁”，但这并不完全准确。在谷歌撤销 DigiNotar 的可信授权后，他们受到了保护，但仍有一段时间用户可能会受到威胁。

对于那些没有采取行动的人来说，威胁可能仍然存在。正如安全研究人员 Graham Cluley 解释的那样，“即使侵入你 Gmail 账户的黑客不再知道你的密码，他们仍然可以做一些事情*而*他们可以访问你的电子邮件，这将允许他们继续监控你的通信。”

出于这个原因，谷歌现在建议伊朗用户采取以下措施来保护他们的账户:

1.  *更改您的密码。当您登录 Google 帐户时，可能已经要求您更改密码。如果没有，可以在这里更改[。](https://web.archive.org/web/20230205044303/https://mail.google.com/support/bin/answer.py?answer=6567)*
2.  *验证您的帐户恢复选项。如果您丢失了密码，辅助电子邮件地址、电话号码和其他信息可以帮助您重新访问您的帐户。检查以确保您的恢复选项是正确的和最新的[这里是](https://web.archive.org/web/20230205044303/http://www.google.com/support/accounts/bin/answer.py?answer=183723)。*
3.  *检查允许访问你账户的网站和应用程序，在此[撤销任何不熟悉的](https://web.archive.org/web/20230205044303/http://www.google.com/support/accounts/bin/answer.py?answer=41236)。*
4.  *检查您的 Gmail 设置，查找可疑的[转发地址](https://web.archive.org/web/20230205044303/https://mail.google.com/support/bin/answer.py?answer=10957)或[委托账户](https://web.archive.org/web/20230205044303/https://mail.google.com/support/bin/answer.py?hl=en&ctx=mail&answer=138350)。*
5.  *密切注意出现在网络浏览器中的[警告，不要点击忽略它们。](https://web.archive.org/web/20230205044303/http://www.google.com/support/chrome/bin/answer.py?answer=95617)*

那些认为自己的账户被攻击的人，可以在这里开始恢复过程。

***更新**:谷歌公关回应称，Chrome 浏览器(和其他浏览器)发出的警告首先改变了公司对该问题的态度。Chrome 用户从一开始就受到保护，除非他们选择点击并忽略浏览器中的“突出的证书警告”。*

显然，这就是为什么谷歌能够做出这样的声明。但事实是，在我看来，如果 Chrome 用户得到了充分保护，就没有必要采取额外的防范措施。Chrome 用户被警告，是的；受保护，不。见鬼，就在上周，我的一个不太懂技术的朋友点击了其中一个警告(与这次攻击无关),很快就感染了病毒。