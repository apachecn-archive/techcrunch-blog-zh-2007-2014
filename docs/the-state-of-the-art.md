# Android vs. iOS 开发:拼了！

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/11/16/the-state-of-the-art/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

永恒的启动问题“先安卓还是先 iOS？”变得越来越棘手，有消息称 Android 的市场份额超过 80%。但是不要管那些管理人员和非技术型创始人:*做什么[开发者！开发商！](https://web.archive.org/web/20230325060922/http://www.youtube.com/watch?v=8To-6VIJZRE)* 想起那段鸿沟？谁让他们的生活更轻松，谁就获得了相当大的优势。

我说的“他们”是指“我们”不写 [TC 专栏](https://web.archive.org/web/20230325060922/https://techcrunch.com/author/jon-evans/)(和[小说](https://web.archive.org/web/20230325060922/http://rezendi.com/))的时候，我是 [HappyFunCorp](https://web.archive.org/web/20230325060922/http://www.happyfuncorp.com/) 的一名软件工程师，这是一家有史以来最好的咨询公司(和网站——继续，点击进入)。随着我发现自己做了越来越多的管理工作，为了跟上进度，我最近为一个宠物个人项目编写并开源了一对几乎相同的 Android 和 iOS 应用程序。所以让我用它们来带你了解一下最先进的技术。

背景:我以前写过许多 Android 和 iOS 应用程序，无论是个人的还是专业的。这些应用程序是我的宠物新闻聚合器 [Scanvine](https://web.archive.org/web/20230325060922/http://www.scanvine.com/) 的原生客户端，它识别在社交媒体上被异常广泛分享的故事。他们的完整源代码可以在 Github 上找到:( [Android](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android) | [iOS](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-ios) )，实际应用也可以下载:([Google Play](https://web.archive.org/web/20230325060922/https://play.google.com/store/apps/details?id=com.scanvine.android)|[App Store](https://web.archive.org/web/20230325060922/https://itunes.apple.com/app/scanvine/id717815889?mt=8)。)

在我们开始之前，我必须提到 Xamarin 的跨平台开发工具。如果我精通 C#，特别是如果我还不知道 Java 和 Objective-C，那将是我开发原生应用程序的首选。

此外，免责声明:这是更“有趣的代码”，而不是“产品质量”你会注意到明显缺乏测试代码；我还需要追查一个 iOS 海森堡；我应该使用 git 子模块，而不是为第三方库复制粘贴文件；等等。(***【eta:***)唉，一个流氓布局文件溜进了 Android 版本，导致它在平板电脑上崩溃。现已修复。)

现在，事不宜迟，*让战斗开始吧！*

### 环境

您仍然可以用文本文件和命令行编写代码，很多人都这样做了，但是使用集成开发环境(IDE)会更有效率。

苹果的是 Xcode，总的来说，这是一种乐趣。它光滑、快速、强大、有用而不具侵入性，并且它越来越擅长掩盖其光滑外表下不友好的编译机制，以及苹果强加给开发者的复杂而偏执的证书/档案机制，以保持其对 iOS 应用和设备的铁腕控制。调试器无缝工作，模拟器快速响应。

但是安卓呢？哦，安卓。目前最先进的 IDE 是 [Eclipse，用 Android 插件](https://web.archive.org/web/20230325060922/https://developer.android.com/tools/sdk/eclipse-adt.html)定制的，而且*差得令人尴尬*。缓慢，笨拙，违反直觉，如果不是完全令人困惑，布局不佳，不必要的复杂，它只是一个烂摊子。它的调试器如此笨拙，以至于我发现自己大部分时间都在调试日志文件，而 XCode 调试器是我在 iOS 上寻找 bug 的工具。越少提到 Android 模拟器越好，它需要*分钟*来启动，然后有一半时间无法连接到 Android 调试桥。

现在，公平地说，谷歌知道这是一个问题，他们正在开发一个新的 Android Studio IDE。唉:

> Android Studio 目前提供早期访问预览版。有几个特性要么不完整，要么还没有实现，您可能会遇到错误。如果您不喜欢使用未完成的产品，您可能希望下载(或继续使用)ADT 包(带有 ADT 插件的 Eclipse)。

很高兴看到他们正在努力，但令人惊讶的是，在我购买我的第一部 Android 手机 4.5 年后，这种混乱仍然是最先进的。

*优势:* iOS，遥遥领先。

### 配置

正如我提到的，在 Xcode 和 Objective-C 光滑无缝的外表下，隐藏着 20 世纪 70 年代编程的洛夫克拉夫特式的恐惧。我开玩笑，我开玩笑…但还是。宏和头文件；项目、目标、方案和构建配置；令人震惊的构建设置列表；遇到令人困惑的链接器错误的可怕绝望；以及[发现](https://web.archive.org/web/20230325060922/http://stackoverflow.com/questions/6646052/how-can-i-disable-arc-for-a-single-file-in-a-project)类似“哦，你的第三方代码不支持 ARC？只需添加-fno-objc-arc 标志！简单，不是吗？”

Android 有一个单一的清单文件，Eclipse 会在你每次保存文件时完整地构建你的应用程序。当你的应用因为没有正确配置权限而无法运行时，我希望你得到的错误信息更加清晰，但这只是一个小问题。总的来说，Android 应用程序配置简单而优雅。

*优势:*安卓。

### UX 设计

你可能会认为苹果会带走这个奖杯。它的界面生成器是一种非常简洁的方式，可以快速地将简单好看的用户界面组合在一起。问题是，我实际使用界面构建器越多，我就越不喜欢它。这是另一层配置复杂性；对于简单的事情来说这是极好的，但是随着时间的推移和应用程序的发展，那些简单的事情往往会变得复杂和混乱；我*真的*不喜欢苹果大约一年前增加的多屏故事板。

虽然 Android 理论上有一个类似的可视化工具，但越少谈论它越好。实际上，你最终会编写出 [XML 文件](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/tree/master/res/layout)，这些文件提供了布局指南，而不是规则，这样应用程序(希望)就能很好地呈现在所有设备和屏幕尺寸上。(苹果的[自动布局](https://web.archive.org/web/20230325060922/https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/AutolayoutPG/Introduction/Introduction.html)也是如此，着眼于未来更大种类的 iOS 屏幕，毫无疑问。)与此同时，Android 提供了一个[图标包](https://web.archive.org/web/20230325060922/http://developer.android.com/design/downloads/index.html)供开发者使用，而 iOS 开发者不得不与第三方合作，比如 [Icons8](https://web.archive.org/web/20230325060922/http://icons8.com/) ，或者开发自己的图标包。

总的来说，这是一场比你想象的更激烈的竞争，尽管我承认这是相当特殊的。最后，有两件事给了 iOS 优势。首先，它仍然简单得多:三种屏幕尺寸(包括 iPad)和两种屏幕密度，而不是 Android 的复杂程度。第二，默认的 iOS 视觉元素——比如弹出菜单和消息——比 Android 的视觉元素更有吸引力。

*优势:* iOS。

### 语言

安卓的 app 都是用 Java 写的；Objective-C 中的 iOS 应用也有例外——还有 Xamarin 还有其他各种各样的原生应用边缘案例；还有像 PhoneGap 这样的原生/web 混合应用——但一般来说，原生 Android 应用是用 Java 编写的，原生 iOS 应用是用 Objective-C 编写的。

我开始接触 Java 编程，起初并不喜欢 Objective-C，很大程度上是因为它过于冗长:像这样的一行

*String s2 = s1.replace("abc "，" XYZ ")；*

成为

*ns string * S2 =[S1 stringbyreplacingoccurrences of string:@ " ABC " with string:@ " XYZ "]；*

但是我越来越喜欢 Objective-C，它比 Java 更好，更干净。它有[块](https://web.archive.org/web/20230325060922/http://en.wikipedia.org/wiki/Block_%28programming%29) : Java 没有。它有[个类别](https://web.archive.org/web/20230325060922/https://developer.apple.com/library/ios/documentation/cocoa/conceptual/ProgrammingWithObjectiveC/CustomizingExistingClasses/CustomizingExistingClasses.html)；Java 没有。它不需要您用大量样板 try/catch 异常处理空白来包装大部分代码:Java 需要。

Java 有它的优势。首先，更好的堆栈跟踪，这意味着跟踪零星的错误会容易得多。直到几年前，Android 还拥有垃圾收集的巨大优势。但现在 iOS 有了[自动引用计数](https://web.archive.org/web/20230325060922/https://developer.apple.com/Library/ios/releasenotes/ObjectiveC/RN-TransitioningToARC/Introduction/Introduction.html)，这种优势基本消失了(尽管旧的第三方工具通常不能与 ARC 一起工作，这意味着你必须做一些 XCode 配置巫术来逐个文件地关闭它。)随着这种区别的消失，赢家是显而易见的。

*优势:* iOS。

### 蜜蜂

Android 和 iOS 都为他们的开发者提供了一个巨大的软件库，从广义上讲，这些库非常相似:有针对电话功能和特性的 API，网络访问功能，一整套视图对象，包括功能强大的 WebView，它本质上是一个成熟的浏览器。同时，大部分工作是在控制器中完成的:非常粗略地说，一个 iOS ViewController 相当于一个 Android 活动。

iOS 拥有而 Android 没有的是一套额外的框架和功能——例如，没有真正的 Android 可以与 iOS 强大的核心数据框架相媲美——以及一个总体上更干净、设计更好的系统。比较一下[这些](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-ios/blob/master/SVMasterViewController.m) [两个](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-ios/blob/master/SVStoryTableViewCell.m)相对简单的 iOS 类，例如，它们真正完成了应用程序中的大部分工作，与[这些](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/blob/master/src/com/scanvine/android/ui/StoryListActivity.java) [三个](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/blob/master/src/com/scanvine/android/ui/StoryListFragment.java) [等价的](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/blob/master/src/com/scanvine/android/ui/StoryArrayAdapter.java) Android 类，它们之间包括六个内部或匿名类。在一天结束的时候，我宁愿使用 iOS[collection view controller](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-ios/blob/master/SVMasterViewController.m)而不是 Android [ListAdapter](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/blob/master/src/com/scanvine/android/ui/StoryArrayAdapter.java) 。

另一个度量标准，尽管有缺陷:代码行数。这些应用程序的功能几乎相同，但 iOS one 有 1596 行自定义代码，包括头文件，相比之下，Android 有 2109 行 Java 代码和 XML。整整多了 32%。

*优势:* iOS。

### 互联网

如今，多对多的应用程序更多的是通向互联网 API 的管道，而不是独立的程序；这非常重要，值得单独研究。iOS 和 Android 都为此提供了全套工具和 API。它们都提供非常相似的网络视图，基本上是成熟的浏览器窗口，你可以在任何地方插入你的应用程序。

网络连接基本都要在后台运行，以免阻塞 app 主线程，多线程比较辛苦。Android 为这类事情提供了一个 [AsyncTask](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/blob/master/src/com/scanvine/android/ui/StoryListFragment.java#L166) 类，虽然冗长但运行良好，还提供了一个[非常简单的方法](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/blob/master/src/com/scanvine/android/util/Util.java#L29)来确定你当前是否在线。iOS 提供了等效的设施，但它们都相当低级，不能令人满意。

然而，有许多开源库使生活变得更加容易。我用的是 AFNetworking，和宣传的一样讨人喜欢。当 web 请求完成时，你只需传递给它运行的代码块——这在 Android 中是不可能的，因为 Java 不做块。

*优势:* Android 原生，但 iOS 当第三方库考虑。

### 共享

将应用程序中的内容分享到脸书、Twitter、Evernote 等网站有多容易？我曾认为这将是 Android 的第一轮淘汰赛，Android 长期以来一直有一个强大的应用程序间通信系统，名为 Intents。总的来说，Android 在让应用程序相互调用和共享数据方面做得更好。

然而，在(或许不幸的)更常见的分享案例中，苹果已经迎头赶上。不要相信我的话，你自己判断吧。分享一个 Scanvine 故事的 Android 代码是[这里](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-android/blob/master/src/com/scanvine/android/ui/StoryArrayAdapter.java#L133)，iOS 代码[这里](https://web.archive.org/web/20230325060922/https://github.com/rezendi/scanvine-ios/blob/master/SVStoryTableViewCell.m#L192)。iOS 代码更长的唯一原因是因为我在那里比在 Android 端做了更多的 Google Analytics 跟踪(我应该修复这个问题。)

*优点:*都不是。

### 分裂

没必要在这上面花太多时间。[安卓](https://web.archive.org/web/20230325060922/http://developer.android.com/about/dashboards/index.html)。 [iOS](https://web.archive.org/web/20230325060922/https://techcrunch.com/2013/10/22/200-million-devices-running-ios-7-five-days-after-launch-64-of-all-idevices-20-million-itunes-radio-listeners/) 。QED。虽然值得注意的是，谷歌正在实施一个有趣的碎片整理策略，所以这可能值得很快重新审视。

*优势:* iOS。

### 出版

发布一个 Android 应用就像做梦一样简单。只要通过一个方便的 Eclipse 向导签署你的应用程序，噗，你就有了一个可以在任何设备上运行的 APK 文件。通过电子邮件发送，放在网站上，或上传到 Google Play，并在一小时内(可能)在全球范围内发布。再简单不过了。检查安装统计数据和崩溃报告，包括堆栈跟踪，它(通常)标识出出错的单独代码行，您可以在闲暇时立即上传一个错误修复版本。

发布苹果应用是一场噩梦。我的一个才华横溢的朋友总是建议人们在他们的 iOS 开发计划中至少增加一天的时间*仅仅是*来与证书和发行版档案搏斗。无论我做了多少次，或者最新版本的 XCode 试图让它变得多么简单，它总是*一个巨大的麻烦。如果没有试飞，测试甚至会更糟*。苹果的“iTunes Connect”网站之于谷歌 Play 开发者控制台，就像福特 Pinto 之于特斯拉一样。祝你能得到任何事故报告，更不用说有用的信息了；享受跳过他们任意设置的圈圈的乐趣；惊叹强大的苹果公司的 UX 能有多糟糕。**

 **优势:*安卓，遥遥领先。

### 获胜者是…

iOS，还有一段距离。Android 有其优势，但总体而言，编写好的 iOS 应用程序比编写好的 Android 应用程序要容易得多。再加上 iOS 用户往往更富有——可以说更有影响力——这一事实，对于大多数想引起轰动的初创公司来说，先用 iOS，后用 Android 仍然是有道理的。可以想象，新的 Android Studio IDE 可以缩小这一差距……但不是全部。

(声明一下，我自己的主要手机是一部 Nexus 4，我对它非常满意。)

*图片鸣谢:*詹妮弗·斯托尔泽， [DeviantArt](https://web.archive.org/web/20230325060922/http://jameson9101322.deviantart.com/art/An-Epic-Duel-for-the-Ages-SPG-347196439) 。*