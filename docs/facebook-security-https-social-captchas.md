# 脸书通过社交验证码和所有 HTTPS 来增强安全性

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/01/26/facebook-security-https-social-captchas/>

# 脸书加强安全与社会验证码和所有 HTTPS，所有的时间

![](img/ac02e4857d1a5dc569a5164722c753be.png)

脸书引入了两项新措施来加强 T2 的安全:扩大 HTTPS 连接作为一个永久的选择和使用社交验证码来验证丢失密码的用户。让我们一次解决一个。

HTTPS 是一种安全连接(比普通的 HTTP 连接更安全)，脸书已经使用 HTTPS 通过脸书连接登录外部网站，并将密码发送回脸书。但是现在你可以选择将 HTTPs 设置为你在脸书上做任何事情的默认连接。网页在 HTTPS 上加载会慢一些，但是你也不会被那些通过 WiFi 使用类似 [Firesheep](https://web.archive.org/web/20230202233908/https://techcrunch.com/2010/10/24/firesheep-in-wolves-clothing-app-lets-you-hack-into-twitter-facebook-accounts-easily/) 的东西嗅探你密码的人[攻击](https://web.archive.org/web/20230202233908/https://techcrunch.com/2011/01/24/security-alert-tech-luminaries-easily-firesheeped-at-dld11/)。(也许脸书应该提供一个“更安全”的开/关按钮，当你在家或办公室没有安全网络时，你可以点击它)。一些应用开发者[将需要使用](https://web.archive.org/web/20230202233908/http://developers.facebook.com/blog/post/452)一个新的“安全画布 URL ”,这样他们的应用也可以通过 HTTPS 访问。

社交验证码功能非常聪明。它会用你一个朋友的照片代替普通的验证码(那些稍微有点扭曲的字母，要求你重新输入以证明你是人类)。当您试图找回丢失的密码或脸书检测到您帐户上的可疑登录活动时，您需要识别该人来验证您的身份。你知道你所有的“朋友”长什么样，不是吗？

[![](img/dcbdc5005f76bd69d194e5e96c6c8481.png "social captchas")](https://web.archive.org/web/20230202233908/https://techcrunch.com/wp-content/uploads/2011/01/social-captchas.jpeg)