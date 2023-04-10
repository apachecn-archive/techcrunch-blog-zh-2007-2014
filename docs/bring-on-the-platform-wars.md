# 带来平台战争！

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/03/09/bring-on-the-platform-wars/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

以前写软件很简单。提醒你，这是个大麻烦，但很简单。你是微软的开发人员，带着装满 Visual Studio CDs 的活页夹；你是一名 Java 开发人员；你用了[灯堆](https://web.archive.org/web/20230328231541/http://en.wikipedia.org/wiki/LAMP_%28software_bundle%29)；或者你使用 IBM 或 SAP 或类似公司的专有产品。

然而现在，尽管我们使用的工具和技术已经有了巨大的进步……想象一下，上帝保佑，你正在构建某种 web 服务。你应该使用 Ruby on Rails 吗？Node.js？Python 和 Django？PHP 和 Drupal？。网？任何 Java 服务器的全景图？像 Go 或 Scala 这样又新又酷的东西？你将如何/在哪里*托管*你的代码？亚马逊？Heroku？App 引擎？Joyent？EngineYard？Force.com？你的 app 怎么样？你会有一个应用程序，对吗？在哪些平台上？原生代码？混合 HTML5？与 [Xamarin](https://web.archive.org/web/20230328231541/http://xamarin.com/) 交叉编译？然后是你的[数据库](https://web.archive.org/web/20230328231541/https://techcrunch.com/2013/01/19/your-database-is-probably-terrible/) …

头脑因[分析麻痹](https://web.archive.org/web/20230328231541/http://en.wikipedia.org/wiki/Analysis_paralysis)而胡言乱语。这几乎足以让我怀念过去微软一家独大的日子。一个平庸的标准比一个被分割成十几个优秀片段的行业更好吗？一个单一的威权政府比十几个陷入永久内战的城邦更有利于其公民吗？等等，更好的软件不是应该让生活更简单吗？

问题是，如今每个人都想成为一个平台，但没有一个可用的选项明显优于其他选项。

考虑一下 [Heroku](https://web.archive.org/web/20230328231541/http://www.heroku.com/) 。我是他们的超级粉丝。[我们](https://web.archive.org/web/20230328231541/http://www.happyfuncorp.com/)用它们做了大量的项目——像 [TeePublic](https://web.archive.org/web/20230328231541/https://teepublic.com/) 、 [Travtap](https://web.archive.org/web/20230328231541/https://www.travtap.com/) 、 [Postography](https://web.archive.org/web/20230328231541/http://www.postography.com/) 等初创公司。，对于较大的客户也是如此。Heroku 最初是一个 Ruby On Rails 服务，但是[现在](https://web.archive.org/web/20230328231541/https://devcenter.heroku.com/articles/cedar)他们支持 Node.js、PHP、Python 等。他们提供免费层。部署到服务器就像输入“git push heroku master”一样简单数据库连接、电子邮件服务等附加服务。等等。等等。几乎是自动的。和他们一起工作是一种享受。

但是它们很贵；他们似乎没有扩展到真正的大型网站；时不时地，您仍然会遇到一些难以理解和棘手的配置错误，需要花费数天时间来调试；他们并没有因为最近的 RapGenius 争议而给自己带来荣耀。很遗憾地说，我对 Heroku 的爱已经随着时间的推移而减弱了。

然后是谷歌应用引擎。我爱 GAE。你可以通过我在上面构建我所有的宠物项目来判断——例如 [ScanVine](https://web.archive.org/web/20230328231541/http://www.scanvine.com/) 、[wiki sheppa](https://web.archive.org/web/20230328231541/http://www.wikisherpa.com/)、 [ePubHost](https://web.archive.org/web/20230328231541/https://github.com/rezendi/epubhub) 。它使测试、部署和版本控制变得轻而易举。它提供了一整套真正强大的工具(例如，异步任务，Heroku 的头疼事，GAE 的小菜一碟；还有实验性的全文搜索和 MapReduce 工具。)它过去只给你谷歌强大但古怪的 BigTable 数据存储作为选项，但现在你可以轻松地插入云 SQL。它提供了一个非常强大的免费层，你可以用 Java、Python 或 Go 编写你的代码。

可能会很贵，但这不是问题。问题是*没有其他人给你这些工具*。(在开源同源软件方面有一些半心半意的尝试，但它们离黄金时间还有很长的路要走。)所以一旦你开始编写使用它们的代码——你会的，因为它们真的很强大，真的很容易使用——你就被困在 GAE 了…

…出于某种原因，这种观念让经理和高管们*发疯*。如果你问我的话，我觉得这没有任何意义。是的，我认为有一个*风险*谷歌会放弃它的旗舰网络平台，或者把价格提高到惩罚性的水平；但是与所有其他的商业风险相比，这在我看来微不足道，而优势却是显著的。但对于一个又一个客户来说，这一事实让 GAE 完全没有希望。

还有很多其他的选择。微软在它的 Azure 平台上押了大赌注。例如，我非常喜欢将[解析为一个简单而强大的 Android 和 iOS 应用内置后端。(它比我不得不使用的一次叫做 RestKit 的恐怖软件要好大约 10 亿倍。不寒而栗。)如果用 Parse，完全不用自己写后端服务器！…当然，另一方面，如果您需要一个后端服务器来做一些不太有趣的事情，那么您现在就不走运了。但是对于简单的应用程序，这是一个很好的解决方案。](https://web.archive.org/web/20230328231541/https://parse.com/)

还有很多其他的平台，上面我提到了一些。如果你使用好的，你可以用更少的开发人员更快地完成更多的工作。

但是由于这样或那样的原因——其中一个原因是成本——所以许多项目不断退回到基础设施服务，如 [Amazon Web Services](https://web.archive.org/web/20230328231541/http://aws.amazon.com/) ,在这种情况下，不是简单地部署到云而不太关心接下来会发生什么，而是必须提供运行 Linux 或 Windows 的单个服务器，并像配置自己的机器一样配置它们。

应用引擎还没有真正起飞，所以谷歌推出了自己的 AWS 克隆版本。此外，还有 Rackspace 和 Savvis 等二流 AWS 山寨产品，根据我的经验(有限但非零),它们的商业模式主要包括与企业决策者拉关系，以虚高的价格购买劣质技术。

AWS 没什么问题。亚马逊试图开发一个名为 Elastic Beanstalk 的平台，这个平台有一个问题，当我最后一次尝试使用它时，导致我在差点用手挖出自己的眼睛之前，把手扔向空中。但亚马逊的弹性计算云总体来说非常棒:非常便宜，非常强大，已经证明可以扩展到企业级，并提供了大量真正有用和有效的工具。事实上，Heroku 和 Parse 都是基于 AWS 构建的。

问题是在使用了 GAE 和 Heroku——或者(我认为)任何其他平台服务——之后，配置服务器感觉如此痛苦和不必要的缓慢、复杂。唉，有时它仍然是正确的选择。或者至少还没有不可否认的更好的出现。

因此，我们仍然受困于我之前列出的所有选择，而且越来越多，似乎每年都有更多，无论你做出什么决定，你都会有一种挥之不去的感觉，觉得自己本可以做得更好。(除非你在 Drupal 上选择了 PHP，在这种情况下，它更像是一个唠叨的必然结果。)我想这就是生活，我认为这种骚动是必要的，也是有益的:

> “你知道那个家伙说了什么——在意大利，博尔吉亚家族统治的三十年里，他们经历了战争、恐怖、谋杀和流血，但他们创造了米开朗基罗、达芬奇和文艺复兴。在瑞士，他们有兄弟般的爱，他们有 500 年的民主与和平——那产生了什么？布谷鸟钟。”

([引用](https://web.archive.org/web/20230328231541/http://en.wikipedia.org/wiki/The_Third_Man)

这是软件复兴。这很好。但对普通工匠来说，这仍然很难。

*图片来源*:在墨西哥城的索卡洛建造世界上最大的圣诞树。