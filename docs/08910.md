# 黑客访问会员记录后，诺基亚关闭了开发者论坛

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/29/nokia-shuts-down-developer-forum-after-hacker-accesses-member-records/>

# 黑客访问会员记录后，诺基亚关闭了开发者论坛

作为预防措施，诺基亚暂时关闭了 T2 的开发者社区网站，此前一名黑客获得了包含论坛成员电子邮件地址和其他信息的数据库表。上周，黑客[利用了公告牌软件中的一个漏洞](https://web.archive.org/web/20230204222142/http://www.thehackernews.com/2011/08/nokia-website-hacked-by-pr0tect0r-aka.html)，该漏洞允许 SQL 注入[攻击](https://web.archive.org/web/20230204222142/https://twitter.com/#!/TheHackersNews/status/106769248013127680)，进而使他(或她)能够[破坏](https://web.archive.org/web/20230204222142/http://www.ubergizmo.com/2011/08/nokia-developer-forum-hacked/)论坛网站。

诺基亚现在已经向其所有开发者论坛成员发送了电子邮件，提醒他们不仅网站被篡改，黑客还获得了访问记录的权限，这些记录——对诺基亚来说是幸运的——不包含密码、信用卡详细信息或其他敏感信息。

然而，诺基亚说，大约 7%的被访问记录包括出生日期、网站网址和/或 AIM、ICQ、MSN、Skype 或雅虎等服务的用户名。

当应用程序的数据库层中的用户输入没有被过滤掉转义字符然后被传递到 SQL 语句中时，或者当用户提供的字段不是强类型的或者没有检查类型约束从而意外执行时，通常会发生 SQL 注入攻击。

诺基亚表示，它最初认为只有一小部分论坛成员的记录被访问过，但进一步的调查发现，这个数字“明显更大”——诺基亚没有透露到底有多少记录被访问过，也没有透露任何其他有关安全漏洞的细节。

该公司还表示，在诺基亚的一个团队进行进一步调查和安全评估期间，作为预防措施，它已经关闭了其开发者社区网站。

(谢谢你的提醒，罗伯特)