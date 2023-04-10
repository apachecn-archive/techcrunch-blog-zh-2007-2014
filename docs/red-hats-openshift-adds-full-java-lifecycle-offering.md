# Red Hat 的 OpenShift 增加了完整的 Java 生命周期产品 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2011/11/15/red-hats-openshift-adds-full-java-lifecycle-offering/>

Red Hat 的 [OpenShift](https://web.archive.org/web/20230204212750/https://openshift.redhat.com/) 平台即服务产品已经公开测试了一段时间。它为人们提供了一个相当简单的方法，通过抽象出所有设置应用程序和数据库服务器的麻烦事来启动“云”开发工作。相反，您只需将您的源代码发布到 OpenShift，他们的平台会完成剩下的工作。受支持的语言是那些被 nimble、agile 启动类型大量使用的语言:PHP、Python、Ruby。有趣的是，OpenShift 也支持 Java。许多人都不会将这种语言与云解决方案联系在一起。今天，Red Hat 宣布他们正在 OpenShift 上改进对 Java 的支持，支持“面向开发者的完整 Java 生命周期”。

我与红帽的 PaaS 主管 Issac Roth(一个很棒的头衔，如果曾经有过的话)和来自红帽中间件团队的 Jason Anderson 讨论了这个声明。根据 Roth 的说法，OpenShift 一直致力于支持开源开发者使用的那些技术——通常是 LAMP 堆栈中的“P ”,以及 Ruby。但 Red Hat 也希望支持企业开发者，并希望帮助企业开发者使用他们喜欢的语言开发云解决方案。通过今天的发布，他们正在以几种方式做到这一点。

首先，OpenShift 正在集成到 [JBoss Tools](https://web.archive.org/web/20230204212750/http://www.jboss.org/tools) 中，这是他们基于 Eclipse 的 Java 开发环境，“允许开发人员轻松地将他们的代码从领先的 Java IDE 推到云端。JBoss Developer Studio 的未来集成也在计划之中。我问 Roth 关于 OpenShift 与其他 ide 的集成，他向我保证工作正在进行中。事实上，[云 IDE](https://web.archive.org/web/20230204212750/http://cloud-ide.com/) 现在应该可以和 OpenShift 一起工作了。

将应用从你的 IDE 推送到一个平台的能力并不是唯一宣布的新特性。Red Hat 也在努力将构建 Java 应用程序的痛苦最小化。OpenShift 正在添加对 [Maven](https://web.archive.org/web/20230204212750/http://maven.apache.org/what-is-maven.html) 的支持，以帮助简化依赖关系解析过程，并添加对 [Jenkins](https://web.archive.org/web/20230204212750/https://wiki.jenkins-ci.org/display/JENKINS/Meet+Jenkins) 的支持，以提供“构建即服务”功能。

根据 Roth 的说法，这是一种推动，允许 Java 开发人员在“云中”做一切事情:编码、构建和扩展。Java 应用程序开发人员可以专注于他们的应用程序，而不用担心基础设施。Maven 的加入让开发人员摆脱了为他们的应用程序手动安装库依赖项，并且在某些情况下可以完全避免使用 Ant 脚本。Jenkins 支持帮助开发者快速迭代，现有的 OpenShift 平台处理可扩展性。

当我想到 Java 应用程序时，我通常会想到与企业数据库和目录服务通信的整体企业应用程序。我不会想到云应用。所以我问 Roth 和 Anderson 谁在推动 OpenShift。特别是，客户对 Red Hat 说“天哪，我希望我们可以在云中构建我们的 Java 应用程序！”他们拒绝讨论客户的具体情况，但确实分享了 Red Hat 正在通过在 OpenShift 上部署几个内容门户和 Java 移动应用后端来吃自己的狗粮。

Red Hat 在云中驱动 Java 并不完全令人惊讶。毕竟，他们拥有 [JBoss](https://web.archive.org/web/20230204212750/http://www.jboss.com/) ，当今使用的主要 Java 中间件产品之一。虽然 OpenShift 的 Java 支持目前仅限于社区驱动版本的 [JBoss AS](https://web.archive.org/web/20230204212750/http://www.jboss.org/jbossas) (就像 Fedora 对于 Red Hat Enterprise Linux 一样)，但我们或许可以期待在不太遥远的将来看到 [JBoss EAP](https://web.archive.org/web/20230204212750/http://www.jboss.com/products/platforms/application/) 支持。此外，如今市场上很少有 PaaS 产品，除了微软 Azure。大多数人似乎专注于基础设施即服务，因此向 PaaS 的转移带来了一些有趣的新机会。

OpenShift 目前是免费使用的，对应用程序的大小和可伸缩性有一些适度的限制。如果你是一个开发者，为什么不尝试一下呢？