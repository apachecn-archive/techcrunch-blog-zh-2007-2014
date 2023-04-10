# Kindle Fire 代码库让开发者困惑:Android，KF8，还是两者都有？TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/11/01/kindle-fire-code-base-kf8/>

***编者按:**特约撰稿人史蒂夫·罗斯内鲍姆是[放大](https://web.archive.org/web/20221007004312/http://magnify.net/)的 CEO。*

距离亚马逊向首批 50 万名预购用户发售备受期待的 Kindle Fire 还有两周时间，开发者社区的人们发现很难确定什么样的 Android 将在该平台上运行。有一点是肯定的，Mobi 已经过时了——因为亚马逊在新格式中同时采用了 HTML5 和 CSS3。

今天 [Kindle Format 8](https://web.archive.org/web/20221007004312/http://www.amazon.com/gp/feature.html?docId=1000729511&imm_mid=0770d2&cmp=em-orm-toc-newsletter-102611+) 为 Kindle Fire 设备上的图书阅读器提供动力，亚马逊现在告诉开发者，KF8 将在未来几个月内在所有 Kindle 电子墨水设备上可用，重要的是，KF8 也将在免费的 Kindle 阅读应用程序上可用。这意味着 KF8 应该可以在 iPad 上使用——这可能非常有趣。

KF8 是对 Mobi 的重大改进，有 150 种新的格式样式，包括嵌入式字体、首字下沉和 CSS 选择器，如行距、对齐、对齐、边距、颜色、样式和边框。

但是，到今天为止，KF8 格式的构建工具还不可用——我们所知道的重要的 KindleGen2 Publisher 工具和 Kindle Previewer 2 的“即将到来”已经够多了。甚至连 Kindle 出版指南都还没有发布，这让内容所有者有了很大的热情，但几乎没有可操作的信息。

Kindle Fire 将向后兼容，因此所有以 Mobi 格式发布的内容都可以在新设备上运行，这可能是亚马逊不急于将 KF8 工具投入市场的一个原因。Kindle Fire 将推出大量内容，只是如果内容所有者早一点掌握该设备的 HTML5 和 CSS3 规格，它就不会那么时髦。

一旦 Kindle Previewer 2 上市，出版商将能够从 Mobi 移植旧图书，并查看它们如何出现在一系列新的 Kindle 设备和免费阅读器应用程序上。

因此，对于“读者”内容世界来说，有一条通往 KF8 新世界的清晰道路——即使发布指南和工具的时机有些模糊。

但是，对于 Kindle Fire 应用开发者来说，这款设备的路线图并不清晰。

Kindle Fire 是一款基于安卓系统的平板电脑。亚马逊开发者一路走来(传言称要么是冷冻酸奶 2.2，要么是姜饼 2.3.4)分支了 Android，实际上这是一款基于智能手机操作系统的平板电脑，而不是当前的 Android 平板电脑操作系统，冰激凌三明治。

所有开发者都知道设备的规格，以及它不支持什么。

在高水平上，它必须针对 Android 2.3.4(姜饼)和分辨率为 1024 x 600 的 7″屏幕进行优化。您的应用程序不需要谷歌移动服务(GMS)、陀螺仪、摄像头、广域网模块、蓝牙、麦克风、GPS 或 micro-SD 来运行。Adobe AIR 预装在 Kindle Fire 上。亚马逊说，为了增加你的应用程序与 Kindle Fire 兼容的“可能性”，你应该只使用向后兼容姜饼的冰淇淋三明治 API。测试呢？亚马逊建议开发者此时配置一个标准的 Android 模拟器来模拟 Kindle Fire 设备平台。

似乎亚马逊目前的重点是测试整个现有的亚马逊市场 Android marketplace，然后提醒应用程序开发者知道他们的应用程序是否可以在 Kindle Fire 上运行。如果它没有通过 QA，那么开发者有机会进行修复并在 Android Marketplace 上重新发布应用。

鉴于亚马逊的大量内容资源，平板电脑战争似乎将成为 2012 年的一个主要主题。摩根大通已经报告说，2011 年第四季度 Fire 的销量将达到 500 万台。与 iPad 市场相比，这是一个快速的开端，据报道，目前消费者手中有 3200 万台 iPad。

博客 [Cult of Android](https://web.archive.org/web/20221007004312/http://cultofandroid.com/?s=+%27Cult+of+Android%27+exclusive+screenshots) 报道称，一名“消息人士”向其提供了“亚马逊内部库存系统的独家截图”，显示前 5 天预购了 254，074 台 Kindle Fires:“每小时超过 2，000 台，每天超过 5 万台。”这使得 Kindle Fire 有望超过 iPad 和 iPad 2 的首月销量

因此，Kindle 十字军东征势如破竹。销售强劲。KF8 标准将影响当前的电子出版物 3 世界。一旦 Android 的风格变得清晰，一旦开发工具和模拟器进入市场，Kindle Fire 将为应用程序开发人员提供一个新的、大的、潜在有利可图的渠道。

如果 Fire 最终与 Android 平板电脑平起平坐，亚马逊将在赢得新的便携式内容消费者的竞赛中创造强大的优势。