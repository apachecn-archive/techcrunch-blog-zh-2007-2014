# 谷歌的罗马尼亚域名被阿尔及利亚黑客 MCA-CRB 篡改。谷歌称:“我们没有被黑客攻击”

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/11/27/googles-romanian-domain-gets-taken-down-by-algerian-hacker-mca-crb/>

![](img/187448a1825d69ef74f1e323f9142db0.png "Google.ro hacked and centered")

看来[巴](https://web.archive.org/web/20221207013119/https://beta.techcrunch.com/2012/11/24/hacking-for-the-sake-of-it-eboz-downed-google-apple-300-other-pakistani-sites-and-many-more-just-to-show-it-can/)并不是主要互联网公司域名被~~黑~~劫持的唯一地方。今天早上， [google.ro](https://web.archive.org/web/20221207013119/http://www.google.ro/) 被接管，功劳被“阿尔及利亚黑客”MCA-CRB，一个连环网站破坏者夺走。据我们的线人说，这个网站看起来像上面的图片至少有一个小时了。我截图的时候还是这个样子~~，虽然现在网站好像已经被全部撤下~~。

现在，它似乎正在慢慢回到正常的谷歌罗马尼亚页面，并被描述为一种可能的“DNS 劫持攻击”(更多内容见下文)。与此同时，谷歌表示，它“没有遭到黑客攻击”，但有人设法将访问者重定向到另一个 Google.ro 网站和“其他几个网址”(完整声明如下。)

Softpedia 报道称，雅虎的网站也发生了同样的事情，但该网站现在对我来说看起来很好。Paypal.ro 也重定向到与 Google.ro 相同的页面，尽管 Paypal 也在 https://www.paypal.com/ro/运营另一个网站。

被黑网站上的文字写着:“由 MCA-CRB /阿尔及利亚黑客”，并给出了三个名字，“所有成员 Sec”——所以可能是许多与 Anonymous 和 LulzSec 相关联的松散黑客组织之一。“S thanks = Mr-AdeL & I-Hmx & lag ripe-Dz 全体会员 Sec，”页面上写道。

马华 DRB 也威胁更多。“未完待续……”网站上说。

这似乎不是一个空洞的威胁。根据 Zone-h 被黑网站的记录，MCA-DRB 迄今已对[5530 个网站被黑和篡改](https://web.archive.org/web/20221207013119/http://www.zone-h.org/archive/notifier=MCA-CRB)负责，其中许多似乎涵盖了来自亚洲、非洲、欧洲、澳洲和美洲各国的政府和公共服务网站。相比之下，h 区有 313 个网站归 Eboz 所有，还不算上周末的 284 个。

有趣的是，这似乎并不是在所有地方都发生的。我的同事 Drew 从他在加州的电脑上发给我 Google.ro 的截图，看起来一切正常:

![](img/d3dbd3569608951bae0ab22729b1945d.png "Google.ro in USA")

这似乎不同于本周末在巴基斯坦的丑化行动，在巴基斯坦，284 个网站被一个名叫 Eboz 的黑客关闭。那次攻击似乎与该国域名注册机构 PKNIC 的渗透有关，所有受影响的域名服务器都被重定向到 Freehostia 托管的服务器。但是根据[目前对 Google.ro](https://web.archive.org/web/20221207013119/http://whois.marcaria.com/domain-whois/Europe/Romania-domain-RO/) 的检查，该网站仍将使用谷歌域名服务器。

我们正在联系谷歌进行评论，并将更新这个故事。【更新如下。]

**更新**:卡巴斯基实验室专家 Stefan Tanase 在 [Securelist](https://web.archive.org/web/20221207013119/http://www.securelist.com/en/blog/208194028/Google_ro_and_other_RO_domains_victims_of_a_DNS_hijacking_attack) 撰文指出，该事件可能是由于“DNS 劫持”攻击。他指出，“两个域名都解析到位于荷兰的 IP 地址，”在**95.128.3.172**(server 1 . joomlapartner . nl)，“所以看起来更像是 DNS 中毒攻击。”

与此同时，谷歌表示，它没有遭到黑客攻击。

“谷歌在罗马尼亚的服务没有遭到黑客攻击。在很短的一段时间内，一些访问 www.google.ro 和其他一些网址的用户被重定向到不同的网站。我们正在与罗马尼亚负责管理域名的组织联系，”一位发言人告诉 TechCrunch。

**马里乌斯 m**