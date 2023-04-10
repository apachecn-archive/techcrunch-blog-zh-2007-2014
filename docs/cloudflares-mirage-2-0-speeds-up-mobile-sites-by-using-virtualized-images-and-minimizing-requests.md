# CloudFlare 的 Mirage 2.0 通过使用虚拟化映像和最大限度地减少请求来加快移动站点的速度 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/06/13/cloudflares-mirage-2-0-speeds-up-mobile-sites-by-using-virtualized-images-and-minimizing-requests/>

大约一年前， [CloudFlare](https://web.archive.org/web/20221206051331/http://cloudflare.com/) 推出了 [Mirage](https://web.archive.org/web/20221206051331/http://blog.cloudflare.com/introducing-mirage-intelligent-image-loading) ，这是一项为其付费用户提供的服务，旨在通过提供较小的图像并使用“惰性加载”来下载实际出现在浏览器视窗中的图像，从而加快网站加载时间。今天，该公司几乎完全[改造](https://web.archive.org/web/20221206051331/http://blog.cloudflare.com/)这项服务基于它从这个第一个版本中学到的东西。

正如 Cloudflare 的创始人兼首席执行官马修·普林斯(Matthew Prince)告诉我的那样，Mirage 的第一个版本拍摄了一个网站上的每张图片，然后创建了五个不同尺寸的副本，以匹配最常用的屏幕尺寸。这很有效，但是这也意味着新的图像经常与页面布局或屏幕大小不匹配。

为了解决这个问题，CloudFlare 在 Mirage 2.0 中使用了一个非常巧妙的技巧。它不是创建多个副本，而是简单地创建图像的高度退化版本，通常只有原始文件大小的 1%。然而，这个图像包含了浏览器将图像放到页面上并开始呈现页面所需的所有元数据。

一旦页面完成渲染，CloudFlare 的新虚拟化图像加载器就会启动，并开始用全分辨率版本替换这些图像。

普林斯告诉我，这种效果类似于老式的渐进式 JPEGs 图像，如果你在网上呆的时间够长的话，你可能会很熟悉。这两种图像之间的切换是网站所有者在使用 Mirage 时必须做出的权衡。这种技术避免了浏览器在开始渲染页面之前必须等待图像下载，这应该会使用户体验感觉明显更快，但用户可能会在一开始看到这些高度降级的图像时有点惊讶。

下面是一个例子，展示了 Mirage 可以给我们的网站带来多大的改变(不过我们现在并没有使用它):

[维梅奥·http://www.vimeo.com/68270834 w = 640 & h = 360]

当然，所有这些也适用于常规网站，但 CloudFlare 专门针对移动网站。

广受欢迎的图像主机 Imgur 已经在其网站上测试了这一功能，正如该公司创始人兼首席执行官艾伦·沙夫告诉我们的那样，Imgur“看到了 Mirage 2.0 的巨大改进。我们真的很高兴 CloudFlare 继续推出创新产品，以确保 Imgur.com 上的页面尽可能快地加载。”

为了进一步加快加载速度，虚拟化图像加载器还考虑了设备的功能和网络条件。CloudFlare 庞大的网络和用户群允许它对大量数据进行采样，并且现在可以根据请求来自的网络来调整积极的 Mirage 2.0 压缩数据的方式。为了保持最小的数据包丢失，该服务还将所有这些图像合并到一个请求中，而不是为每个图像发起一个新的请求。

Mirage 2.0 现已面向所有付费 CloudFlare 用户推出测试版，包括那些拥有每月 20 美元专业版帐户的用户。然而，CloudFlare 的好心人也给了我们 50 个免费使用 Mirage 2.0 测试版的促销代码，即使你只是使用免费帐户。如果你有兴趣——也是 CloudFlare 用户——只需[到这里注册](https://web.archive.org/web/20221206051331/https://www.cloudflare.com/mirage-beta-techcrunch)。