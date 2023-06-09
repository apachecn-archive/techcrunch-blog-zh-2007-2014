# 迭代:iOS 应用分发的残酷现实 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/10/21/iterations-the-harsh-realities-of-ios-app-distribution/>

**编者按:** *[塞米·沙阿](https://web.archive.org/web/20221207014826/http://blog.semilshah.com/)是一位拥有 Javelin Venture Partners 的 EIR，自 2011 年 1 月以来一直是* TechCrunch *的官方撰稿人。你可以在推特上关注他，地址是[@ semi](https://web.archive.org/web/20221207014826/http://www.twitter.com/semil)。*

在这篇文章中，我将尝试阐明许多应用程序开发人员面临的一个战术问题，但不幸的是，我必须提前声明，如果不进行根本的改变，我不知道是否存在任何解决方案。本周专栏的主题是剥离苹果 iOS 中的移动应用分发层，并通过这样做，希望照亮开发者在当前存在的危险条件下可以利用的领域。

正如许多这类帖子的情况一样，我会给出一些免责声明。首先，我专注于 iOS 应用生态系统，因为这是我主要接触的内容。是的，我在过去尝试过安卓产品，我确实认识到它的开放系统允许开发者更快地开发东西，而且比苹果的系统限制更少。第二，在这篇文章中，我将要求读者把游戏、通讯工具、大品牌扩展(我肯定 Target 有很大的用户群)、原生苹果应用(比如 iMovie)，尤其是那些预装的应用，以及基本的工具应用，比如 Fandango(电影票)等等——这些应用拥有最多的下载量和最激烈的竞争。不言而喻，这些类型的应用程序是最常被下载的，所以暂且抛开这些，我们这些不是 Instagram 的人如何获得真正的 iOS [分发](https://web.archive.org/web/20221207014826/http://blog.semilshah.com/2012/07/10/distribution-is-a-hell-of-a-drug/)？

简短的回答是:恐怕，至少现在，对许多人来说，这是一个无法实现的目标。

得出这个结论花了一些时间。在过去的几个月里，我接触并测试了许多令人兴奋的移动概念，在少数情况下，当我看到一款产品并想象它在我的手机上运行的漫长未来时，我被一个反复出现的问题绊倒了:“太好了，但这款应用程序如何能在数百万部手机上留下印记，而不仅仅是几十万部？如果它真的爆发了，有什么计划让这款应用每天提供价值，或者接近每天的价值？”最令人沮丧的是，在这几个案例中，我可以很容易地想象出一个未来，几乎每个 iOS 客户都会使用这些应用程序，它们将提供巨大的价值，但想到第一个障碍——分发——可能是最高的，这既令人难过又令人害怕。

如今，人们很容易被“手机”迷住。所有的传感器。速度，时尚的手机。永远在线的后台功能。此外，愤怒的小鸟、优步、Voxer 和 Instagram 等应用和服务的成功让 iOS 变得更加诱人。在某种程度上，这些应用程序创造了现代应用程序淘金热，现在创建这些应用程序更容易了，每个人都在这个游戏中，从大品牌到世界各地的学生，他们只想创建他们希望看到存在的东西。从“制造者”的角度来看，这是惊人的；从消费者的角度来看，这可能是压倒性的，正如 *TechCrunch 的*联合编辑 [Alexia Tsotsis](www.twitter.com/alexia) 在 2011 年 11 月的这篇[精彩帖子](https://web.archive.org/web/20221207014826/https://beta.techcrunch.com/2011/11/11/start-making-sense/)中指出的。今天的结果是应用程序和服务的高度分散，甚至一些精明的应用程序开发人员会真正惊讶地发现五个或更多与他们基本相似的应用程序。

这种淘金热的一个结果是“移动优先”的心态。流行的观点似乎是，公司首先为 iOS 开发产品，这当然有道理。这就是 Instagram 所做的，然后他们最终通过为图片创建单独的页面来扩展到网络。然而，最近我遇到了一些创始人，他们原本打算专注于移动领域的新公司，但对于这些与分销相关的具体问题，他们首先从网络开始。在今天的环境中，有一些合理的理由考虑“网络优先”的方法。应用程序开发者可以尝试寻找初始受众的来源，他们可以为自己的品牌建立知名度，他们可以推动注册，衡量留存率、参与度和其他关键指标，并享受更快迭代的能力。我并不是建议每个应用程序都重新调整策略来采用这种方法，但鉴于目前的情况，这是值得考虑的，我见过的少数几家首先使用网络和/或[电子邮件](https://web.archive.org/web/20221207014826/http://blog.semilshah.com/2012/07/23/timehopping-into-nostalgia/)的公司已经或可能会从种子阶段筹集健康的 A 轮融资——我不得不相信，在某种程度上，他们从网络到移动的序列游戏与此有关。

一旦一款 iOS 应用准备就绪，开发者就必须使出浑身解数来确保发布成功。这可以转化为围绕公共关系、新闻稿、邀请和推荐挂钩的各种策略，并迫使每个同事、朋友、投资者和顾问在他们的社交网络上分享新闻和对你的应用发布的评论。一个不幸的副作用是，一些公司已经决定动用他们的资金，花在更传统的营销和公关工作上，只是为了帮助获得最初的提升，这通常投资回报率很低，并且通常不可持续。

如果应用程序提供了一些新的东西，人们会越来越多地使用它(希望如此)，然后开发者可以利用技术给自己提供增长和保留的每一个机会。像 Instagram 一样，他们让分享到社交网络变得容易，因为他们相信好的内容会传播，希望有一天网络效应会发生。此外，有许多技术可以用来提高保留率和参与度。像 [Lift](https://web.archive.org/web/20221207014826/http://lift.do/) 一样，他们可能会使用默认的选择加入电子邮件提醒，这与原生应用程序体验密切相关。像[高亮](https://web.archive.org/web/20221207014826/http://highlig.ht/)一样，他们可能会使用 iOS 通知在后台运行，并根据上下文向您发送警报。而且，像[愤怒的小鸟](https://web.archive.org/web/20221207014826/http://www.angrybirds.com/)一样，他们都祈求好运，希望得到那种即使金钱和名誉也买不到的口碑传播。但是，在我们拥有重要的保留和参与之前，最初的分销障碍需要被清除。

综合来看，情况似乎很糟糕。我们将何去何从？

一种观点认为，这一负担落在手机和操作系统制造商身上，让应用程序的分发、发现和共享变得更加容易，这样用户就可以接触到更好的应用程序集，从理论上讲，随着时间的推移，这不仅有助于安装数量，还可以创造更好的用户保留和参与度。也许脸书可以帮助 T9，因为大多数人的手机都安装了脸书，两家公司对我们使用的应用程序都有很好的了解，可以推荐给朋友。现在，我只从朋友那里听说应用程序，或者如果它以某种方式出现在我的 Twitter 上。我对苹果和他们新设计的应用商店有 101 条建议，所以我不会在这里深入讨论，只是指出开发者确实感受到了这种痛苦 iOS 应用商店的新设计似乎是应用发现的一种倒退。

然而，另一种观点认为，这个负担同样落在了应用程序制造商(和消费者)身上。消费者可能会很难区分除了一些微小差异之外看起来相似的应用程序。许多 iOS 用户有许多“死亡应用程序”屏幕，一旦下载并试用，现在只是在后台腐烂。一个人真正能用的 app 有几个吧？也许我们在技术世界中太习惯于测试一切新的东西，这样我们就可以成为第一批宣布新赢家的人之一，但现实是，日常消费者可能只会关注那些为他们提供特定上下文信息和服务的应用程序，或者一些全新的、新颖的和引人入胜的东西。这可能是一个新的设计(就像大约的[创造了零食大小的新闻)，或者是一个新的商业模式(就像](https://web.archive.org/web/20221207014826/http://cir.ca/) [Lyft](https://web.archive.org/web/20221207014826/http://lyft.me/) 创造了拼车，聚合线下以满足移动需求)，或者是一个习惯形成的互动(就像 [Lift](https://web.archive.org/web/20221207014826/http://lift.do/) 相当成功)，或者是一个围绕熟悉的心理模型的定义良好的日常用例(就像 [Sosh](https://web.archive.org/web/20221207014826/http://sosh.com/) 在下班后外出所做的)。 或者[在社交网络上协调](https://web.archive.org/web/20221207014826/http://blog.semilshah.com/2012/08/10/the-mobile-harmonization-of-social-data/)用户数据以创造新产品(就像[布鲁斯特](https://web.archive.org/web/20221207014826/https://www.brewster.com/)所做的那样，将社交网络与电话联系人列表配对)，或者[将](https://web.archive.org/web/20221207014826/https://beta.techcrunch.com/2012/07/07/bringing-technologies-to-mobile-applications/)真正的技术引入移动设备(就像[棱镜](https://web.archive.org/web/20221207014826/http://blog.semilshah.com/2012/08/23/the-long-road-to-prismatic-for-iphone/)已经能够利用其个性化新闻服务)。 也许这些应用程序已经突破了所有的障碍和噪音，因为它们认识到了 iOS 领域的雷区，并相应地为这场战斗做好了准备。

我在这里没有很多答案。也许苹果可以改变 App Store 的某些方面。也许突破需要的应用和服务的门槛仍然非常高。也许开发者会慢慢远离原生应用，使用 HTML5 或一些变体来回避原生应用发现问题，而是使用移动网络来推动他们的分发。也许消费者对碎片化的应用前景感到满意，或者最好的做法是在 iOS 上最受关注的几个类别中建立全新的产品体验。我很乐意阅读您下面的想法和建议，尽管有一点是明确的——某个地方存在问题，用户仍然被选择淹没，[开发人员对这些限制感到沮丧](https://web.archive.org/web/20221207014826/http://t.co/jZRcO32g),构建下一个东西的竞争只会加速。结果是，考虑到我们周围的环境因素，在这个特定的时刻，“移动优先”策略可能不是特定类别中特定应用的正确方法。相应地规划你的应用的未来。

**图片来源:**[techburst](https://web.archive.org/web/20221207014826/http://www.flickr.com/photos/techburst/2624884458/)/*Flickr 知识共享*