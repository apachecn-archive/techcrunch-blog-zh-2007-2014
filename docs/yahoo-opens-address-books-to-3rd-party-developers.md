# 雅虎向第三方开发者开放通讯录 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/06/04/yahoo-opens-address-books-to-3rd-party-developers/>

# 雅虎向第三方开发者开放地址簿

[![](img/d2500fddc104f871ffe08a84577caa02.png)](https://web.archive.org/web/20221209114355/http://www.crunchbase.com/company/yahoo)

雅虎今天发布了一个[地址簿 API](https://web.archive.org/web/20221209114355/http://developer.yahoo.com/addressbook) ，它将让第三方开发者无需传统但原始的页面抓取方法就能访问雅虎用户的联系人列表。

除了搜索特定的联系人和字段并读取其数据，开发人员还可以使用它来添加联系人和更改现有记录(尽管开始时，只有预先批准的开发人员有权进行编辑)。

雅虎开发者网络负责人 Chris Yeh 认为这次发布是雅虎开放服务(YOS)活动的第二个主要“证据”，该活动在三月份的 Web 2.0 博览会上开始。第一点是[搜索猴子](https://web.archive.org/web/20221209114355/http://www.beta.techcrunch.com/2008/04/24/yahoo-open-search-platform-launches-into-private-beta/)，它让任何人都有可能增强网站结果在雅虎搜索中的显示方式。

就像微软和谷歌自己的联系 API 一样，雅虎已经决定实施一个专有的许可系统——他们称之为[bb auth](https://web.archive.org/web/20221209114355/http://developer.yahoo.com/auth/)——而不是实施像 [oAuth](https://web.archive.org/web/20221209114355/http://en.wikipedia.org/wiki/OAuth) 这样的开放协议。Yeh 说他希望看到 oAuth 在短期内被雅虎采用，尽管他不能说什么时候会发生。

LinkedIn 和 Plaxo 是两家合作伙伴，他们已经实现了新的 API，甚至在过去几个月里公开使用了它。

Yeh 说，目前还没有政策来限制开发者可以存储和使用他们从 API 中提取的数据的时间。但是，正如它的许多开发者倡议一样，雅虎保留停止它认为不良行为的权利。

正如戴夫·麦克卢尔最近向我建议的那样，如果开发者不仅能从雅虎、Hotmail 和 Gmail 等网络邮件服务中检索基本的联系人信息，还能确定用户与这些联系人的关系类型，那将是非常强大的。例如，如果我想找出用户的前 5 个联系人，我可以通过查看发送给所有联系人的消息的频率来实现。这种查找可以通过只针对具有特定关键字的消息来改进，以便属于特定类别的联系人(例如，高尔夫爱好者)可以通过他们的消息来识别。

不幸的是，雅虎的新 API 没有这种高级查询功能，至少在开始时没有。叶向我保证，YOS 竞选团队中的其他团队正在研究如何识别通讯录中的关系，所以我们希望将来能看到这种功能。