# 脸书发布超级书呆子大数据工程博文吸引铁杆程序员 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/11/08/a-riddle-wrapped-in-a-mystery-inside-an-enigma/>

# 脸书发布超级书呆子大数据工程博文吸引铁杆程序员

100 集群！一天 60，000 次蜂巢查询！脸书最新的[1800 字的工程博客帖子](https://web.archive.org/web/20221207080522/https://www.facebook.com/notes/facebook-engineering/under-the-hood-scheduling-mapreduce-jobs-more-efficiently-with-corona/10151142560538920)只有一个目标:向世界顶级程序员证明，如果他们想要挑战，他们应该为社交网络工作。对于门外汉来说，除了脸书的数据仓库比 2008 年大了 2500 倍之外，没什么别的了。这是后端极客色情，对脸书的长期成功至关重要。

脸书和任何上市的科技创业公司一样，面临着留住人才的问题。如果一只小股票没有可能在某一天价值连城的巨大优势，那么让最好的程序员、设计师、产品愿景者和商业奇才加入或不跳槽是很困难的。

创办一家公司并发号施令是有诱惑力的。加入一个踢屁股的小创业公司是令人兴奋的，因为它击中了它的曲棍球棒。如果脸书不能超越这些，它可能会停滞不前，变得更容易受到破坏。

但是脸书有一个年轻的创业公司没有的东西。或者我应该说十亿件事。它庞大的用户群意味着它所构建的东西会严重影响世界，它正试图解决计算机科学前沿的工程问题。然而，乍一看，它可能只是另一种消费产品。这就是为什么它需要像“引擎盖下:使用 Corona 更有效地调度 MapReduce 作业”这样的博客帖子。

【T2![](img/3599ce3f25c4399a833b8b0809c7ed75.png "corona2.jpg")

该说明详细说明了 Hadoop MapReduce 调度框架的限制，以及脸书如何构建自己的 Corona 版本来超越这些限制。脸书有开源的 Corona，它现在在 GitHub 上。好处包括使用 MapReduce 将插槽重新填充时间从 10 秒降至 600 毫秒，将作业延迟减半，以及更好的集群利用率和调度公平性。我不打算再转述它们了，所以如果那些东西让你感兴趣，[读一下帖子](https://web.archive.org/web/20221207080522/https://www.facebook.com/notes/facebook-engineering/under-the-hood-scheduling-mapreduce-jobs-more-efficiently-with-corona/10151142560538920)。

脸书已经[发布工程博客文章](https://web.archive.org/web/20221207080522/http://www.facebook.com/Engineering?sk=notes)好几年了，但是《引擎盖下》系列大约是在它申请 IPO 的时候开始的。旧的 eng 博客帖子过去更多的是关于建设脸书后端的人类故事，但自从它上市以来，似乎变得更加铁杆。这是明智之举，因为它不再有估值快速上升带来的意外之财来吸引工程师了。

脸书必须证明这是一个谜，包裹在一个谜中的谜，因为这是让伟大的程序员兴奋的原因。