# GoInstant 的下一章是“多人网络”的开发者平台 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/07/17/goinstants-next-chapter-is-a-developer-platform-for-the-multiplayer-web/>

# GoInstant 的下一章是“多人网络”的开发平台

Salesforce.com 以 7000 万美元收购的初创公司 GoInstant ，推出了一个新的开发者平台，称之为“[多人网络](https://web.archive.org/web/20221006021547/https://www2.goinstant.com/blog/welcome-to-the-multiplayer-web)

该公司作为 Salesforce 内部的一个独立实体运营，使用该术语来描述更多关于共享体验的网络新品牌。这些应用程序，如 Twitter 和脸书，提供了无尽的新闻和评论照片的能力，并看到其他评论。Google Docs 是一个服务的例子，它通过共同编辑功能关注用户的存在。

新的 GoInstant 平台为开发人员提供了一个安全层，通过一个开发人员可以集成到现有或新应用程序中的 API 来管理访问控制、实时消息传递、状态存储和端到端安全。它取代了该公司最初开发的 GoInstant 协同浏览器服务。

“我们的共同浏览产品有一个 API，该服务的主要整体使用是通过 API 进行的，所以我们决定真正专注于这一成功，”联合创始人 Jevon MacDonald 在一次电子邮件采访中说。

[![cylinder_stack](img/081bdf5eff69fe012942b1841ad580ff.png)](https://web.archive.org/web/20221006021547/https://beta.techcrunch.com/2013/07/17/goinstants-next-chapter-is-a-developer-platform-for-the-multiplayer-web/cylinder_stack/)

GoInstant 已经为企业校准了其服务，能够在传统应用程序上放置实时层。它通过其服务堆栈来实现这一点，这些服务旨在提供注重安全的公司在开发现代服务时所需的功能。

通过这项新服务，GoInstant 进入了后端即服务(BaaS)领域。Parse、Firebase、Kinvey 和许多其他公司都在提供后端环境，这样开发人员就不必构建自己的堆栈。联合创始人 Gavin Uhma 在 [Hacker News](https://web.archive.org/web/20221006021547/https://news.ycombinator.com/item?id=6058783) 上写道，它与其他 baa 相比，但区别在于多人游戏概念的这一概念。

> ….GoInstant 专门专注于多人游戏应用。Firebase 和 Parse 都是很棒的产品。它们作为应用程序后端非常有用。GoInstant 完全专注于多用户、实时数据。它补充了你的后端，而不是取代它。我们 API 中的所有决策和概念都是为了让管理用户之间的协作变得非常容易。它完全集中在您为多用户用例开发的思想上，无论是同步还是异步协作。
> 
> 所以，GoInstant 发生的一切都涉及到其他用户。如果您在我们的键/值存储中设置数据或发送消息，其他用户会听到。一切都包装在发布/订阅消息队列中。当您连接或断开连接时，其他用户会知道。当然，你要决定哪些用户会知道，所以我们把用户组组织成“房间”。我们从头开始构建了企业级安全性，因此身份验证、访问控制和加密都非常可靠。

GoInstant 依赖于实时数据以及如何管理这些数据，因此我们可以获得我们习惯的无缝体验。【T2