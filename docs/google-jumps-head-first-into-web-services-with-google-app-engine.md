# 谷歌凭借谷歌应用引擎率先进入网络服务领域

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/04/07/google-jumps-head-first-into-web-services-with-google-app-engine/>

我们对谷歌应用引擎发布活动[的现场报道在这里](https://web.archive.org/web/20230327002257/https://techcrunch.com/2008/04/07/live-from-google-campfire-one/) ( **更新:**我们已经在这里构建并发布了[测试应用。](https://web.archive.org/web/20230327002257/https://techcrunch.com/2008/04/08/techcrunch-labs-our-experience-building-and-launching-app-on-google-app-engine/)

[![](img/22b23d1270d5a6647f078d603f72a131.png)](https://web.archive.org/web/20230327002257/http://www.crunchbase.com/product/google-app-engine)

谷歌不再仅仅谈论在云中托管应用程序。今晚太平洋时间 9 点，他们将发布[谷歌应用引擎](https://web.archive.org/web/20230327002257/http://code.google.com/appengine/) ( **更新**:该网站已上线)，这是一个雄心勃勃的新项目，提供一个全栈、托管、自动扩展的网络应用平台。它由 Python 应用服务器、 [BigTable](https://web.archive.org/web/20230327002257/http://labs.google.com/papers/bigtable.html) 数据库访问(这里预计[这里](https://web.archive.org/web/20230327002257/https://techcrunch.com/2008/04/04/source-google-to-launch-bigtable-as-web-service/)和[这里](https://web.archive.org/web/20230327002257/https://techcrunch.com/2008/04/06/major-google-announcement-monday-evening-is-it-bigtable/))和 [GFS](https://web.archive.org/web/20230327002257/http://labs.google.com/papers/gfs.html) 数据存储服务组成。

乍一看，这是亚马逊提供的一套[网络服务](https://web.archive.org/web/20230327002257/http://www.amazon.com/b?ie=UTF8&node=342335011&me=A36L942TSJ2AJA)的完全竞争对手，包括 [S3](https://web.archive.org/web/20230327002257/http://aws.amazon.com/s3) (存储) [EC2](https://web.archive.org/web/20230327002257/http://aws.amazon.com/ec2) (虚拟服务器)和 [SimpleDB](https://web.archive.org/web/20230327002257/http://www.amazon.com/SimpleDB-AWS-Service-Pricing/b/ref=sc_fe_l_2?ie=UTF8&node=342335011&no=3440661&me=A36L942TSJ2AJA) (数据库)。

与 Amazon Web Services 的松散耦合架构不同，它由几个本质上独立的服务组成，开发人员可以随意将这些服务捆绑在一起，Google 的架构更加统一，但灵活性较差。例如，亚马逊可以独立于任何其他服务使用他们的存储服务 S3，而谷歌使用他们的 BigTable 服务将需要编写和部署一个 Python 脚本到他们的应用服务器，这将创建一个 web 可访问的 BigTable 接口。

这一切意味着:谷歌应用引擎是为那些想在谷歌资源上运行他们的整个应用程序栈的开发者设计的。相比之下，亚马逊提供了更多的点菜服务，开发者可以挑选他们想要使用的资源。

谷歌产品经理 Tom Stocky 在今天的采访中向我描述了这项新服务。开发人员只需将他们的 Python 代码上传到 Google，启动应用程序，就可以通过多平台桌面应用程序监控使用情况和其他指标。

来自谷歌的更多细节:

> 今天，我们宣布了 Google App Engine 的预览版，这是一个应用托管工具，开发者可以使用它在 Google 的基础设施上构建可扩展的 web 应用。目标是让 web 开发人员更容易构建和扩展应用程序，而不是专注于系统管理和维护。
> 
> 利用谷歌应用引擎，开发者可以:
> 
> *   **编写一次代码，然后部署。**为 web 服务和数据存储供应和配置多台机器既昂贵又耗时。Google App Engine 通过根据需要动态提供计算资源，使部署 web 应用程序变得更加容易。开发人员编写代码，Google App Engine 负责剩下的工作。
> *   **吸收交通高峰。**当一个 web 应用程序大受欢迎时，流量的突然增加可能会让各种规模的应用程序不堪重负，从初创公司到大型公司，他们发现自己每年都要对数据库和整个系统进行数次架构调整。通过自动复制和负载平衡，Google App Engine 利用 Bigtable 和 Google 可扩展基础架构的其他组件，可以更容易地从一个用户扩展到一百万个用户。
> *   **轻松集成其他谷歌服务。对于开发人员来说，为每个新的应用程序从头开始编写像身份验证和电子邮件这样的组件是不必要的，也是低效的。使用 Google App Engine 的开发人员可以利用内置组件和 Google 更广泛的 API 库，为简单但重要的功能提供即插即用功能。**

**谷歌应用引擎:局限性**

这项服务正在测试阶段，有很多限制。

首先，只有前 10，000 名注册测试版的开发者才被允许部署应用程序。

这项服务在测试期间是完全免费的，但是有使用上限。应用程序每天不能使用超过 500 MB 的总存储、2 亿兆周期/天的 CPU 时间和 10 GB 的带宽(双向)。我们被告知，对于典型的网络应用程序来说，这相当于大约 500 万次页面浏览量/月。测试期结束后，这些上限将被取消，但开发者需要为任何超额支付费用。谷歌尚未确定这项服务的价格。

当前的一个限制是要求应用程序用 Python 编写，Python 是一种用于构建现代 web 应用程序的流行脚本语言(Ruby 和 PHP 等被广泛使用)。Google 说 Python 只是第一个被支持的语言，并且整个基础设施被设计成语言中立的。谷歌最初对 Python 的关注是有意义的，因为他们在内部使用 Python 作为他们的脚本语言(他们在 2005 年雇佣了 Python 的创造者[吉多·范·罗苏姆](https://web.archive.org/web/20230327002257/http://www.oreillynet.com/onlamp/blog/2005/12/python_creator_guido_van_rossu.html))。

**更新**:吉多·范·罗苏姆在发布会上谈论 App Engine: