# 深入了解微软最新数据可视化工具 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/12/04/meet-pivot-microsofts-newest-data-visualization-tool/>

# 深入了解微软最新的数据可视化工具 Pivot

![](img/d0489974b44c51dbf5d65c08458070d2.png)

几周前，在微软的 [PDC](https://web.archive.org/web/20221209122810/http://microsoftpdc.com/) 活动上，微软 [Live Labs](https://web.archive.org/web/20221209122810/http://livelabs.com/) 推出了一项名为 [Pivot、](https://web.archive.org/web/20221209122810/http://getpivot.com/)的新技术，以理解网络上对象之间的相互联系。Pivot 的基本前提是查看 web 上个人信息“集合”之间的关系。网络上项目之间的许多联系不一定是有形的，但 Pivot 有助于抓取网络上的大量对象，并产生所有联系的圆滑可视化。我们与微软技术人员 [Gary Flake、【Pivot 的创建者以及微软传道者 Brandon Watson 一起深入探讨了这个应用程序。虽然 Pivot 目前处于私人测试阶段，但我们收到了 500 份 TechCrunch 读者的邀请，他们在这里下载应用程序](https://web.archive.org/web/20221209122810/http://www.microsoft.com/presspass/exec/techfellow/Flake/default.mspx)[时使用的代码是“16FC 2946 0C4C 4CCB”。](https://web.archive.org/web/20221209122810/http://getpivot.com/download/)

Pivot 本身是一个独立的应用程序，但它严重依赖于 Internet Explorer 的渲染引擎。理解 Pivot 重要性的最佳方式是通过一个真实世界的例子来了解这项技术是如何工作的。比方说，我想要一个所有维基百科到 TechCrunch 的链接的可视化， Pivot 将基本上抓取所有维基百科，并创建一个连接到 TechCrunch 的维基百科页面的地图，例如[迈克尔·阿灵顿的维基百科页面。](https://web.archive.org/web/20221209122810/http://en.wikipedia.org/wiki/Michael_Arrington)

Pivot 的另一个实际应用是从脸书提取数据。例如，你可以使用 Pivot[抓取脸书](https://web.archive.org/web/20221209122810/http://www.anythingtheycando.com/blog/)并通过各种数据点如关系状态或大学来划分朋友。微软有一个有趣的例子，Pivot 被用来对体育画报封面进行分类，你可以根据体育类型、球队、运动员等将封面分成垂直类别。

在后端，Pivot 是一个构建在。NET 框架，由 Seadragon 提供支持，Seadragon 还集成了 Silverlight 的部分功能，Silverlight 是微软的 Flash 版本。Seadragon 为 Pivot 的高级缩放和可移动界面做出了贡献。该应用程序还包括一个 Excel 插件，允许您将数据导入到 Pivot 中。

当打开时，Pivot 还可以理解您自己的浏览历史(如果您使用的是 Internet Explorer)。Pivot 在应用程序中托管 IE 的一部分，并将获得一段时间内您的浏览历史，然后基于各种垂直领域对您的历史进行切片和切片。你甚至可以[将](https://web.archive.org/web/20221209122810/http://www.manyniches.com/developers/crunchbase-data-mashed-into-microsoft-pivot-2/) Pivot 与我们自己的数据库 CrunchBase 集成，这样用户就可以直观地分解网站中的所有数据。

Pivot 绝对是一个很酷的玩具，它的可伸缩性和结果令人印象深刻。它不仅允许从网络上进行深度数据挖掘，而且其可视化效果非常流畅，Seadragon 的富媒体功能使该应用程序易于导航。

Pivot 并不是微软实时实验室中第一项引人注目的技术。 [Photosynth，](https://web.archive.org/web/20221209122810/http://photosynth.net/)Live Labs 的毕业生，是一个[令人印象深刻的](https://web.archive.org/web/20221209122810/http://www.beta.techcrunch.com/2009/04/22/macs-now-play-nice-with-photosynths-nifty-3d-photo-albums/)照片查看项目，它将图像拼接在一起，创建伪 3D 世界。

下面是一个开发人员如何使用 Pivot 从脸书挖掘数据的精彩截屏: