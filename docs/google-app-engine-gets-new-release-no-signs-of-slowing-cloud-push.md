# 谷歌应用引擎获得新版本，没有放缓云推进的迹象 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/06/12/google-app-engine-gets-new-release-no-signs-of-slowing-cloud-push/>

# 谷歌应用引擎获得新版本，没有放缓云推进的迹象

谷歌刚刚推出了带有大量新功能的谷歌应用引擎 1.8.1，其中最引人注目的是期待已久的搜索 API 和推送部署功能，类似于将代码推送到 Git 存储库。

这些新功能是在谷歌繁忙的 I/O 活动之后推出的，该活动见证了该公司有史以来对云服务市场的最大推动。在宣布之前，谷歌一直对谷歌云平台保持沉默。但是现在随着[的全面上市](https://web.archive.org/web/20220930104935/http://www.techmeme.com/130515/p57#a130515p57)，团队正在推出[的每周新功能](https://web.archive.org/web/20220930104935/http://googlecloudplatform.blogspot.com/2013/06/get-your-mobile-application-in-the-cloud-with-mobile-backend-starter.html)和[，以一种前所未有的方式连接组织的不同部分。](https://web.archive.org/web/20220930104935/https://beta.techcrunch.com/2013/06/12/google-launches-cube-slam-an-open-source-pong-clone-to-show-off-the-power-of-webrtc-and-webgl/)

今天，谷歌应用引擎也有了一些新的更新:

**搜索 API:** **自从[搜索 API](https://web.archive.org/web/20220930104935/https://developers.google.com/appengine/docs/features) 发布大约一年后，谷歌已经将其转移到预览阶段——正式发布。Search API 允许开发人员在结构化数据上集成类似 Google 的搜索，比如纯文本、HTML、atom、数字、日期和地理位置。正如我们上周报道的那样，谷歌将开始对运营和存储收费。定价详情可在[这里](https://web.archive.org/web/20220930104935/http://developers.google.com/appengine/docs/billing.html#search_pricing)找到。价格可能会随着供货情况而变化。**

 ****Source Push-to-Deploy:**App Engine 现在支持通过 Git 工具部署 Python 和 PHP 应用程序。开发人员可以像部署 git 库一样轻松地部署应用程序。

**谷歌云存储客户端库:**谷歌正在通过[云存储客户端库](https://web.archive.org/web/20220930104935/https://developers.google.com/appengine/docs/features)的预览版，改善从 App Engine 对[谷歌云存储](https://web.archive.org/web/20220930104935/https://cloud.google.com/storage)的访问。在其博客文章中，谷歌表示，客户端库包含了文件 API 中的大部分功能，但具有更强的完整性保证和更好的整体开发体验。有一些重叠，所以文件 API 将在未来的版本中退役。云存储客户端库将被升级。

任务队列:一个流行的请求，开发者现在可以快速地将任务添加到任何任务队列中，而不会阻塞，这使得开发者的应用程序可以更有效地处理请求。

**数据存储:**谷歌表示，在这个版本中，谷歌云数据存储有两个重大变化。团队已经更改了[数据存储默认自动 ID 策略](https://web.archive.org/web/20220930104935/http://googlecloudplatform.blogspot.com/2013/05/update-on-datastore-auto-ids.html)以使用分散的 ID。此外，NDB 图书馆现在支持“独特的”查询。

1.8.1 的特性和错误修复列表可以在 Google 的[发布说明](https://web.archive.org/web/20220930104935/http://code.google.com/p/googleappengine/w/list)中找到。**