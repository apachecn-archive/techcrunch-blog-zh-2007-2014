# 云监控初创公司 Finally.io 现在允许客户添加规则来测试和横向扩展其基础架构 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2014/02/04/finally-io-rules-dashboard/>

# 云监控初创公司 Finally.io 现在允许客户添加规则来测试和扩展他们的基础架构

去年夏天， [Finally.io](https://web.archive.org/web/20230210015529/https://www.finally.io/) 推出，帮助大量使用云服务的公司监控他们的表现，并在出现问题时做出改变。现在，该公司正在为其服务添加一种全新的方式，允许其客户设置规则，用于测试其云基础设施的弹性，在需要时自动扩展或重启。

该服务的工作原理是让客户输入他们的凭据，并为他们提供一个单一的仪表板，他们可以从其中监控云服务的性能。但有了这项新功能，用户可以轻松地创建一套规则，在服务中断时提供主动自动化。

“我们认为这比监控更重要，”联合创始人卢克·格茨林告诉我。“当你的网站被关闭时得到提醒是一回事，但建立一个修复它的规则是另一回事。这会更有价值。”

这是通过创建规则来完成的，这些规则可用于围绕 Amazon Web Services 产品(包括 EC2、RDS 和 DynamoDB)设置自动化参数。通过设置一系列“如果-这个-那么-那个”场景，it 可以自动执行任务，帮助他们的云服务保持工作，即使是在前所未有的紧急情况下。

通过更新，用户可以在使用率超过一定阈值时，将存储容量自动添加到 RDS 数据库实例中。他们可以停止并重新启动随着时间推移而降级的 EC2 实例，以响应失败的状态检查或 CPU 利用率，所有这些都可以帮助他们避免遭受更严重的故障。

依赖 DynamoDB 的用户也可以使用 Finally.io 根据实际使用情况即时扩大或缩小服务，在流量较高时扩大服务，在流量较低时缩小服务。

这些规则还可以用来测试客户基础设施的弹性。使用类似于[网飞著名的混沌猴](https://web.archive.org/web/20230210015529/https://techcrunch.com/2012/07/30/netflix-open-sources-chaos-monkey-a-tool-designed-to-cause-failure-so-you-can-make-a-stronger-cloud/)的过程，该服务允许用户创建受控场景，允许各种 EC2 实例的随机停止和重启，以查看这是否会破坏他们的基础设施。

最后. io 是由 Gotszling 和 Alex Bendig 创建的[，他们都是 About.me 的早期员工。新功能是根据每个规则覆盖的实例或 DynamoDB 表的数量进行销售的，现在客户可以普遍使用。](https://web.archive.org/web/20230210015529/https://techcrunch.com/2013/07/15/finally-io/)