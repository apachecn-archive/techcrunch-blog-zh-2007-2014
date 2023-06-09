# 前 Lolapps 工程师推出了 Rollbar，这是一个面向开发者的错误跟踪平台，具有历史感

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/02/26/former-lolapps-engineers-launch-rollbar-an-error-tracking-platform-for-developers-that-has-a-sense-of-history/>

面向开发人员的错误跟踪产品 Rollbar (原名 Ratchet.io)在经过 9 个月的私下测试后，于今天发布了测试版产品。这家新公司由前 Lolapps 工程师创建，灵感来自他们曾经在内部依赖的工具，由来自 [Resolute.vc 的迈克·赫希兰](https://web.archive.org/web/20230223072954/http://www.crunchbase.com/financial-organization/resolute-vc)、KISSmetrics 的[希滕·沙阿](https://web.archive.org/web/20230223072954/http://www.crunchbase.com/person/hiten-shah)和前 Lolapps 首席执行官[阿琼·塞西](https://web.archive.org/web/20230223072954/http://www.crunchbase.com/person/arjun-sethi)的一小轮“种子前”融资(25 万美元以上)提供支持。

这家初创公司由前 Lolapps 首席技术官布莱恩·鲁(Brian Rue)创建，他在 2012 年 3 月与 6waves 合并后离开了该公司。今年 5 月，他开始与 Lolapps 的首批员工之一科里·维罗克(Cory Virok)一起开发现在被称为 Rollbar 的产品。现在，一个位于旧金山的三人团队，该公司正在追求一个有点不太性感但绝对必要的开发基础设施:错误跟踪。

[![Rollbar2](img/9541c5908f9c4f9a974cb7154ceb33d6.png)](https://web.archive.org/web/20230223072954/https://techcrunch.com/2013/02/26/former-lolapps-engineers-launch-rollbar-an-error-tracking-platform-for-developers-that-has-a-sense-of-history/rollbar2/)

Rue 解释说，错误跟踪产品解决的核心问题是，当开发人员编写代码时，他们破坏了很多东西。“使用上一代解决方案，您可以看到日志中发生了什么，并在出现错误时收到电子邮件，”Rue 说。但这种解决方案并不那么有用，因为如果你只收到一封电子邮件，你不知道你以前是否见过这个问题，或者它是否在过去被解决过。你不知道问题的严重性。“所以这个产品的核心部分是把东西组合在一起，这样你就知道每一期的历史，”他说。

有了[滚动条](https://web.archive.org/web/20230223072954/http://rollbar.com/)，当你得到一个警告时，它是可操作的，因为问题要么是新的，要么是已经被重新打开的。您可以深入查看历史记录，以及诸如问题何时开始、是否由某个员工引起、它在什么服务上、它在什么浏览器上、哪些国家受到影响、与它相关联的参数等信息。

【T2![Rollbar3](img/4e4d18702c368ee6fbc270a93ad2e741.png)

Rollbar 与其竞争对手的不同之处在于其严重性级别的概念——该服务提供了从“调试”到“关键”的五个级别。例如，由脸书 API 关闭引起的错误不会被认为是影响系统关键任务部分的问题。

Rollbar 的功能集也相当丰富，支持高级搜索功能、部署跟踪、评论、自动客户支持电子邮件(告诉他们问题已经解决)、取证等。该系统还对什么是异常有很强的理解，并且能够消除重复的错误消息，以便辨别哪些问题彼此不同，哪些应该被认为是相同的。

[![Rollbar4](img/2147bfaf36ae3e00b38d937458a42b8c.png)](https://web.archive.org/web/20230223072954/https://techcrunch.com/2013/02/26/former-lolapps-engineers-launch-rollbar-an-error-tracking-platform-for-developers-that-has-a-sense-of-history/rollbar4/)

Rollbar 的 JSON API 是平台无关的，可以与大多数 web 语言兼容，包括 Ruby、Python、PHP、Node.js、Javascript 和 Flash。iOS 和 Android 支持工作正在进行中，将在几个月后推出。就集成必要的库而言，开发人员可以在大约五分钟内启动并运行。然后，他们可以在在线仪表板中查看数据和通知。这个仪表盘还没有包含自己的工作流程，但是 Rollbar 目前支持与 GitHub Issues、PivotalTracker 和 Asana 的集成。

客户根据使用情况支付滚动条费用，[从每月 12 美元到每月 500 美元](https://web.archive.org/web/20230223072954/http://rollbar.com/pricing)，取决于公司的规模。目前的客户包括许多知名的科技创业公司，包括 MapMyRun、Everest、excellently、CrowdFlower、InstaCart、InstaEDU、Spruce Media、MesssageMe、Homejoy、Bombfell、SocialSci 等。

感兴趣的用户可以[在这里](https://web.archive.org/web/20230223072954/http://rollbar.com/pricing)注册免费试用。