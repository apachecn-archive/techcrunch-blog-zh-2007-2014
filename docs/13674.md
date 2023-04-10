# iOS 应用程序的脸书现在快了两倍:更快的启动、照片、提要和内置 Messenger | TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/08/23/facebook-for-ios-faster/>

不再是“慢”了。今天，脸书发布了其 iOS 应用程序的 [v5，速度快了两倍，因为它是基于 Objective-C 而不是 HTML5。导航基本相同，但应用程序启动，照片加载，新应用程序中显示新故事的速度是一天中推出到应用程序商店的两倍](https://web.archive.org/web/20230314074141/http://itunes.apple.com/us/app/facebook/id284882215?mt=8)[，如果你还没有看到的话](https://web.archive.org/web/20230314074141/http://itunes.apple.com/us/app/facebook/id284882215?mt=8)。

内容在视图之间缓存，Messenger 独立应用程序的所有功能现在都内置了，一个下拉“新故事”横幅实时提醒您新的新闻内容，一个用于 [iPad 应用程序](https://web.archive.org/web/20230314074141/http://itunes.apple.com/us/app/facebook/id284882215?mt=8)更新的脸书允许用户查看时间线。

脸书的 iOS 移动产品经理 Mick Johnson 告诉我，“我们自己也非常强烈地感受到了(关于速度慢的)痛点……所以这次针对 iOS 版脸书应用的重大更新专注于一件事——速度。”

约翰逊向我解释了为什么这个应用程序直到现在都感觉很慢。“为了达到规模，我们特意进行了权衡。我们使用 [HTML5 来测试和尝试](https://web.archive.org/web/20230314074141/https://www.facebook.com/notes/facebook-engineering/under-the-hood-rebuilding-facebook-for-ios/10151036091753920)，人们喜欢在浏览器中使用它，但他们对原生 IOS 应用有不同的期望。因此，在这个版本中，我们在过去的 9 个月里从头开始重建了应用程序，主要的改进是性能。现在，Objective-C 中内置的代码比 HTML5 多得多。”

#### 在脸书新的本土速度赛车手的引擎盖下

**发布**——正如脸书在宣布发布的[博客文章](https://web.archive.org/web/20230314074141/http://newsroom.fb.com/News/A-Faster-Facebook-for-iOS-1b4.aspx)中所写的，“现在应用程序打开速度快多了，当你打开脸书时，你的新闻提要和通知就能加载。”以前，新闻提要可能需要 10 秒钟才能真正显示出来。现在我只需要大约四秒钟就能搞定。这种反馈非常灵敏，手指轻轻一点[就能以高帧率](https://web.archive.org/web/20230314074141/https://www.facebook.com/notes/facebook-engineering/under-the-hood-rebuilding-facebook-for-ios/10151036091753920)立即移动，导航侧边栏也更加清晰地滑出。

**加载**——不幸的是，脸书没有预加载通知后的屏幕，所以当你进入一个新的事件或状态更新时，仍然会有一点滞后。但是消息、事件、群组和其他类别肯定会打开得更快。

**新闻提要**——一旦你进入提要，向下滚动可以更快地载入新闻。如果你在订阅中间，朋友发布了新的更新，你会在屏幕顶部看到一个下拉横幅，注明“新故事 10+”。你可以点击它跳到顶部，自己滚动到那里，或者继续浏览，而不用重新加载提要，你会丢失你的位置。当你查看单个帖子时，一个类似的“新评论”栏会实时显示出来。

![](img/dd299f1a73f1e4f6a049a4cc4192db6f.png "Facbook Messenger in iOS App Features") **照片**——照片加载速度也更快，现在出现在[脸书相机](https://web.archive.org/web/20230314074141/https://techcrunch.com/2012/05/24/facebook-camera/)独立应用的设计中，使用覆盖反馈按钮，但这里还没有滤镜或批量上传。为了有助于单手使用，您可以下拉以快速关闭照片，并返回到上一个屏幕，而不必触及后退按钮。

**Messenger**——脸书 [Messenger 应用](https://web.archive.org/web/20230314074141/https://techcrunch.com/2012/05/04/facebook-messenger-read-receipts/)的所有功能和界面现已整合到 iOS 版脸书应用中，以保持一致性，包括向朋友发送照片和您的位置信息。为了方便开发者，这两个应用程序现在共享一个代码库。

如果你用的是谷歌操作系统手机，不用担心。约翰逊指出，很快“你可以期待 Android 上类似的有趣发展。”

#### 浏览广告也更快

Johnson 强调“HTML5 对我们来说仍然非常重要。我们(在 m.facebook.com)获得的移动流量是 iOS 和 Android 总和的两倍。”尽管如此，HTML5 在 iOS 应用中出现的减少将减少脸书悄悄测试新功能的灵活性。这可能会使它更容易发生意外降低参与度或乐趣的发货变化。它也不能写一套代码，并把它推给所有的应用程序。

不过，总的来说，这一更新应该会让数亿 iOS 脸书用户高兴很多。速度更快的应用程序会吸引他们的注意力更长时间，因为这是你最有可能反弹的痛苦加载时间。这意味着约 1.3 亿脸书 iOS 用户更有可能浏览更长时间，看到更多广告——随着用户群转向移动，这对脸书的盈利至关重要。

但是真正的胜利在于用户体验。iOS 版脸书的响应速度如此之快，以至于你感觉与界面有了物理接触。离和朋友面对面更近了一步。