# GitHub 到底是什么？

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/07/14/what-exactly-is-github-anyway/>

本周，安德森·霍洛维茨宣布向 [GitHub](https://web.archive.org/web/20230220041834/http://github.com/) 投资 1 亿美元。你可以在网上看到关于 GitHub 将如何处理这笔钱的评论和猜测[，这对安德森·霍洛维茨来说是否是一笔好投资，以及接受如此大的投资对 GitHub 来说是否是一件好事。](https://web.archive.org/web/20230220041834/http://www.techmeme.com/120709/p50#a120709p50)

但是 GitHub 到底是什么，为什么开发者对它如此兴奋？你可能听说过 GitHub 是一个代码共享和发布服务，或者它是一个面向程序员的社交网站。这两种说法都是对的，但都没有准确解释 GitHub 的特殊之处。

GitHub 的核心是 Git，这是一个由 Linux 创建者 Linus Torvalds 发起的开源项目。GitHub 的培训师 Matthew McCullough 解释说，Git 和其他版本控制系统一样，管理和存储项目的修订。虽然它主要用于代码，但 McCullough 说 Git 可以用于管理任何其他类型的文件，如 Word 文档或 Final Cut 项目。可以把它想象成一个文件草稿的归档系统。

Git 的一些前身，比如 [CVS](https://web.archive.org/web/20230220041834/http://www.nongnu.org/cvs/) 和 [Subversion](https://web.archive.org/web/20230220041834/http://subversion.tigris.org/) ，有一个与项目相关的所有文件的中央“存储库”。McCullough 解释说，当开发人员进行更改时，这些更改会直接发送到中央存储库。对于像 Git 这样的分布式版本控制系统，如果您想要对一个项目进行更改，您需要将整个存储库复制到您自己的系统中。在本地副本上进行更改，然后将更改“检入”到中央服务器。McCullough 说，这鼓励分享更精细的更改，因为你不必每次做更改时都连接到服务器。

GitHub 是一个 Git 存储库托管服务，但是它增加了许多自己的特性。虽然 Git 是一个命令行工具，但 GitHub 提供了一个基于 Web 的图形界面。它还提供了访问控制和几个协作功能，例如 wikis 和每个项目的基本任务管理工具。

GitHub 的旗舰功能是“分叉”——将一个存储库从一个用户的帐户复制到另一个用户的帐户。这使您能够使用自己的帐户来获取您没有写权限的项目并对其进行修改。如果您做出了想要共享的更改，您可以向原始所有者发送一个名为“提取请求”的通知。然后，用户只需点击一个按钮，就可以将您的回购中的更改与原始回购合并。

这三个特性——fork、pull request 和 merge——使得 GitHub 如此强大。Code School 的 Gregg Pollack(刚刚推出了一个名为 TryGit 的课程)解释说，在 GitHub 之前，如果你想为一个开源项目做贡献，你必须手动下载项目的源代码，在本地进行更改，创建一个名为“补丁”的更改列表，然后通过电子邮件将补丁发送给项目的维护者。然后维护者必须评估这个补丁，可能是一个完全陌生的人发来的，并决定是否合并修改。

波拉克解释说，这就是网络效应在 GitHub 中开始发挥作用的地方。当您提交一个 pull 请求时，项目的维护者可以看到您的个人资料，其中包括您在 GitHub 上的所有贡献。如果您的补丁被接受，您将在原始网站上获得积分，并显示在您的个人资料中。它就像一份简历，帮助维护者决定你的声誉。GitHub 上的人和项目越多，项目维护者对潜在贡献者的了解就越多。补丁也可以公开讨论。

即使对于那些最终没有使用 GitHub 接口的维护者来说，GitHub 也可以让贡献管理变得更加容易。开源开发平台 Node.js 的维护者艾萨克·施鲁特(Isaac Schlueter)说:“我最终只是下载补丁，或者从命令行而不是从合并按钮进行合并。但 GitHub 提供了一个集中的地方，人们可以在那里讨论补丁。”

降低进入门槛使开源开发民主化，并帮助年轻项目成长。“如果没有 GitHub，Node.js 就不会有今天，”Schlueter 说。

除了面向公众的开源库，GitHub 还为企业销售私有库和内部软件实例。这些解决方案显然不能充分利用 GitHub 的网络效应，但它们可以利用协作特性。GitHub 就是这样赚钱的，但它在这个市场上并不孤单。

[Atlassian 在 2010 年收购了一家名为 BitBucket 的竞争对手](https://web.archive.org/web/20230220041834/https://techcrunch.com/2010/09/29/atlassian-buys-mercurial-project-hosting-site-bitbucket/)。今年早些时候，Atlassian 推出了 [Stash](https://web.archive.org/web/20230220041834/http://www.atlassian.com/software/stash/overview) ，这是一款能够让你托管私有的本地 Git 存储库的产品，具有 BitBucket/GitHub 风格的协作特性。该公司还销售开发者协作工具，如 bug 追踪器吉拉和 wiki Confluence。来自 Atlassian 的竞争[在 2010 年](https://web.archive.org/web/20230220041834/https://techcrunch.com/2010/07/14/atlassian-accel-60-million/)从 Accel Partners 获得了 6000 万美元的资金，这可以帮助解释 GitHub 为什么获得这轮资金，并暗示该公司未来可能的发展方向。例如，Schlueter 说 GitHub 的问题跟踪功能最终可能会在一些项目上与 JIRA 竞争。

钱可能在私人和内部托管，但爱是在公共仓库。也许最重要的是，GitHub 已经成为亚历山大的代码示例图书馆。由于 Git 鼓励细粒度的变更记录，程序员，无论是绝对的初学者还是专家，都可以追踪世界上一些最伟大的开发人员的步骤，并找出他们是如何解决棘手问题的。但是，如果 GitHub 遇到了和亚历山大图书馆一样的命运，它可以从分布在世界各地的许多开发者笔记本电脑上的所有本地分支中重建。不管这项投资结果如何，这对 GitHub 团队来说都是一笔巨大的遗产。