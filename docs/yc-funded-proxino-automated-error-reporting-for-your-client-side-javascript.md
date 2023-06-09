# YC 资助的 Proxino:为您的客户端 JavaScript TechCrunch 提供自动错误报告

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/08/22/yc-funded-proxino-automated-error-reporting-for-your-client-side-javascript/>

这里有一个新的由 Y Combinator 支持的初创公司，它肯定会吸引大量 web 开发人员的目光: [Proxino](https://web.archive.org/web/20230131031305/http://www.proxino.com/) ，这是一个新的服务，它承诺让开发人员检测他们所有客户端 JavaScript 上的错误，而不必用重复的错误处理命令手动包装他们的代码。

首先，有点高层背景。与 Python 等在你访问的网站的服务器上执行的语言不同，JavaScript 代码通常在你的 web 浏览器上本地执行。这允许快速的响应时间和漂亮的效果，但是有一个缺点:开发者很难弄清楚他们的站点是否给一些用户带来了问题。每个浏览器执行代码的方式都不一样——如果出现问题，开发人员不会自动收到错误报告。

有一些方法可以解决这个问题。开发人员可以构建自己的测试套件，自动检查各种浏览器的大量测试用例。他们还可以在代码中用异常处理程序包装每个函数。但 Proxino 的创始人表示，测试套件并不完美(最糟糕的错误是那些逃过这些测试的错误)，许多开发人员不想手动添加错误处理。

这就是普罗西诺的用武之地。开发人员通过 Proxino 的代理服务器传递他们的 JavaScript 应用程序，代理服务器会自动用生成异常报告的代码包装应用程序的每个部分，因此每当用户的浏览器出现问题时，他们都会收到 pinged。代理还可以精简代码以减少下载时间，并缓存 JavaScript 应用程序以进一步加快速度。他们会自动将其他语言，比如 CoffeeScript，转换成可检测的、捕捉异常的 JavaScript。

当然，代理服务器有一个潜在的缺点:如果服务器宕机，你的应用可能会宕机，而你无法直接控制它再次工作。为了补救这一点，Proxino 使用了一种回退技术——如果 Proxino 出现故障，您只需像往常一样从自己的服务器开始提供 JavaScript 应用程序。

![](img/7cd23ba6fef97a11331b33d5f0530fc1.png)

Proxino 承认已经有一些工具可以帮助优化 JavaScript，比如 Google 的 closure 编译器。但他们说，没有多少工具能让开发人员很好地检测浏览器中的错误——他们说，他们的竞争对手在不同的浏览器中表现不一致，如 Webkit 和 Opera。

Proxino 根据您网站的流量收费。每月访问量低于 1000 的低流量网站有一个免费版本；第一个付费等级是每月 30 美元，最多 10，000 次页面浏览(你可以在这里看到他们的完整价目表[)。](https://web.archive.org/web/20230131031305/https://www.proxino.com/plan)

从长远来看，Proxino 有一些非常雄心勃勃的目标:他们说他们想“为世界的 Javascript 服务”。