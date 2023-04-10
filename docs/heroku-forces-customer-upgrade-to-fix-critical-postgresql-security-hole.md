# Heroku 迫使客户升级以修复关键的 PostgreSQL 安全漏洞

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/04/01/heroku-forces-customer-upgrade-to-fix-critical-postgresql-security-hole/>

# Heroku 强迫客户升级以修复严重的 PostgreSQL 安全漏洞

Heroku 客户将首次获得 PostgreSQL 数据库系统的关键更新，该更新将修补一个主要的安全漏洞。整个 PostgreSQL 社区将在周四获得更新。

以下是 Heroku 的声明:

> Heroku Postgres 数据库将在今天星期一(4 月 1 日)到星期三(4 月 3 日)之间进行一次简短但重要的更新。在更新过程中，您的数据库将脱机大约 60 秒，然后将重新启动。由于此更新的性质，计划的时间是不可能的。对于需要维护的数据库，不会单独发送通知。

上周四，PostgreSQL 网站发布了一份[声明](https://web.archive.org/web/20230326030253/http://www.postgresql.org/about/news/1454/)，称将于 4 月 4 日发布更新，包括对一个高暴露安全漏洞的修复。他们强烈要求客户在更新可用时立即应用。

还没有回复，但是我已经询问了 Heroku 的公共关系团队，询问他们为什么要进行强制更新，以及他们为什么要首先访问。

黑客新闻评论者说，早期访问可能是由于大量 Heroku 客户使用 PostgreSQL 数据库。

这种特权也引发了关于 PostgreSQL 安全策略的问题，以及谁可以提前访问，谁不能。

一位黑客新闻评论者说:

> 与此同时，他们对其他许多同样非常重视安全的公司的安全修补程序进行了限制。这就造成了这样一种情况，即考虑 posgresql 的公司现在必须问“我是应该在安全补丁准备好的时候马上得到它们，还是应该故意让我处于易受攻击的状态，而让更多的特权用户提前访问？”在我看来，这不是一个好的先例。

这是 Heroku 的一个不寻常的举动，也是云安全是一个重大问题的一个突出例子。像 Heroku 这样的公司很少发布这些强制更新。最常见的是对平台进行重大更新。但是像这样的安全漏洞可能会对整个平台产生影响。