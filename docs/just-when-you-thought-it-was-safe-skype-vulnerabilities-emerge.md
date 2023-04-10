# 就在你认为安全的时候:Skype 漏洞出现 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/07/15/just-when-you-thought-it-was-safe-skype-vulnerabilities-emerge/>

# 就在你认为它是安全的时候:Skype 漏洞出现了

愚蠢的黑客总是试图破坏互联网，他们已经找到了另一个目标，即流行的网络电话软件 Skype。根据[有史以来最甜的文字安全报告](https://web.archive.org/web/20230204155849/http://www.noptrix.net/advisories/skype_xss.txt)，链接自 [h-online 的摘要](https://web.archive.org/web/20230204155849/http://www.h-online.com/security/news/item/Vulnerability-in-Skype-allows-accounts-to-be-hijacked-Update-1279864.html):

> “由于缺乏对‘手机’档案条目的输入验证和输出净化的
> , Skype 存在持续的跨站脚本漏洞。
> 其他输入字段也可能受到影响。”

我喜欢这个——输出净化。基本上，这意味着攻击者可以在他或她的个人资料描述的移动电话字段中嵌入 JavaScript。Skype 不过滤该字段，这意味着攻击者的联系人登录时可以执行该 JavaScript。从那里，各种不好的事情都可能发生，如帐户访问，甚至系统级访问。根据 Levent Kayan 的说法，当前版本的 Skype 受到影响(ver。5.3.0.120 ), Skype 已经意识到了这个问题，应该会在下周发布补丁。Skype 对这个问题有点轻描淡写，指出“攻击者必须出现在受害者的经常联系列表中”，以便利用这个安全问题。

这个故事的寓意是什么？下周之前，请记住，你在海外的岳母(你经常和她用 Skype 聊天)现在可能会破坏你的系统，把你拖垮！当心！

[通过[H 安全](https://web.archive.org/web/20230204155849/http://www.h-online.com/security/news/item/Vulnerability-in-Skype-allows-accounts-to-be-hijacked-Update-1279864.html)