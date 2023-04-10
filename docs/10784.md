# Dropbox 的 API 获得了安全提升(现在是网络友好的)

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/10/21/dropboxs-mobile-api-gets-a-security-boost-and-is-now-mobile-web-friendly/>

# Dropbox 的 API 获得了安全提升(现在是网络友好的)

炙手可热的初创公司[Dropbox](https://web.archive.org/web/20230202020314/http://www.dropbox.com/)——你知道，刚刚以 40 亿美元的估值[筹集了 2.5 亿美元](https://web.archive.org/web/20230202020314/https://techcrunch.com/2011/10/18/dropbox-raises-250m-in-funding-boasts-45-million-users/)的文件同步服务——本周宣布了一项不如其大规模融资轮那么受关注的事情，但仍然令人兴奋:该公司[发布了其 API 的改进版本](https://web.archive.org/web/20230202020314/http://blog.dropbox.com/?p=915)，使该服务在本地应用程序(移动设备上)和网络应用程序方面都更好。

Dropbox first [在 2010 年 5 月发布了它的 API](https://web.archive.org/web/20230202020314/https://techcrunch.com/2010/05/04/dropbox-launches-android-app-mobile-api-gives-ipad-cloud-sync-apple-should-have-built/)，从那以后，它已经在许多移动应用程序中实现。但是新版本的 API 已经解决了一些问题。

首先，它现在增加了对“应用文件夹”的支持。在此次更新之前，如果你想让第三方应用程序连接到你的 Dropbox 账户，你需要让它访问你的整个*账户——这对于相机应用程序来说不一定有意义。现在，应用程序将能够将自己与一个单独的文件夹关联起来(用户可以随意移动和重命名该文件夹)，而不必交出王国的钥匙。*

同样，现在使用认证系统增强了安全性，该系统不需要您在第三方应用程序中输入凭据。相反，当你通过一个应用程序进行认证时，你会被切换到 Dropbox 的移动网络版本或你的原生 Dropbox 应用程序(脸书和其他一些服务使用类似的机制)。

该 API 还允许第三方应用程序访问 Dropbox 使用的版本控制/修订系统，这将允许用户跳转到文件的以前版本并取消删除。

最后，虽然 API 的原始版本主要是为本地移动应用程序设计的，但这个新版本也适用于 web 应用程序(包括桌面应用程序)。

**更新**:这篇文章的前一个版本说，安全更新和其他功能只适用于移动 eapp，但它们实际上与任何使用 Dropbox API 构建的应用程序(包括 web 应用程序)相关。