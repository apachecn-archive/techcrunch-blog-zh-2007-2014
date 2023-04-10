# 不要用 FiveRuns 的 TuneUp TechCrunch 单独调试

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/05/29/dont-debug-alone-with-fiveruns-tuneup/>

# 不要用 FiveRuns 的调准单独调试

[![](img/8d3cd6bbfb33525eedb16401a66adb8e.png)](https://web.archive.org/web/20221006050706/http://www.crunchbase.com/company/fiveruns)

随着 Ruby on Rails 爱好者聚集在 [RailsConf 2008](https://web.archive.org/web/20221006050706/http://en.oreilly.com/rails2008/) (以及同时举行的 un-conf[CabooseConf](https://web.archive.org/web/20221006050706/http://conference.caboose.org/))，性能初创公司 [FiveRuns](https://web.archive.org/web/20221006050706/http://www.fiveruns.com/) 正在推出 [TuneUp](https://web.archive.org/web/20221006050706/https://tuneup.fiveruns.com/) ，这是一款针对 Rails 应用程序的“社交”调试工具。

TuneUp 插件会告诉你一个 RoR 应用在哪里运行缓慢。如果你已经编写了一些非常低效的数据库查询，它会指出是哪些。

但是调试并不总是那么简单，所以在一个由谷歌搜索编程答案主导的世界里，TuneUp 做了一些急需的事情。报告机制会将您的报告发送到 TuneUp 的网站上，供其他人查看。每个报告，或者说“运行”,都包含了完整的 Rails 配置、请求的整个执行路径以及总的执行时间。当您发布这些运行时，其他程序员和团队成员可以诊断您的问题并提供潜在的修复。

[![](img/c7aa02658866b980d931f8a876966d9a.png)](https://web.archive.org/web/20221006050706/https://beta.techcrunch.com/wp-content/uploads/2008/05/tuneup_shot.jpg)

TuneUp 有可能消除 Ruby 论坛上详述程序员配置、精确 SQL 查询等的长篇帖子。随着时间的推移(如果 FiveRuns 的结构正确)，TuneUp 可能会形成一个巨大的知识库，其中包含常见的编程问题和错误以及它们的答案。

FiveRuns 属于支持其他 Rails 应用程序的快速增长的 Rails 应用程序类别。 [New Relic](https://web.archive.org/web/20221006050706/http://www.newrelic.com/) 、 [Heroku](https://web.archive.org/web/20221006050706/http://www.heroku.com/) 和 [Engine Yard](https://web.archive.org/web/20221006050706/http://www.engineyard.com/) 是最近进行了大规模风险投资的其他公司。FiveRuns 本身已经从 T21 的 Austin Ventures 筹集了 900 万美元。

观看下面的视频，观看调整的截屏。

[维梅奥·http://www.vimeo.com/1086057 w = 550 & h = 332]