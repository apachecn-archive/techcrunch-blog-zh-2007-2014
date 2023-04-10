# 明年的头条:微软未能在 Powerset TechCrunch 上做任何有意义的事情

> 原文：<https://web.archive.org/web/https://techcrunch.com/2008/07/18/next-years-headline-microsoft-fails-to-do-anything-significant-with-powerset/>

# 明年的头条:微软未能在 Powerset 上做任何有意义的事情

有一个明显的细节，每个报道微软收购 Powerset 的人都没有提到:Powerset 是一家基于 Unix 的公司。它的所有核心组件——它的应用程序、打包系统和持续集成系统——都是为在 Unix 平台上运行而设计和编写的。

作为一家大型软件公司，微软非常支持自己的工艺。不出所料，微软的所有产品，包括 Live search，都运行在 Windows 服务器上。因此，我们来到了微软-Powerset 矛盾的根源。虽然把软件从 Unix 移植到 Windows 并非不可能，但不可否认，这是一项地狱般的任务。Powerset 在过去的三年中开发了一个大型的代码库，自然地，它选择了在其开发栈中使用许多开源项目，这些项目都必须进行移植。它使用的大部分软件已经是跨平台的，但是那些不是真正的问题。

当 Powerset 推出时，开发者凯文·克拉克[对 Powerset 所依赖的开源技术大声疾呼](https://web.archive.org/web/20230204060554/http://glu.ttono.us/articles/2008/05/12/holy-god-powerset-launches)。下面给出了这些技术与 Windows 兼容性的状态。

【Powerset 使用的开源技术的 Windows 兼容性

| **Hadoop/Hbase** | 要求 Cgywin 在 Windows 上运行。 |
| **红宝石** | 在 Windows 上运行缓慢，这是微软使用 IronRuby 的好机会？ |
| **Ruby on Rails** | 将在 Ruby 运行的任何地方运行。IronRuby [最近达到了 Rails 奇点](https://web.archive.org/web/20230204060554/http://www.iunknown.com/2008/05/ironruby-and-rails.html)。 |
| **Merb** | 与 Rails 的情况相同。目前还没有关于 IronRuby 功能的消息。 |
| **上帝** | 不在 Windows 期间运行。也没有计划 Windows 支持。然而，[写上帝](https://web.archive.org/web/20230204060554/http://rubyisawesome.com/)的好撒玛利亚人恰好为 Powerset 工作。也许他们可以求他做一个 Windows 版本。 |
| **杂种狗** | 在 Windows 上完全支持。 |
| Mootools | JavaScript——他们的战斗是在浏览器而不是操作系统。 |
| **二郎** | 良好的 Windows 支持！ |
| **雅司病** | 基于 Erlang，也适用于 Windows。 |
| **Memcached** | 有一个非官方的 Windows 端口，不应该在生产环境中使用。 |

总而言之，任何需要 Cgywin 的东西都无法在像 Live.com 这样的高流量生产环境中运行。Windows 上的官方 Ruby 解释器太慢，而 IronRuby 太新，没有经过充分的现场测试，无法支持微软的搜索。使用上帝不是一个选项，所以他们将不得不寻找一些其他的方法来管理他们在 Windows 上的进程。替换 Memcached 并不困难。最后，Erlang 在 Windows 上的地位似乎不错，但转型仍将是艰难的。

如果微软想利用 Powerset 的现有 IP，让 Ruby 进入最佳状态是很重要的。根据 Ruby on Rails 播客上的[采访](https://web.archive.org/web/20230204060554/http://podcast.rubyonrails.org/programs/1/episodes/github-and-powerset)，“组织的所有部分都使用 Ruby”。包括他们开发的所有自然语言解析和至少 60%的内部工具。

最有可能的情况是，微软将放弃 Powerset 的大部分代码，并将移植核心技术和实现 Windows Live 搜索的必要捆绑的任务交给团队——Powerset 工程师可能会愤愤不平地接受这项任务，这取决于他们认为哪个平台更优越。Powerset 的核心实际上是语义搜索技术，它是从 PARC 学来的，并在此基础上进行了扩展。换句话说，微软确实想要 PARC 的技术，但它买下了 Powerset [【为了他们的人民】](https://web.archive.org/web/20230204060554/http://blogs.msdn.com/livesearch/archive/2008/07/01/powerset-joins-live-search.aspx)，因为 Powerset 的工程师是唯一真正了解 PARC 东西的人。

微软声称 Powerset 的语义搜索将在年底出现在 Live search 中，这是微软向其股东广播的胡言乱语，以帮助证明他们 1 亿美元的收购是合理的。切换到 Windows 平台不是一件小事，而[切换到一个不熟悉的封闭平台放大了复杂性](https://web.archive.org/web/20230204060554/http://www.techcrunchit.com/2008/07/16/google-where-companies-go-to-die/)。然而，有传言说微软在内部运行一些 BSD 服务器，在这种情况下，Powerset 集成实际上是可能的。最终，这次收购感觉像是微软的一次研发实验。语义搜索仍然是计算机科学的一个灰色地带，微软正在通过收购 Powerset 来碰运气。