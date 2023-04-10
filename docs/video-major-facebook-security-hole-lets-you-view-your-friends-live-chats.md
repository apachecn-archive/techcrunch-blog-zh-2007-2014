# 视频:脸书重大安全漏洞让你可以查看你朋友的实时聊天

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/05/05/video-major-facebook-security-hole-lets-you-view-your-friends-live-chats/>

# 视频:主要脸书安全漏洞让你查看你的朋友的实时聊天

![](img/f328809ee0b3b8d012755b8e5e775068.png)

你必须把它交给[脸书](https://web.archive.org/web/20230204205348/http://www.facebook.com/)。他们当然知道如何实现安全——但不知道。

今天有人向我报告说，这个社交网站有一个重大的安全漏洞，只要点击几下鼠标，任何用户都可以查看他们“朋友”的*实时聊天*。使用听起来很简单的技巧，用户还可以访问他们朋友的最新好友请求，以及他们共同分享的好友。这是很多潜在的敏感信息。

我觉得不可思议，直到我亲自测试了这个漏洞。

你猜怎么着？它工作了。

具有讽刺意味的是，这个漏洞是通过脸书让你预览自己的隐私设置来实现的。换句话说，隐私*功能*包含一个缺陷，如果其他人知道这个漏洞，他们就可以查看私人信息。

我知道脸书希望我们分享更多的信息并开放，但我不确定这是不是他们想要的。

因为这对用户隐私有重大影响，我们已经通知了脸书关于这个漏洞。

这是该漏洞的视频。

<param name="wmode" value="transparent"><param name="allowFullScreen" value="true"><param name="allowscriptaccess" value="always"><param name="src" value="http://www.youtube.com/v/ny8ui4delEo&amp;hl=en_US&amp;fs=1&amp;"><param name="allowfullscreen" value="true">

(帽尖: [@Scott56r](https://web.archive.org/web/20230204205348/http://www.twitter.com/Scott56r) 和 [@Laird_Attwood](https://web.archive.org/web/20230204205348/http://www.twitter.com/Laird_Attwood) )

几个小时后，脸书给我们发来了这份声明。

“在有限的一段时间内，一个漏洞允许一些用户通过操纵脸书隐私设置的“预览我的个人资料”功能，向他们的朋友显示他们的聊天信息和未决的好友请求。当我们收到问题报告时，我们的工程师迅速进行了诊断，并暂时禁用了聊天功能。我们还推出了一个解决可视好友请求的补丁，现在已经完成了。聊天将很快在整个网站上重新打开。我们迅速解决了这个问题，确保一旦有人向我们报告了这个问题，我们就能迅速找到并实施解决方案。"