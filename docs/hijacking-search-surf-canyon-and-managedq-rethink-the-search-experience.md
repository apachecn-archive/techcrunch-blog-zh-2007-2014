# 劫持搜索:冲浪峡谷和管理 q 重新思考搜索体验 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/02/19/hijacking-search-surf-canyon-and-managedq-rethink-the-search-experience/>

创造一个新的搜索引擎似乎是徒劳的。如果雅虎和微软都无法在搜索方面与谷歌抗衡，那么创业公司还有什么机会？因此，我们没有创造新的搜索引擎，而是开始看到位于现有搜索引擎之上的搜索应用程序的崛起。

最近的两个例子是 [Surf Canyon、](https://web.archive.org/web/20221210003037/http://www.surfcanyon.com/)今天公开推出其浏览器插件，以及 [ManagedQ](https://web.archive.org/web/20221210003037/http://beta1.managedq.com/) 几周前悄悄推出自己的网站。我已经玩了两个星期了。它们都对我们都熟悉的精简搜索界面进行了改进，并指出了搜索可以做得更好的地方。对于两个没有任何风险投资的创业公司来说还不错(Surf Canyon 已经筹集了 25 万美元的天使资金，ManagedQ 是从创始人在帕洛阿尔托的地下室跑出来的)。尽管两者都指向正确的方向，但没有一个能提供比谷歌更好的整体搜索体验。

[![surf-canyon-logho.png](img/4083bac80f52bb31eef21336c1b831f9.png)](https://web.archive.org/web/20221210003037/http://www.surfcanyon.com/)**Surf Canyon**是一款位于常规搜索结果之上的应用。这家初创公司有自己的网站，你可以在那里进行搜索，但浏览器插件使它更实用。该插件适用于 Firefox 或 Internet Explorer，基本上允许你对谷歌、雅虎或 Windows Live Search 的搜索结果进行重新排序。(谷歌[不喜欢其他网站对其搜索排名进行重新排序](https://web.archive.org/web/20221210003037/http://www.beta.techcrunch.com/2008/02/08/a-radical-option-for-yahoo-out-open-google/)，但 Surf Canyon 并不依赖于谷歌的 API 来做它所做的事情，因而感觉不受谷歌限制的约束)。

[![surf-canyon-4.png](img/d532e8512467469986d7a1594d2cf4fb.png)](https://web.archive.org/web/20221210003037/https://beta.techcrunch.com/wp-content/uploads/2008/02/surf-canyon-4.png "surf-canyon-4.png") 每当你进行搜索时，每个结果的右边都会出现一个小靶心图标。如果你点击靶心，冲浪峡谷会插入三个推荐的搜索结果，它们与你点击的结果相似。它们在您试图深入查看的结果下缩进显示。例如，如果您搜索“techcrunch”，三个推荐的结果可能是指向 TechCrunch UK、Crunchgear 和 TechCrunch Tech President primarys 的链接(即使是同一搜索，推荐的结果也会随着时间的推移而变化)。您可以在推荐的结果中再钻取两次，以继续细化您的搜索。因此，如果你再次点击其中一个推荐链接旁边的靶心，你可能会在常规谷歌搜索结果的第 8 页看到亚马逊 Kindle 商店上的 TechCrunch 链接，在第 12 页看到《纽约时报》Bits 博客上的提及，或者在第 5 页看到 TechCrunch 脸书小组的链接。

结果是无中生有。冲浪峡谷基本上每次点击有三次机会提出相关的推荐。总的来说，这比你点击谷歌在每个搜索结果中提供的“相似页面”链接更接近，但感觉还是很随意。显示三个以上的推荐结果会有所帮助。但是我最喜欢冲浪峡谷的是界面。它不会带你到另一个网页。推荐的结果会显示在相应链接的下方。它感觉更像一个应用程序，而不是一个繁琐的网站，你必须点击多个页面才能找到你想要的东西。Google 可以从 Surf Canyon 的界面设计中学到 Ajax 的优点。

[![managedq-logo.png](img/c500ab73a24b7fcffb8dd835dd1276b9.png) ](https://web.archive.org/web/20221210003037/http://beta1.managedq.com/) **ManagedQ** 采取更激进的方法。它重新考虑了整个用户界面，使其更加可视化。创始人 David Stat 解释道:

> 搜索十年来都没变过。结果质量提高了，但您所看到的并没有改变。搜索界面在命令层面一直停滞不前，那么为什么没有一个搜索应用程序，而不是创建一个搜索引擎，我们可以坐在任何搜索引擎的结果之上。目前我们使用谷歌。

[![managedq-4-small.png](img/ca8fc44a29f611aaef229c5b2af13083.png)](https://web.archive.org/web/20221210003037/https://beta.techcrunch.com/wp-content/uploads/2008/02/managedq-4.png "managedq-4.png")

[![managed-q-sidebar.png](img/df8e4cada760145cb6311b3462ba8022.png)](https://web.archive.org/web/20221210003037/https://beta.techcrunch.com/wp-content/uploads/2008/02/managed-q-sidebar.png "managed-q-sidebar.png") 每当你在 ManagedQ 上搜索时，前六个结果的右边会出现一个网格，这样你就可以直观地看到通常是蓝色链接的另一边是什么。如果你点击其中一个图片，它会打开一个更大的可浏览窗口，仍然在 ManagedQ 中。这个想法是你可以在不离开搜索应用的情况下在网上冲浪。

可视化呈现搜索结果并不是什么新鲜事。像 ViewFour 这样的网站已经做了很多年了。但是 ManagedQ 结合了视觉搜索和引导式搜索体验。

左边是人员、地点和事物的列表，帮助您优化搜索。ManagedQ 使用自然语言处理(NLP)从整个搜索框中提取主要概念。它使用点对点技术，以分布式方式快速完成这项工作。NLP 系统的一个缺点是，它们需要花费大量时间来解析和分块大型数据集。ManagedQ 解决了这个问题。

当你点击左边的一个名字或概念时，无论它出现在右边的微型网页的什么地方，它都会被高亮显示。因此 ManagedQ 为您提供了一种引导式的搜索体验，其中的建议术语可以帮助您缩小搜索范围。如果你搜索“巴拉克·奥巴马”，它会提示相关的人，如“约翰·爱德华兹”、“希拉里·克林顿”和“约翰·麦凯恩”，以及其他相关的搜索词:“哈佛大学”、“主题演讲”、“投票记录”、“早期生活”和“参议员生涯”。"

ManagedQ 的主要缺点是，如果你想看到第一个结果网格以外的内容，你必须点击底部的“下一步”按钮。当您尝试使用左侧的一个引导词来细化搜索时，您不会显示包含该词的搜索结果，而是停留在现有的半填充灰色框的网格中，这些框上写着“没有匹配”。您必须单击搜索结果集来查找匹配的网页，在这种情况下，搜索项会高亮显示。(关于 ManagedQ 的更多信息，请观看[教程](https://web.archive.org/web/20221210003037/http://beta1.managedq.com/tutorial/p1.html))。

仅仅这个缺陷就使得 ManagedQ 在这一点上仅仅是一个有趣的实验。搜索谷歌仍然要快得多，而且能更直接地得到你想要的结果。但是，谷歌可以在这里学到一些东西。为什么不在搜索结果旁边给每个网站提供一个合适大小的图片，给搜索者一个视觉提示，让他们知道链接的另一边有什么？正是这些额外的小信息，在某些情况下，但不是所有情况下，可以帮助人们更容易地整理搜索结果。