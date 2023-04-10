# 超越 Meteor: Derby 是另一个高速 Node.js 框架 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/07/27/move-over-meteor-derby-is-the-other-high-speed-node-js-framework-in-town/>

# 超越 Meteor: Derby 是另一个高速 Node.js 框架

虽然 Google Docs 中用于构建实时 JavaScript 应用程序的框架, [Meteor](https://web.archive.org/web/20221006095645/http://meteor.com/) 背后的公司刚刚宣布了一轮 1120 万美元的巨额融资，但这并不是唯一的游戏。在本周早些时候我在[的故事](https://web.archive.org/web/20221006095645/https://beta.techcrunch.com/2012/07/25/andreessen-horowitz-keeps-eating-the-software-world-with-11-2-million-investment-in-javascript-framework-company-meteor/)中，我提到了由雅虎开发的框架 [Mojito](https://web.archive.org/web/20221006095645/http://developer.yahoo.com/cocktails/mojito/) 。但是还有一个框架没有引起我的注意，尽管它比 Meteor 存在的时间更长: [Derby](https://web.archive.org/web/20221006095645/http://derbyjs.com/) 。

与 Meteor 和 Mojito 非常相似，Derby 是用于构建实时应用程序的客户端和服务器端 JavaScript 框架。它的同步引擎 [Racer](https://web.archive.org/web/20221006095645/https://github.com/codeparty/racer) 可以独立于 Derby 使用。

[内特·史密斯](https://web.archive.org/web/20221006095645/http://www.linkedin.com/in/nateps)(前谷歌员工)和[布莱恩·野口](https://web.archive.org/web/20221006095645/http://www.linkedin.com/in/briannoguchi)是该框架的核心开发者，也是 stealth startup Lever 的创始人。“我们有一个稳定的财政基础，”史密斯在该项目的谷歌团队上写道。“我们的商业模式与 Meteor 非常不同，我们正在创建一家专注于产品的公司，将继续支持该框架。”另一方面，Meteor 正在作为 Meteor 开发组的主要产品进行开发。

从技术角度来看，一个主要的区别是项目处理服务器端 JavaScript 的方式。这两个项目都在服务器端使用 Node.js，但 Meteor 使用了一个名为 Fibers 的库，它从根本上改变了 Node.js 应用程序的编写方式。默认情况下，Node.js 使用回调，这是一种为非程序员很好解释的编码方法[这里是](https://web.archive.org/web/20221006095645/http://code.danyork.com/2011/01/25/node-js-doctors-offices-and-fast-food-restaurants-understanding-event-driven-programming/)。纤程将回调抽象化，这样开发者可以使用更传统的编程风格。纤程与回调已经成为 Node.js 社区中一个有争议的话题。使用纤程代替回调的支持者声称使用纤程在 Node.js 中编码要容易得多。核心 Node.js 团队[声称](https://web.archive.org/web/20221006095645/http://www.mikealrogers.com/posts/a-vocal-minority.html)社区中只有少数人喜欢纤维。即使是这样，也有可能是不喜欢回调的开发人员被 Node 吓跑了。另一方面，我听说回调模型对 Node.js 的成功至关重要。自从 1995 年引入 JavaScript 语言以来，已经有很多尝试在服务器上运行 JavaScript，但是 Node.js 是第一个真正起飞的。许多失败的服务器端 JavaScript 项目试图将 JavaScript 硬塞进更传统的编程方法中，但是 Node.js 接受了 JavaScript 的异步特性。

有可能两种方法都有存在的空间。 [Tim Caswell](https://web.archive.org/web/20221006095645/http://howtonode.org/) ，cloud 9 IDE[的常驻 Node.js 导师](https://web.archive.org/web/20221006095645/https://c9.io/)，[总结道](https://web.archive.org/web/20221006095645/http://bjouhier.wordpress.com/2012/04/14/node-js-awesome-runtime-and-new-age-javascript-gospel/#comment-227)“我只是建议他们先学习基础知识，一旦他们适应了，就可以随意尝试这些替代工具，而不是教新人永远不要使用这些工具。”

无论如何，这不是一个零和游戏，但有一点将决定这些项目的成功，那就是社区采用。正如 Matt Asay 指出的那样，你不能用风投的钱买下一个社区。对两个社区来说都是早期。Meteor 的[贡献者](https://web.archive.org/web/20221006095645/http://www.ohloh.net/p/derbyjs/contributors/summary)[比 Derby](https://web.archive.org/web/20221006095645/http://www.ohloh.net/p/derbyjs/contributors/summary) 多一些，但是这两个项目都吸引了一些赞助公司之外的贡献者。两者都有小而活跃的邮件列表。