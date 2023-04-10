# Twitter 照片托管的迹象 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/05/31/signs-of-twimg-twitters-photo-hosting-in-the-wild/>

# Twitter 照片托管在野外的迹象

![](img/056ce8f712689e7d59f6ddb7a197f6cf.png)

自从我们最初在 Twitter 的照片分享服务上报道了之后，更多的细节浮出水面，即苹果新的 [iOS 5](https://web.archive.org/web/20221225124822/https://techcrunch.com/2011/05/31/twitter-pictures-ios5/) 可能会带有一个内置的 Twitter 图片分享功能。

一位消息人士告诉我们，一个快乐的苹果 iOS 设计者已经发布了一个测试链接(我们已经看到了，但没有在这里复制)。线人给我们提供了一个 http://a0.twimg.com/status_photos/的网址，这个网址出现在他的时间线上，然后很快就消失了。

虽然 Twitter 在 http://a1.twimg.com/profile_images/上发布个人资料图片已经有一段时间了，但/status _ photos/appendix 是新的，或者说相对来说是新的。

稍微谷歌一下[就会发现另外三个迹象:一个](https://web.archive.org/web/20221225124822/http://www.google.com/#sclient=psy&hl=en&site=&source=hp&q=http:%2F%2Fa0.twimg.com%2Fstatus_photos%2F&aq=f&aqi=&aql=&oq=&pbx=1&bav=on.2,or.r_gc.r_pw.&fp=32e85c385197ec57&biw=1602&bih=853)[测试账户](https://web.archive.org/web/20221225124822/https://twitter.com/#!/test033011)在 3 月 30 日发布了照片，一个受保护的 Twitter office 账户的谷歌缓存在 3 月 31 日发布了[上面的照片](https://web.archive.org/web/20221225124822/http://a1.twimg.com/status_photos/236640447)，这个奇怪的账户[昨天发布了照片](https://web.archive.org/web/20221225124822/http://twitter.com/#!/gilbertsoLANO/statuses/75301545121562624)以及 Twitter 设计师 Coleen Baik 从她的账户发布了[这张照片](https://web.archive.org/web/20221225124822/http://tweetmeme.com/story/4935238589/)的 Tweetmeme 缓存，但原始推文已经找不到了。

如果我们听到的是正确的，该服务只是一个简单的 S3 上传程序，那么上面的/status_photos/链接似乎是有意义的。然而，我们期待这些最终会被重新格式化为更干净的东西，比如 Twimg.com/3dkd。

更新:看起来网络图片是托管在 Photobucket(而不是 S3)上，并且网络的 URL 至少是 pics.twitter.com。我们必须等到周一才能看到 iOS mobile 上的图像。

*图像:[办公室](https://web.archive.org/web/20221225124822/https://twitter.com/#!/TheTwoffice)*