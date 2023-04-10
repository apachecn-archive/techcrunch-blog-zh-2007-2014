# Dropbox 如何知道你何时分享了受版权保护的内容(无需实际查看你的内容)

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/03/30/how-dropbox-knows-when-youre-sharing-copyrighted-stuff-without-actually-looking-at-your-stuff/>

昨晚晚些时候，一条推文被广泛传播，显示 DMCA 的一份通知阻止了一个文件在 Dropbox 用户的账户上共享。

截至今天下午，它已经被转发了近 3000 次。

发生了什么事？Dropbox 突然做了一些粗略的事情吗？他们是否突然潜伏在用户的文件夹中，挖掘隐藏在个人文件中的版权材料？

没有。这个系统既不是新的，也不是粗略的。它已经存在[多年了](https://web.archive.org/web/20230326030349/http://www.wpcentral.com/dropbox-reads-your-fileskinda?style_mobile=0)，这大概是反版权侵权系统所能得到的最低调的了。它允许 Dropbox 阻止预先选择的文件在个人之间共享(从而防止 Dropbox 被联邦调查局搜查)，而他们的反侵权系统*根本不知道*你的大部分文件实际上是什么。

**在我们开始之前，有几件事要弄清楚:**

*   一些人将最初的推文解读为，用户私人收存箱中的一个文件已经被 DMCA 屏蔽了。事实并非如此。只有当一个文件在用户与用户之间(或者在互联网上)共享时，DMCA 检查系统才会发挥作用。在这种情况下，会生成一个共享链接，通过 IM 发送。
*   一些人认为原始文件已经从用户的 Dropbox 中删除了——事实也并非如此。Dropbox 只是阻止文件被共享。
*   这条推文的原作者[随后澄清说，他不认为](https://web.archive.org/web/20230326030349/https://twitter.com/darrellwhitelaw/status/450323101868253184) Dropbox 在这里做任何邪恶的事情，他只是觉得这很有趣——他并不打算让它以这种方式传播。

如果你知道“针对黑名单的文件散列”是什么意思，请随意跳过这篇文章的其余部分。Dropbox 会对照禁止列表检查共享文件的哈希，如果匹配，就会阻止共享。

如果这些话对你来说听起来像巫术，请继续读下去。

# 工作原理:

在计算机科学中，有一个非常普遍的概念叫做“哈希”。

它几乎无处不在——从允许网络服务检查你的密码而不必实际存储你的原始密码，到确认一个文件在从一个用户传到另一个用户时没有以某种方式改变。

在这种情况下，哈希函数只是一种算法，它根据输入的内容生成一个唯一的标识符。

哈希通常只是字符串。文件 A 的哈希可能是“4f2900f2fdfaf”，而文件 B 的哈希可能是“dba7b12a19fe9”。Dropbox 的哈希值可能比这个长(允许更多的唯一哈希值)，但是你应该明白。

使用正确实现的散列函数，通过算法运行相同的文件两次将返回相同的标识符——但是即使稍微改变一个文件*完全*也会改变散列。因此，即使只改变文件 A 的几个比特，它的哈希也会变成完全不同的东西，比如“e3c277c771c8e”。

![fingerprint chart](img/2f3ad0bc8ed8f9f88185e8c8f1934405.png)

*(这张图片是通过维基共享的[公共领域图片](https://web.archive.org/web/20230326030349/http://en.wikipedia.org/wiki/File:Fingerprint.svg)的修改版)*

这个标识符可以用来告诉你一个文件是否与另一个文件完全相同，但是这是一条单行道。如果你不知道或者没有一个文件副本来比较，散列不能告诉你原始文件*是什么*。

把散列想象成指纹可能会有所帮助。每个人的指纹都是独一无二的，但它不能用来识别一个人，除非你已经*有*那个人的指纹记录与之进行比较。同样，基于哈希的 DMCA 合规系统也无法辨别什么是文件*，除非它与收到撤销请求的文件*完全相同。**

 *当你上传一个文件到 Dropbox 时，会发生两件事:生成一个散列，然后文件被加密，以防止任何未经授权的用户(无论是黑客还是 Dropbox 的员工)在 Dropbox 的服务器上不小心打开它。

(关于加密的说明:Dropbox 处理加密密钥，所以如果法律要求的话，他们*可以*查看你的文件。他们的系统有适当的检查，既有物理的，也有技术的，以防止员工因一时兴起而去翻你的东西[。)](https://web.archive.org/web/20230326030349/https://www.dropbox.com/help/27/en)

在 Dropbox 的法律团队核实了 DMCA 的投诉后，Dropbox 将该文件的哈希添加到一个大的哈希黑名单中，已知这些哈希对应于他们在法律上不允许共享的文件。当您共享一个文件的链接时，它会根据黑名单检查该文件的哈希。

如果你共享的文件*与版权所有者投诉的文件*完全相同，那么它将被禁止与其他人共享。如果是其他东西——一个新文件，甚至是同一文件的修改版本——基于哈希的反侵权系统不应该知道它在看什么。

换句话说:至少根据他们公开声明的内容，Dropbox 并没有主动扫描你的垃圾来寻找有版权的材料。没有人(甚至没有机器人)听你的 MP3，试图找到热门的泄露的 Fergie 曲目，或者阅读你的哈利波特粉丝集。他们刚刚得到了一个他们不能共享的文件的大列表，并且他们以一种故意无视任何未列入黑名单的文件实际上是什么的方式来识别这些文件。

现在，这并不是说基于哈希的系统没有安全问题。例如，如果政府要求的话，Dropbox 理论上*可以*识别任何在账户上存储了特定文件的用户。但是这同样适用于几乎所有的*基于云的存储系统，在那里用户并不自己处理所有的加密。*

**声明一下，这是 Dropbox 对这条推文的官方评论:**

> 围绕我们如何处理版权通知，一直存在一些问题。我们有时会收到 DMCA 以版权为由删除链接的通知。当我们收到这些时，我们会根据法律对其进行处理，并禁用已识别的链接。我们有一个自动系统，然后防止其他用户使用另一个 Dropbox 链接共享相同的材料。这是通过比较文件散列来完成的。我们不会查看您私人文件夹中的文件，并致力于保护您的资料安全。"*