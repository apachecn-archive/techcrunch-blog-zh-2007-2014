# Appsfire 宣布 iOS 的开源 UDID 替代品:OpenUDID TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/09/01/appsfire-announces-open-source-udid-replacement-for-ios-openudid/>

移动应用营销平台 Appsfire 推出了自己的解决方案，以解决苹果公司决定逐步取消开发者在 iOS 设备上使用 UDID(唯一设备标识符)的问题。它叫做 [OpenUDID](https://web.archive.org/web/20230204225529/http://openudid.com/) 。正如您可能已经猜到的名字，这是一个开放源代码的 UDID 倡议。

换句话说，它试图创建一个非专有的解决方案，旨在取代所有失去的东西，并且所有利益相关者都可以参与其中。

在最近的一组 iOS5 发行说明[中提到了对 UDID 访问的更改，并将其列为“已弃用](https://web.archive.org/web/20230204225529/https://techcrunch.com/2011/08/19/apple-ios-5-phasing-out-udid/)”对于那些不知道的人来说，UDID 是每个苹果设备独有的字母数字字符串，目前被移动广告网络、游戏网络、分析提供商、开发者和应用测试系统使用，例如 [TestFlight](https://web.archive.org/web/20230204225529/http://www.testflight.com/) 。在某些情况下，开发者甚至使用 UDID 来验证用户是否正在通过新设备访问他们的应用程序。

通过在 iOS5 中移除对 UDID 的访问，苹果已经将整个生态系统置于混乱之中。

上周，移动游戏网络 [OpenFeint 推出了一个名为 OFUID](https://web.archive.org/web/20230204225529/https://techcrunch.com/2011/08/26/openfeint-announces-replacement-for-udids-on-ios/) 的 UDID 替代品，为游戏开发者社区提供了一个解决方案。选择加入 OpenFeint 新的单点登录系统的用户因此可以让开发者访问这个 OFUID，这是一个面向游戏网络跨平台用户的通用账户系统。OFUID 允许开发者追踪用户在不同应用中的行为，并帮助他们进行广告定位。

但是这个系统被批评为不完全的 UDID 替代品，并且是其专有性质。

新提出的 OpenUDID 将有所不同。

[表示](https://web.archive.org/web/20230204225529/http://blog.appsfire.com/appsfire-introduces-the-open-source-openudid-initiative/) Appsfire:

> *由于 Appsfire 既是消费者应用程序的开发商，也是广告网络的开发商，我们寻求 UDID 的替代者，但对任何单一提供商拥有的解决方案都不感兴趣。我们还预见到了一个分散的市场，在这个市场中，UDID 管理由多个提供商运营，它们之间没有合作。为了帮助我们自己和成千上万的其他移动应用程序开发者，我们开始致力于 OpenUDID 开源倡议。*

该公司表示，它希望与其他公司合作，为每个设备的通用唯一设备标识符提供可靠的代理和替代。它还希望 OpenUDID 能够被任何应用程序访问，提供开源代码来为 iOS(以及后来的 Android)生成和访问 OpenUDID，并从一开始就纳入一个允许用户选择退出的系统。

AppsFire 解释说，后一个要求是因为新系统应该“符合苹果的最初意图”。苹果没有说明为什么决定移除 UDID。它做出这一改变可能是为了回应之前的隐私担忧，或者是为了预先防范未来的担忧。但不管是哪种情况，很明显，该公司正在采取措施，通过移除 UDID 来进一步尊重用户的隐私。新的开源系统应该尊重苹果在这件事上的决定。

Appsfire 已经发布了一个简单的 Objective-C 类，它提供了一行代码来利用 [github](https://web.archive.org/web/20230204225529/http://openudid.com/) 上的 OpenUDID。该公司表示，现在邀请所有移动应用开发者加入测试过程。

http://OpenUDID.com 的网址[也指向了新的 github 页面。](https://web.archive.org/web/20230204225529/http://openudid.com/)