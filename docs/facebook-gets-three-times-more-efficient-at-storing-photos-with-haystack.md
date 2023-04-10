# 脸书在巨大的干草堆中寻找照片的效率提高了三倍

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/04/30/facebook-gets-three-times-more-efficient-at-storing-photos-with-haystack/>

# 脸书在巨大的干草堆中寻找照片的效率提高了三倍

![](img/dd39f0e59219563999b22b9a360dc4b1.png)

拥有超过 150 亿张照片(以及 600 亿个不同大小的复制图像文件)，仅照片应用程序一项，脸书就消耗了大量存储空间。会员每周新增 2.2 亿张照片。脸书目前拥有超过 1.5 的照片存储空间，并且还在以每周 25tb 的速度增长。去年，脸书仅在 NetApp 存储设备上就花费了[约 3000 万美元](https://web.archive.org/web/20221007064625/http://www.beta.techcrunch.com/2008/10/31/facebooks-growing-problem/)，仅仅是为了跟上照片和其他上传内容的增长。为了降低部分成本，脸书决定设计自己的存储架构，名为 [Haystack](https://web.archive.org/web/20221007064625/http://www.beta.techcrunch.com/2009/04/06/facebook-completes-rollout-of-haystack-to-stem-losses-from-massive-photo-uploads/) 。

现在，关于这个系统实际上是如何运作的更多细节已经浮出水面。简而言之，Haystack 将允许脸书从昂贵的商业存储设备转向现成的商品硬件。它正从传统的网络文件系统转变为更类似于精简的网络应用程序，只做它需要做的事情。脸书不仅将获得日常用品的成本节约，还将获得 3 倍的存储容量提升。换句话说，过去需要 30 张光盘才能存储的东西，现在只需要 10 张。

面对数十亿张图片，找到合适的就像大海捞针。在传统的网络文件系统中，大量的元数据飞来飞去，详细描述了文件最后一次修改的时间、它们被列在什么目录中等等。所有这些元数据在来回传递时都会造成瓶颈。因此，建造 Haystack 的两位脸书工程师(Doug Beaver、Peter Vajgel 和 Jason Sobel)决定去掉大部分元数据。正如他们在脸书的[工程博客](https://web.archive.org/web/20221007064625/http://www.facebook.com/FacebookEngineering#/note.php?note_id=76191543919&ref=mf)上解释的那样:

> 新的照片基础架构将照片服务层和存储层合并为一个物理层。它实现了一个基于 HTTP 的照片服务器，将照片存储在一个名为 Haystack 的通用对象存储中。新层的主要要求是消除照片读取操作的任何不必要的元数据开销，以便每个读取 I/O 操作只读取实际的照片数据(而不是文件系统元数据)

所有的元数据都存储在脸书所谓的“针”里每根针汇集了成千上万张图像的元数据。这些针与一个索引成对出现，组成了干草堆对象存储。你可以在脸书工程博客上阅读所有的技术细节。该公司将为已经上传的 150 亿张照片保留其现有的网络文件系统(毕竟，那些 NetApp 盒子是沉没成本)。但今后，所有新照片的上传都将由 Haystack 处理。在未来，脸书甚至可能开源该架构，以便其他公司可以从中受益。对于一个由三个工程师建造的东西来说，还不错。

(图片来源:Flickr/ [熊伟·安图内斯](https://web.archive.org/web/20221007064625/http://www.flickr.com/photos/janeladeimagens/166051502/))