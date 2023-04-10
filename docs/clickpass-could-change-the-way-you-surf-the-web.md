# 将 OpenID 带给大众:click pass 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/03/11/clickpass-could-change-the-way-you-surf-the-web/>

OpenID，一种用一套凭证登录多个网站的方法，有着不可思议的前景。大公司已经签约。[上千家网站](https://web.archive.org/web/20221210002816/http://openiddirectory.com/)走 OpenID 签到。一切都好，对吗？

不完全是。首先，那些大公司只发放身份证，他们还不接受。而 OpenID 的用户体验只是[平平](https://web.archive.org/web/20221210002816/http://marshallk.com/making-openid-easy)差。用户必须记住他们的 OpenID URL，然后被重定向到登录页面。对于那些已经在某个网站拥有账户，但想开始使用 OpenID 的人来说，情况更糟。将这两个账户联系起来并不容易。

这就是今天推出的新创业公司 [Clickpass](https://web.archive.org/web/20221210002816/http://www.clickpass.com/) 的用武之地。我们第一次听说他们是在去年的 Y Combinator 演示日，但是创始人彼得·尼克斯和伊马德·阿克洪德当时并没有说太多。

他们首先是一个 OpenID 发行者。但是他们也试图让用户更容易使用 OpenID。首先，他们与 Plaxo、GetSatisfaction、Pownce 和许多 Y Combinator 创业公司合作。这些网站将显示 ClickPass 按钮，用户只需点击一下就可以通过 OpenID 登录(他们不需要记住自己的 OpenID URL)。如果您是第一次使用 OpenID，Clickpass 会询问您在您尝试登录的服务中是否有现有帐户，并将该信息传回网站以加入帐户。

当您将网站添加到 ClickPass OpenID 时，您会看到它们在 ClickPass 网站上列出。每个网站都会给你一个不同的 OpenID URL，你可以用它来管理多个身份，所有这些都在 ClickPass 上绑定在一起。如果你选择在 ClickPass 上填写个人资料信息，他们会在你加入的新网站上自动填写这些信息。Clickpass 还通过让您选择希望与网站共享的信息类型来确保隐私控制。可以想象，这项服务可以作为你个人数据的一个节点，在不同的网站账户之间进行连接。

简而言之，ClickPass 采用了 OpenID 的技术透明性和开放性，并增加了一层简单性和熟悉性。

[Vidoop](https://web.archive.org/web/20221210002816/http://www.crunchbase.com/company/vidoop) 正在以类似的方式接近 OpenID， [PassPack](https://web.archive.org/web/20221210002816/http://passpack.com/) 是非 OpenID 解决方案。发布时，他们将活跃在黑客新闻、Plaxo、Disqus 上，并通过 WordPress 插件。

![picture-10.png](img/565d54792d36288cea130408a95f48e4.png)用户体验是干净的。登录 Clickpass 后，您只需单击一个按钮即可登录任何启用了 OpenID 的网站。

如果您不想使用 Clickpass 作为您的 ID 提供者，您可以将它链接到任何其他的 OpenID 提供者，但是这将真正违背目的。如果该网站有 OpenID 但没有 Clickpass，您仍然可以使用他们的 Firefox 插件或 Clickpass 的 OpenID url 登录。

当然，任何集中式登录系统都会出现一些问题。这不就意味着小偷只需要偷一个密码，你的 Clickpass 密码吗？联合创始人 Peter Nixey 说我们已经有这个问题了。大多数服务会将忘记的密码转发到你的电子邮件账户，这让雅虎、Hotmail 或 Gmail ( [尤其是现在的](https://web.archive.org/web/20221210002816/http://www.beta.techcrunch.com/2008/03/09/gmail-scam-signal-of-a-much-bigger-security-issue/))成为致命弱点。

至于更有可能的网络钓鱼攻击，Clickpass 计划实施独特的视觉或文字提示(照片或报价)，让你知道你是否被骗了。但总的来说，Clickpass 的目标不是开始保护你的银行账户，而是过多的有用服务提供了大量的个人效用，但对黑客来说没有什么价值(登录 my news.yc 账户不会造成太大损害)。

很明显，OpenID 确实需要这样一个系统来获得广泛采用。这可能是 OpenID 主席斯科特·克韦顿加入 Clickpass 董事会的原因之一。很明显，网络也需要像 Clickpass 这样的东西。