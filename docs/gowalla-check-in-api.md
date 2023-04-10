# Gowalla 最终发布了他们的签入 API，提供了一些不错的工具和 OAuth 2 支持 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/08/09/gowalla-check-in-api/>

# Gowalla 最终发布了他们的签入 API，提供了一些不错的工具和 OAuth 2 支持

你可以说阻碍基于位置的服务发展的原因之一是没有完整的 API 支持。毕竟，竞争对手 Foursquare 自去年 11 月以来已经拥有了完整的 API 摇摆和滚动[。但是过了今天，你就不能再这样争论了。](https://web.archive.org/web/20221006074443/https://beta.techcrunch.com/2009/11/16/foursquare-api/)

Gowalla 刚刚正式[宣布](https://web.archive.org/web/20221006074443/http://gowalla.com/blog/2010/08/hello-3rd-party-apps-gowalla-checks-in-with-oauth/)他们的签到 API 现在对所有开发者开放。这是今年二月发布的 API Gowalla [的扩展。值得注意的是，该 API 是只读的——但今天的添加也为 Gowalla 生态系统带来了完整的写功能。](https://web.archive.org/web/20221006074443/https://beta.techcrunch.com/2010/02/09/gowalla-to-roll-out-api-today/)

第三方开发者已经[向](https://web.archive.org/web/20221006074443/https://beta.techcrunch.com/2010/05/12/gowalla-api-problems/)请求这种写支持很长时间了。今年早些时候，我与联合创始人乔希·威廉姆斯交谈时，他说写作支持一直在计划中，他们只是必须找到正确的方式。随着 OAuth 2 的使用，他们相信他们已经找到了方法。

[OAuth 2](https://web.archive.org/web/20221006074443/http://tools.ietf.org/html/draft-ietf-oauth-v2-08) 被认为是更安全的远程认证版本。如果你一直在关注 [OAuth WRAP](https://web.archive.org/web/20221006074443/http://wiki.oauth.net/OAuth-WRAP) 的开发，那已经被 OAuth 2 取代了。像脸书、微软、谷歌和雅虎这样的公司已经为这个想法努力了一段时间，脸书甚至[用 FriendFeed 作为它的试验场](https://web.archive.org/web/20221006074443/https://beta.techcrunch.com/2009/12/21/facebook-friendfeed-oauth-wrap/)。

Gowalla 谈到 OAuth 2 时说:

> 在今天的版本中，我们扩展了可能性，使您的应用程序能够代表用户创建签入。这是通过我们的 OAuth 2.0 实现的，OAuth 2.0 允许用户安全地授权访问他们的 Gowalla 帐户。

Gowalla 还更新了他们的 [API Explorer](https://web.archive.org/web/20221006074443/http://gowalla.com/api/explorer#/spots?lat=30.2697&lng=-97.7494&radius=50) 工具，展示你可以用他们的 API 访问哪些数据。像 Gowalla 上的大多数东西一样，这个功能看起来很光滑。

一段时间以来，许多第三方一直在使用 Gowalla 的 API 来构建有趣的工具，如[Gowalla walk](https://web.archive.org/web/20221006074443/http://gowallawalk.com/)——一款外观精美的应用程序，以可视化的方式向您显示您去过的地方。也有一些工具，像 [Check.in](https://web.archive.org/web/20221006074443/http://check.in/) ，一直在使用 Gowalla 的 API 中的[变通方法来检查用户，即使没有完全支持。现在他们大概可以合法地这么做了。](https://web.archive.org/web/20221006074443/https://beta.techcrunch.com/2010/03/25/check-in/)