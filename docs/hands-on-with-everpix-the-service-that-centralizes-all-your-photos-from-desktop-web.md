# 使用 Everpix，这项服务可以集中管理桌面和网络 TechCrunch 上的所有照片

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/10/22/hands-on-with-everpix-the-service-that-centralizes-all-your-photos-from-desktop-web/>

在过去的一周里，我一直在测试 Everpix 服务的 alpha 版本，该服务旨在自动集中和组织你所有的数码照片，无论是在线还是离线。我很高兴地告诉大家，到目前为止，它的效果和宣传的一样。

如果你错过了，前苹果工程师创造的 Everpix 是[今年 TechCrunch Disrupt 决赛入围者之一](https://web.archive.org/web/20230203085143/https://techcrunch.com/2011/09/12/everpix-all-your-photos-automatically-organized-and-accessible-from-anywhere/)。Everpix 使用一个在电脑上运行的小工具，让你连接到当地的照片商店，脸书、Flickr、Picasa 和 Instagram 等在线服务，甚至连接到 Gmail 中发送给你的照片。

鉴于 Everpix 的两位联合创始人 [Pierre-Olivier Latour](https://web.archive.org/web/20230203085143/http://www.crunchbase.com/person/pierre-olivier-latour) 和 [Kevin Quennesson](https://web.archive.org/web/20230203085143/http://www.linkedin.com/in/kevinquennesson) 都曾在苹果*工作过几年(联合创始人 [Wayne Fan](https://web.archive.org/web/20230203085143/http://www.linkedin.com/pub/wayne-fan/36/541/233) 曾在 [frog design](https://web.archive.org/web/20230203085143/http://www.crunchbase.com/company/frog-design) )，*ever pix 首先面向 Mac 用户推出并不令人意外。

首先，您需要安装一个实用程序，在 Mac 的菜单栏中放置一个图标。最初，同步可能会降低电脑的速度，因为它会上传整个照片图库。出于这个原因，在睡觉前开始上传可能是个好主意，这样就不会打断你的工作。

点击菜单栏图标将带您到 Everpix 网站，在那里您可以配置您想要连接的各种服务，并指向您桌面上包含您想要在线同步的照片的文件夹。

[![](img/51849f289d314cd27b5a2cf96927d29f.png "everpix-settings")](https://web.archive.org/web/20230203085143/https://techcrunch.com/wp-content/uploads/2011/10/everpix-settings.png)

对于那些在电脑上使用复杂的文件夹中文件夹系统来组织照片的人来说，你可能会有点失望地发现，使用 Everpix，你不能选择只上传选定的文件夹或文件。您必须全局启用或禁用整个图片文件夹(或者也可以选择启用或禁用您的文档和桌面)。然而，我认为，对于大多数人来说，这将是一个功能，而不是一个错误。由于在可以同步的内容方面提供了更少的选择，它简化了设置，减少了启动所需的点击量。*(你点击图标，进入“照片来源”然后点击你想联机的文件夹。也就是两次点击)。*

不过，在我的情况下，我用来保存博客文章中出现的照片的文件夹是在我的图片文件夹中，我不想在 Everpix 的网站上把这些照片和我的家庭照片放在一起。看来，我将被迫把那个文件夹转移到别处。

默认情况下，你所有的照片都是私人的，除非你另外指定，否则将一直保持私人状态，所以除非你有一些真正的个人照片，否则我不会太担心把它们发布到网上。当然，看到一个安全的 URL(即以 https://…)开头的 URL 会让我感觉舒服一些。

从 Everpix 网站上，你可以选择启用额外的在线照片共享服务，所有这些服务都使用 OAuth 连接，或者在脸书的情况下，使用脸书连接。最令人失望的是 Gmail。尽管事实上 [Gmail 早在 2010 年 3 月就增加了对 OAuth](https://web.archive.org/web/20230203085143/https://techcrunch.com/2010/03/01/gmail-security-enhancements-expected-tuesday/) 的支持，Everpix 直接要求你输入 Gmail 用户名和密码，并指出它将存储你的加密密码或其服务器。*不用了，谢谢。当有更好的方法可用时，根本没有理由用这种方式处理事情。我选择不连接我的 Gmail，并且在 OAuth 得到支持之前不会这样做。*

[![](img/89e327e334463f673135e32db06bbd7b.png "everpix-photo-groups")](https://web.archive.org/web/20230203085143/https://techcrunch.com/wp-content/uploads/2011/10/everpix-photo-groups.png)

至于服务的组织方面，Everpix 兑现了承诺——它将照片按“时刻”分组。这些时刻是代表生活事件的时间段。在大多数情况下，我发现照片是按日期分组的，但在某些情况下，它知道将我在白天拍摄的照片与晚上拍摄的照片分开。

我对“时刻”功能的一个愿望是希望手动将这些分组组合成一个。例如，像 TechCrunch Disrupt 这样的会议的照片分散在好几天，而我宁愿把它保存为一个瞬间。由于所有照片对人眼来说都很容易识别，属于同一个组(即绿色背景，会议舞台)，很明显没有超级智能的机器算法来处理分组。

[![](img/dcd77d57bd7d3e4de03e30b42ce25582.png "everpix-combine")](https://web.archive.org/web/20230203085143/https://techcrunch.com/wp-content/uploads/2011/10/everpix-combine.png)

另一大特色，自动监管，我更喜欢。在大型照片集中，该服务将运行整个批处理并隐藏(而不是删除)不良照片，如模糊、失焦、黑暗、曝光不足或过度曝光的照片。只需点击页面底部的一个按钮，您就可以返回查看这些照片。要永久取消隐藏照片，只需点击照片上的箭头图标。

[![](img/3a0381b78249746764e2a7debf0af971.png "everpix-hidden")](https://web.archive.org/web/20230203085143/https://techcrunch.com/wp-content/uploads/2011/10/everpix-hidden.png)

最好的功能是 Everpix 简单的隐私设置。如上所述，默认情况下，所有照片都是隐私的，但只需点击一下，你就可以改变这一点。通过页面顶部的切换开关，可以通过提供的网址访问相册(或选择相册中的照片)，你可以通过脸书、推特或电子邮件分享该网址。

[![](img/686743522771f3db5d5c761a929b1c80.png "evernote-public-pix")](https://web.archive.org/web/20230203085143/https://techcrunch.com/wp-content/uploads/2011/10/evernote-public-pix.png)

总的来说，尽管服务很简单，但仍有许多 Everpix 缺乏的功能。例如，应该是纵向的照片却没有为你旋转，网站上也没有这样做的机制。*(当然，这可能也是它们出现在原始网站上的方式，但这会破坏体验。)【Everpix 即将推出的移动界面也是一个非常需要的补充，因为它将提供一种无论你在哪里都可以将照片放在手边的方式，另外还提供了一种更简单的从你的设备自动上传照片的方法。不过，这还在开发中，所以这只是时间问题。我也想给我的一些瞬间命名，给它们贴上标签，或者按人物、地点、日期或主题搜索，但是根本不提供搜索。*

如果 Everpix 能够引入 iPhoto 和脸书已经拥有的面部标签并将它们结合起来，那将是一个值得称赞的壮举。我想这是 Everpix 接下来要做的事情——不做的话，他们会疯掉的。我会说，一个全面的照片数据库需要是可搜索和结构化的，而不仅仅是有组织和漂亮的。

该公司仍然没有关于定价或公开发布的细节，但与此同时，我很高兴手头有这个资源。在此之前，我的照片一直在网络上广泛传播，没有简单的方法来集中它们。就这个特性而言，在我看来，Everpix 是一个值得拥有的工具。

Everpix 在这里接受注册。