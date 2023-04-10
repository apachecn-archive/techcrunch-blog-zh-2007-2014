# Twitter 向第三方开放照片服务——API 暗示其他媒体

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/15/twitter-photo-api/>

# Twitter 向第三方开放照片服务——API 向其他媒体暗示

自从 Twitter 首次与 Photobucket 合作推出自己的照片分享服务以来，已经过去了两个半月。就在上周，他们完成了[向所有用户推出](https://web.archive.org/web/20230204225415/https://techcrunch.com/2011/08/09/twitter-photo-uploading-now-available-for-100-of-users/)。今天，他们采取了下一步:向第三方开发者开放。

正如[刚刚在 Twitter 开发者博客上宣布的](https://web.archive.org/web/20230204225415/https://dev.twitter.com/blog/photo-upload-api)，有一个新的照片上传 API 已经准备好供公司以外的开发者使用。虽然许多第三方 Twitter 服务已经上传照片有一段时间了，但他们通常使用自己的方法，或者使用更大的播放器，如 TwitPic 或 yFrog。有了新的 API，他们将能够在 Twitter 的服务器上与 Photobucket 一起上传、存储和服务图像。

Notes Twitter:

> 如果您已经使用 OAuth Echo 进行图像上传，您会发现 POST status/update _ with _ media 中提供的新方法更简单，并且需要的依赖性更少。关于这种方法，您首先会注意到的是主机名:媒体状态更新只能在 upload.twitter.com 执行，而不能在 api.twitter.com 执行。使用此替代主机名作为上传路径可确保高可用性和灵活性。

除了“高可用性”好消息之外，您还会注意到“用媒体更新”方面。Twitter 似乎向照片之外的媒体敞开了大门，比如视频。Twitter 表示，目前他们在这方面没有什么可宣布的。同样，毫无疑问，他们只是为未来留下了无限的空间。

为了使用这项服务，Twitter 要求开发者遵循他们的显示指南，这非常简单。值得注意的一点是，他们要求你使用 pic.twitter.com/SLUG 而不是 t.co/SLUG,，似乎是为了让用户知道这是一张点击后出现的图片。

另外，遗憾的是，不支持动画 gif。实际上，感谢上帝。

Twitter 还指出，照片服务也将“很快”整合到 Twitter 移动客户端中。但是“T6”还没有时间表可以分享。我认为它将在今年秋天 iOS 5 推出之前准备好，[依赖于它](https://web.archive.org/web/20230204225415/https://techcrunch.com/2011/06/09/twitter-ios/)。