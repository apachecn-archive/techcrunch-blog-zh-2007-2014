# 是时候建立一个开放的地点数据库了

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/04/17/open-database-places/>

![](img/54bfa25bbafe6b5b5b75875914981d0f.png)

随着 Twitter 上周宣布，它打算开始根据地理编码推文的坐标来识别地点，[地点土地热潮](https://web.archive.org/web/20230305230833/https://techcrunch.com/2009/12/23/location-2010/)正在如火如荼地进行。包括 Twitter、 [Google](https://web.archive.org/web/20230305230833/https://techcrunch.com/2009/12/16/check-in-google-foursquare-loopt/) 、 [Foursquare](https://web.archive.org/web/20230305230833/http://www.crunchbase.com/company/foursquare/posts) 、 [Gowalla](https://web.archive.org/web/20230305230833/http://www.crunchbase.com/product/gowalla/posts) 、 [SimpleGeo](https://web.archive.org/web/20230305230833/https://techcrunch.com/2010/03/19/location-gold-rush/) 、 [Loopt](https://web.archive.org/web/20230305230833/https://techcrunch.com/2009/11/03/loopt-shifts-its-strategy-to-tap-the-pulse-of-location/) 和 [Citysearch](https://web.archive.org/web/20230305230833/https://techcrunch.com/2010/01/29/citysearch-citygrid-local-advertising/) 在内的一长串公司在创建独立的地理坐标地图数据库方面进展很快。特别是，将企业映射到人们登记入住、发推文或锁定照片的 GPS 位置附近，是能够向他们显示地理定位广告的第一步，这可能有助于在很大程度上推动本地移动在线广告。

问题在于:这些创建底层地点数据库的努力是重复的，任何一家公司从比其他公司更全面中获得的任何竞争优势充其量都是短暂的。是时候建立一个开放的地方数据库了，所有的公司和开发商都可以贡献和借鉴。但是为了让这样一个数据库有用，最大和发展最快的 Geo 公司需要为它做出贡献。

前几天晚上，在一次聚会上，我向 Foursquare 的首席执行官丹尼斯·克劳利提出了这个建议，他对此很感兴趣。Foursquare 正在建立自己的综合性地点数据库，称之为“地点”，通过用户添加他们想要登记的地点，如果这些地点还不存在的话。Foursquare 将他们的 GPS 纬度/经度坐标与它的地点数据库(商业、兴趣点，甚至[人们的家](https://web.archive.org/web/20230305230833/https://techcrunch.com/2010/02/17/please-rob-me-makes-foursquare-super-useful-for-burglars/))进行匹配。后来，我通过电子邮件问克劳利:“你的用户建立的位置目录的质量难道不是一个竞争优势吗？”他的回答是:

> 是啊，但社交图也是。但 facebook connect 表明，当我们都表现良好时，事情会变得更好。“地点的 facebook 连接”将会是惊人的。不确定谁会建立它——Google、fbook、twitter 等——但我敢打赌，这个问题到明年大部分都会得到解决。有很多人在研究这个问题。

值得一提的是，Twitter 创始人杰克·多西那天晚上也正好在房间里，他的反应有点冷淡和谨慎。(我应该指出，多尔西没有以任何官方身份在 Twitter 上发言，这只是无聊的鸡尾酒会聊天)。但是考虑到 Twitter 最近从[搬到](https://web.archive.org/web/20230305230833/https://techcrunch.com/2010/04/09/twitter-fills-its-first-hole-with-an-official-blackberry-app/)[声称](https://web.archive.org/web/20230305230833/https://techcrunch.com/2010/04/09/twitter-acquires-tweetie/)更多的[部分](https://web.archive.org/web/20230305230833/https://techcrunch.com/2010/04/14/twitter-confirms-it-will-launch-its-own-link-shortener/)属于自己，以及由此产生的[争议](https://web.archive.org/web/20230305230833/https://techcrunch.com/2010/04/17/seesmic-tweetmeme-say-twitter-ecosystem-is-just-fine-thank-you/)，我突然想到 Twitter 可以通过创建这样一个开放的地点数据库来重新获得一些开发者失去的好感。我怀疑 Twitter 确实想创建“脸书地点连接”，并通过其 API 向开发者开放。它[收购了](https://web.archive.org/web/20230305230833/https://techcrunch.com/2009/12/23/twitter-acquires-mixer-labs/)的 Mixer Labs，当然[正朝着这个方向](https://web.archive.org/web/20230305230833/https://techcrunch.com/2009/11/12/geoapi-places-twitter-flickr/)发展，它的 [GeoAPI](https://web.archive.org/web/20230305230833/http://geoapi.com/) 仍得到 Twitter 的支持。希望地理编码推文中的所有地点数据也能放入其中。

一个脸书的地方连接还不够。克劳利的类比是站不住脚的，因为脸书仍然控制着社交图谱。它向其他网站和开发者公开了社交图(其成员之间的联系)，但其他网站无法自行添加到社交图中。一个真正开放的位置数据库应该允许给予和索取。它应该是一个每个人都可以贡献，但没有人必须拥有的东西。Foursquare 应该能够像 Twitter 或 Google 或任何其他 Geo 初创公司一样轻松地更新它。应以最佳数据为准。

相反的观点是，一些人——推特、谷歌、脸书——需要控制数据库，以确保其质量。如果你让任何一个地理应用程序的开发者更新数据库，它可能最终会充满不准确的地理数据，甚至更糟，地理垃圾邮件。我感觉多尔西的犹豫部分是因为这种担忧。但是肯定有办法设计一个奖励好数据而不是坏数据的地点数据库。也许一个地方直到两三个数据库同意它是同一个地方，或者基于来源的整体可信度和历史准确性，才成为官方的。

一个开放的位置数据库也会随着时间的推移而自我修正。而且，只有当特定的企业或地点从他们自己审查过的地理目录中消失时，公司才可以选择引用它。换句话说，让最好的数据占上风。不是十几家公司都在建立相同的地理目录，而是成千上万的公司可以在一个开放的数据库上创新新的地理服务、广告和应用程序。它应该只是移动网络基础结构的一部分。

*图片:Flickr/ [内特·博尔特](https://web.archive.org/web/20230305230833/http://www.flickr.com/photos/boltron/2947116237/)*