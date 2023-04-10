# W3i 建议 iOS 开发者使用 MAC 地址作为 UDID 替代品 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/10/28/w3i-suggests-ios-developers-use-mac-address-as-udid-replacement/>

移动应用货币化和分发网络宣布了其测试结果，以确定 iPhone 的 MAC 地址是否可以取代 UDID(唯一的设备标识符)，这是苹果正在逐步淘汰的一种方式，开发者可以通过这种方式来跟踪应用的用户。

根据 W3i 的说法，开发者可以也应该开始跟踪 iPhone 的 MAC 地址，作为 UDID 的替代方案，因为它已经成功地看到苹果批准了自己的应用程序。不幸的是，这个建议可以说是不成熟的。苹果可能会推出一款应用，但如果大量 iOS 开发者开始做同样的事情(也就是追踪 MAC 地址)，苹果肯定会改变在这件事上的立场。

作为背景，8 月，Erick 报道了[苹果如何在 iOS5 中偷偷做了一个重大改变](https://web.archive.org/web/20230203100023/https://techcrunch.com/2011/08/19/apple-ios-5-phasing-out-udid/):不允许开发者访问 UDID。UDID 是每个苹果设备独有的字母数字字符串，已经被移动广告网络、游戏网络、分析提供商、开发者和应用测试系统使用，如 [TestFlight](https://web.archive.org/web/20230203100023/http://www.testflight.com/) 。在某些情况下，开发人员使用 UDID 来验证用户是否从新设备访问他们的应用程序，或者作为一种跨应用程序跟踪用户的方式。

自从这一变化被披露后，各公司都在争先恐后地想出解决办法。 [OpenFeint 宣布其 UDID 替代 OFUID](https://web.archive.org/web/20230203100023/https://techcrunch.com/2011/08/26/openfeint-announces-replacement-for-udids-on-ios/) 。 [AppsFire 提出了一个名为 OpenUDID](https://web.archive.org/web/20230203100023/https://techcrunch.com/2011/09/01/appsfire-announces-open-source-udid-replacement-for-ios-openudid/) 的开源解决方案。现在 W3i 建议开发者使用 iPhone 的 MAC 地址——特别是设备 Wi-Fi 网络接口的 MAC 地址。

MAC 地址也是唯一的标识符，用于物理网段上的通信。W3i 想要确定的是，在多种设备类型和不同配置(例如，飞行模式、Wi-Fi 关闭或打开、不在范围内等)下，是否可以可靠地捕获该地址。)

W3i 使用其专有应用程序 AppAllStar 于 10 月 5 日提交并获得批准，从 10 月 5 日到 10 月 22 日收集了 78，662 个 MAC 地址，代表了 iPhone、iPod Touch 和 iPad 设备上 100%的安装。在那段时间(10 月 1 日)，该应用程序也被重新提交，以纠正一些与测试无关的错误。在这两种情况下，该公司表示，它将代码放在了一个非常高的级别，同时也适当地命名了这些类。

然而，W3i 确实发现 33 个设备有重复的 MAC 地址，W3i 认为这可能表明越狱或山寨设备。其中一部分也有伪造的 UDIDs。关于复制品所在位置的数据很有趣。中国和荷兰各有 9 个副本，意大利有 5 个，西班牙 3 个，沙特阿拉伯 2 个，新加坡、美国、澳大利亚、捷克和印度各有 1 个。

基于这些发现，W3i 现在建议开发人员开始收集和存储带有相关 UDID 的 Wi-Fi MAC 地址，并修改应用程序逻辑以使用 UDID 和 Wi-Fi MAC 地址。

当然，所有这些建议从长远来看可能毫无价值。涉及单一应用程序的测试绝不是苹果会允许大规模应用的决定性证据。毕竟，考虑到取消开发者对 UDID 的访问是为了更好地尊重用户隐私，简单地允许开发者改用第二个唯一 ID 将违反苹果决定的精神，如果不是实际条款的话。