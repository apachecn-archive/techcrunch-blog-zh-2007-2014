# Android 版 WhatsApp 的漏洞让黑客窃取你的对话

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/03/12/hole-in-whatsapp-for-android-lets-hackers-steal-your-conversations/>

# 安卓版 WhatsApp 的漏洞让黑客窃取你的对话

作为主要是 Android 安全问题的一部分，一名首席技术官兼顾问[发现了](https://web.archive.org/web/20230406203744/http://bas.bosschert.nl/steal-whatsapp-database/#comment-3)WhatsApp 加密中的一个漏洞，该漏洞可能允许另一个应用程序访问并读取用户在其中的所有聊天对话。

DoubleThink 的首席技术官 Bas Bosschert 发布了他自己访问 WhatsApp 聊天的方法，并证实在[昨天的 Android 大更新](https://web.archive.org/web/20230406203744/https://techcrunch.com/2014/03/11/whatsapp-for-android-update-lets-users-pay-for-their-friends-subscriptions/)之后，该漏洞仍然存在。

它是这样工作的:

WhatsApp for Android 将对话存储在手机的 SD 卡上，只要用户给予这些应用所需的权限，手机上的许多其他应用就可以访问 sd 卡(许多应用要求完全访问手机)。这是 Android 的基础设施问题，而不是 WhatsApp 的安全漏洞。

从那里，恶意应用程序可以访问 WhatsApp 的对话数据库。精明的用户会注意到，这很难称得上是黑客，而更像是 Android 数据沙箱系统的问题。

Bosschert 建立了一个配套的应用程序来测试它，并在上传数据库文件时使用一个可爱的加载屏幕来分散用户的注意力。

在最近的版本中，WhatsApp 已经开始加密数据库，加密到无法用 SQLite 打开的程度，但 Bosschert 报告说，他可以用自己的 Python 脚本解密数据库。

你可以在[这里](https://web.archive.org/web/20230406203744/http://bas.bosschert.nl/steal-whatsapp-database/#comment-3)找到破解的分步指南。

在 190 亿美元的收购后，脸书肯定会在未来几个月内改善 WhatsApp 的安全性。但这又一次带来了关于 Android 基础设施的挥之不去的问题。

在 Android 上，任何对智能手机拥有完全访问权限的应用程序(很多都是这样)都可以访问其他应用程序的数据，并将其上传到第三方。

相比之下，苹果不允许访问应用程序自身沙盒之外的数据，这阻止了恶意开发者通过虚拟应用程序修改你的数据，如上所述。