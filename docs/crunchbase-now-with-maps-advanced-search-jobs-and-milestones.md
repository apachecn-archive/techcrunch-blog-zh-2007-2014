# CrunchBase:现在有了地图、高级搜索、工作和里程碑

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/06/22/crunchbase-now-with-maps-advanced-search-jobs-and-milestones/>

[![](img/183e3ececc57ceaf2e02123e9ad27487.png "cb-logo")](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/)

我们今天很自豪地宣布对我们的科技创业生态系统信息目录 [CrunchBase](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/) 的一系列新改进。

**贴图**

公司和金融机构的总部现在已经进行了地理编码，并且可以在使用谷歌地图 API 的交互式地图上定位。

假设你正在查看 Yelp，想知道这家公司在哪里，附近还有哪些初创公司。你可以点击 Yelp 地址旁边的[【地图】](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/at/companies/yelp/110)链接，它的总部就会出现在它的 50 个最近的邻居中，包括几个街区之外的[Kongregate](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/at/companies/kongregate/445)the building over 和 [Slide](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/at/companies/slide/137) 。

此外，你现在可以通过[城市](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/city/Seattle)、[州](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/state/MA/)、[邮政编码](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/zip/94043/)或[国家](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/country/AUS)进行浏览。或者选择一个任意的位置，并绘制某个范围内的所有结果(例如，悉尼[10 英里内的所有初创公司](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/search?range=10&geo=Sydney%2C+Australia)，曼哈顿[的 165 家公司](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/search?range=1.0&geo=Manhattan)，或者沙丘路的[风投)。](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/search?range=1.0&geo=Sand+Hill+Road%2C+Menlo+Park%2C+CA)

[![](img/b3d6118dff1275f0574b31167fdba2b0.png)](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/maps/at/financial-organizations/mayfield-fund/4329)

我们现在也在跟踪一些大型机构的多个办公室(见[红杉资本](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/financial-organization/sequoia-capital))。

**高级搜索**

我们新的高级搜索功能真正利用了 CrunchBase 的结构化维基格式。除了简单的关键字搜索，用户现在还可以通过指定他们希望结果符合的特殊标准来搜索[公司](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/search/advanced/companies)、[金融组织](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/search/advanced/financial-organizations)和[人员](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/search/advanced/people)。举例来说，现在你可以搜索所有 2004 年后成立、融资至少 5000 万美元的公司，这些公司都出现在 TechCrunch 上。

[![](img/e34af2b6ecd43ed20e2897e954c8d3f2.png)](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/search/advanced/companies)

结构化数据的伟大之处在于它非常容易聚合。我们有 CrunchBase 中所有[融资轮](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/funding-rounds)和[收购](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/acquisitions)的清单，每一轮都可以以不同的方式排序。

借助高级搜索，您可以深入查看特定结果，即使地理位置起了作用。例如，您可以查询自 2004 年以来在伦敦 5 英里范围内被收购的所有公司。或者所有 30 岁以下的人，他们都是被成功收购的公司的一部分。我们将继续改进我们的搜索能力，所以请在评论中留下任何要求和建议。

**工作岗位**

[![](img/46b7539b3e3db21e04714e9318d4c762.png)](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/company/digg)

我们现在在公司页面上展示 [CrunchBoard](https://web.archive.org/web/20221207212443/http://www.crunchboard.com/) 职位列表。例如，你现在会看到 [Digg](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/company/digg) 正在招聘。有了这些额外的功能，以及我们的 [LinkedIn API 集成](https://web.archive.org/web/20221207212443/http://www.beta.techcrunch.com/2008/05/23/crunchbase-now-integrated-with-linkedin-api/)，我们希望 CrunchBase 将成为求职者越来越重要的研究工具。

**里程碑**

里程碑是我们在 CrunchBase 上最新最具实验性的功能。它的灵感来自我们的写作团队，他们收到许多标题为“服务 X 达到 100 万用户大关”或“公司 Y 雇佣新 CEO”的新闻稿。

虽然这些新闻项目并不总是出现在 TechCrunch 的头版，但我们希望在 CrunchBase 中有一个突出显示它们的地方，所以我们创建了一个名为 Milestones 的轻量级数据类型。这非常简单:每个里程碑都有日期、描述和来源(如果可以在网上找到的话)。

我们希望为每个公司和产品创建一个有用的时间表。以下是 Twitter 最近的一些里程碑事件:

[![](img/4d0faed3cadaaaaac025b904012889e1.png)](https://web.archive.org/web/20221207212443/http://www.crunchbase.com/company/twitter)

和以前一样，CrunchBase 的宗旨是社区参与。我们不仅自己向系统中添加数据，还鼓励其他人也做出贡献。注意到任何丢失或不正确的数据吗？只需点击任何个人资料页面右上角的“编辑此页面”按钮，并提交您所需的更改。还可以从主页添加公司、金融机构和人员。

期待看到更多的社区功能尽快工作，让贡献者在网站上更大的存在。