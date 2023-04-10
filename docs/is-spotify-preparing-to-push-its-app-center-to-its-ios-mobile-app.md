# Spotify 是否准备将其应用中心推至其 iOS 移动应用？

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/09/09/is-spotify-preparing-to-push-its-app-center-to-its-ios-mobile-app/>

昨天，Josh 写了 Spotify 如何计划推出其音乐流媒体服务的基于浏览器的版本。今天早些时候 [AllThingsD](https://web.archive.org/web/20221205113948/http://allthingsd.com/20120909/yes-spotify-is-headed-to-the-web-no-spotify-isnt-cutting-its-prices/) 进一步证实了这一点，并增加了一点色彩:价格不太可能同时降低；它将在大约一个月后开始推出。我们从一个消息来源听到了一个类似的十月份的报告。现在，除此之外，我们还看到了一些证据，表明 Spotify 也可能计划通过将第三方应用服务加入其中来增强其移动应用。

目前，Spotify 的桌面应用程序提供了一个[的特定部分，在那里他们展示了使用该公司 API 的第三方应用程序](https://web.archive.org/web/20221205113948/http://www.spotify.com/us/about/apps/)——例如，一个 TuneWiki 应用程序给你 Spotify 曲目的歌词；LastFM 提供个性化推荐。但目前在 iOS 应用中没有 Spotify 第三方应用的链接。

将应用中心添加到移动应用中对 Spotify 来说非常有意义，因为它试图使其服务更加无处不在，并继续寻找延长在该平台上花费时间的方法，并使该平台成为音乐流媒体服务的核心。

我们采访的一位开发者指出，Spotify 目前在移动领域拥有许多最活跃的用户(当然也更有利可图，考虑到所有移动用户都注册了 Spotify Premium 虽然在美国，广播服务在 Android 和 iOS 上是免费的)。创建一个应用商店将是发展移动业务的一个途径。

这也意味着与桌面(可能还有网络浏览器)体验更接近的功能和平等。此外，鉴于在苹果和谷歌 Play 等应用商店发现应用程序是一场噩梦，在 Spotify 应用程序中突出显示这些应用程序将为这些第三方应用程序提供另一条发现途径。这也可能鼓励更多公司为 Spotify 平台开发应用。目前，Spotify 在其网络应用上列出了 47 个应用。

此前有报道称，苹果公司正在研究更多的流媒体服务，这可能会打击潘多拉等竞争对手。

开发人员 tico-man(链接到他的网站[这里](https://web.archive.org/web/20221205113948/http://ethansites.com/))首先引起了我们的注意，他发现 Spotify 的一些现有代码中嵌入了一组文件(他要求我们在报告此事时不要公开此方法；所以我们是)。他的观点是:这是一个“极好的 HTML 5 捆绑证据，表明 Spotify 准备要求他们的开发者为 iPhone 创建应用内应用。”

数据没有具体提供实际实现的细节，“但代码中的早期文档是非常令人信服的材料，表明第三方将为他们的移动应用程序编写应用程序，”他指出。

我们已经看到了自己的代码，它包括。json 文档指定了诸如 UserInstallable、Dependencies、SupportedDeviceClasses、AppName、AppDescription、ApiPermissions 之类的细节——所有这些细节都可以被希望将其应用集成到平台上的开发人员所使用。

它似乎还提供了描述某些功能的其他指针:“应用程序对象管理您的应用程序和它在其中运行的 Spotify 客户端之间的交互，”例如，这是对应用程序类的描述。

这些文件似乎还包含现有 Spotify 应用程序的一个更新、未发布版本的代码——进一步指出了一些可能即将到来的事情。这个新版本被称为 1.0.0(相对于[当前版本 0.8.3](https://web.archive.org/web/20221205113948/https://developer.spotify.com/blog/2012/07/31/versioning-the-spotify-apps-api/) )。

很可能，如果这是它看起来的样子，虽然 Spotify 的移动应用中心可能不提供应用程序本身的下载——这将违反苹果自己关于“Inception”的规则，就像 iOS 应用程序中的应用程序商店一样——Spotify 可以提供这样的功能来帮助用户发现应用程序。这将通过苹果的应用商店提供这些应用的链接。这类似于脸书通过其 iOS 原生应用和网络应用提供第三方应用的做法，或者 Openfeint 在其 iOS 应用中的做法(当它迁移到 Gree 时，可能会继续这样做)。

**更新** : Spotify 回应了我们的评论请求。“非常感谢您让我们注意到这一点，但是根据前一天的文章，我们不会对这些故事发表任何评论。”

罗曼·迪莱特补充报道。