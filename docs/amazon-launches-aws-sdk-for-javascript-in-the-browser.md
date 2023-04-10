# 亚马逊在浏览器中推出 AWS SDK For JavaScript 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/10/31/amazon-launches-aws-sdk-for-javascript-in-the-browser/>

# 亚马逊在浏览器中推出面向 JavaScript 的 AWS SDK

亚马逊今天[发布了](https://web.archive.org/web/20230118210101/http://aws.typepad.com/aws/2013/10/developer-preview-aws-sdk-for-javascript.html)其 [AWS SDK for JavaScript](https://web.archive.org/web/20230118210101/http://aws.amazon.com/sdkforbrowser/) 的开发者预览版。有了它，开发人员现在可以轻松地构建动态 JavaScript 应用程序，这些应用程序可以从浏览器[访问 AWS 服务](https://web.archive.org/web/20230118210101/https://aws.amazon.com/sdkforbrowser/)，而不需要编写任何服务器端代码，也不需要配置应用服务器进行托管。

亚马逊之前发布了 Node.js 应用软件的 SDK，所以这不是亚马逊第一次尝试支持 JavaScript。事实上，这个新的 SDK 在浏览器和服务器端 Node.js 代码中使用了相同的编程模型。

有了这个新的 SDK，开发人员可以直接调用亚马逊的 S3 存储服务，亚马逊 SQS 读取和写入消息队列，社交网络生成和处理移动通知，以及亚马逊的 DynamoDB NoSQL 数据库。目前还不能访问亚马逊更传统的数据库服务。这意味着开发人员现在可以构建 JavaScript 应用程序，例如，可以创建流行的 S3 桶，并查询 DynamoDB 表，而无需通过任何服务器端代码访问这些服务。

要访问这些功能，开发人员需要添加一个标签，将亚马逊的 JavaScript 库集成到他们的代码中。SDK 支持 Amazon 的 web identity federation 特性(毕竟，您不会想在 HTML 和 JavaScript 中添加 AWS 凭证)。通过这样做，你也可以使用公共身份提供商，比如脸书、谷歌或者当然还有亚马逊自己。

就像亚马逊的所有东西一样，设置并不完全琐碎，但是该公司已经创建了一些教程[来帮助你开始。](https://web.archive.org/web/20230118210101/https://aws.amazon.com/developers/getting-started/browser/)