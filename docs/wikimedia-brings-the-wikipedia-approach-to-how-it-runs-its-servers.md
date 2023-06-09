# Wikimedia 将维基百科的方法引入其服务器的运行方式 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/04/16/wikimedia-brings-the-wikipedia-approach-to-how-it-runs-its-servers/>

# 维基媒体将维基百科的方法引入其服务器的运营

维基百科及其所有相关项目显然是由成千上万志愿者的工作推动的。有趣的是，虽然维基百科运行在开源堆栈之上，但传统上志愿者很难帮助该组织运行其网站。目前，大部分工作都是由受薪员工完成的。然而，在大约一年半的时间里，[维基媒体基金会](https://web.archive.org/web/20230201185418/http://www.wikimedia.org/)——维基百科及其姐妹项目背后的组织——一直在悄悄地[为](https://web.archive.org/web/20230201185418/http://blog.wikimedia.org/2012/04/16/introduction-to-wikimedia-labs/)[维基媒体实验室](https://web.archive.org/web/20230201185418/https://labsconsole.wikimedia.org/wiki/Main_Page)工作，这是一个基于 [OpenStack](https://web.archive.org/web/20230201185418/http://openstack.org/) 的新项目，将允许志愿者帮助维基媒体团队开发、测试和部署对该组织后端基础设施的更改。维基媒体实验室于 2011 年 10 月推出封闭测试版，目前仍处于封闭测试阶段。

需要澄清的是，维基媒体实验室与其说是开发维基百科软件，不如说是运行和改善基础设施，以保持维基百科这样的大型项目顺利运行。目前志愿者社区正在进行的一些项目包括托管大量自动编辑维基百科的[机器人](https://web.archive.org/web/20230201185418/https://labsconsole.wikimedia.org/wiki/Nova_Resource:Bots)的基础设施，以及与 OpenStreetMap 的合作项目，以改善该组织的基础设施，并为维基媒体的项目添加 OpenStreetMap 支持。

正如维基媒体基金会的运营工程师 Ryan Lane 今天所指出的那样，在维基百科的早期，志愿者们通常拥有项目基础设施的根权限。然而，随着维基百科及其姐妹网站的发展，停机变得越来越不可接受，基金会慢慢降低了志愿者访问其基础设施的程度。根据莱恩的说法，维基媒体已经“多年没有新的志愿者了。我们甚至没有一个新的志愿者有 shell 权限。”

这样做的原因是可以理解的。虽然开源软件开发往往规模很大，但毕竟运营并不适合众包。

维基媒体现在正在做的是建立一个基础设施，允许志愿者测试和记录他们的贡献。如果被接受，这项工作就可以部署到生产中。Lane 写道，这使运营团队能够重新获得在组织早期拥有的一些灵活性，而不会有停机和其他问题的风险。