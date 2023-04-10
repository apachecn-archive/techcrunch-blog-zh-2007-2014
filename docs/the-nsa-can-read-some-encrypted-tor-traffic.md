# 国家安全局可以读取一些加密的 Tor 流量 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2013/09/07/the-nsa-can-read-some-encrypted-tor-traffic/>

# 国家安全局可以读取一些加密的 Tor 流量

安全专家 Robert Graham 做了一些研究，并发表文章称，早期版本的“安全”Tor 协议使用的加密标准很可能是不安全的，NSA 可以读取。[绝大多数 Tor 服务器](https://web.archive.org/web/20221207113441/http://torstatus.blutmagie.de/)运行的是使用 1024 位 RSA/DH 加密的软件 2.2 版本。这与[被美国国家安全局](https://web.archive.org/web/20221207113441/https://beta.techcrunch.com/2013/09/05/nsa-subverts-most-encryption-works-with-tech-companies-for-back-door-access-report-says/)公开破解的加密标准相同，可以使用非常昂贵的定制芯片在几个小时内被颠覆。

这对你意味着什么？不多，除非你重视匿名。Tor 提供匿名浏览功能，这个功能对于活动家、记者、自由战士和其他需要避开公众视线浏览的人来说非常重要。也就是说，事实上，在其最受欢迎的化身，其加密可以(相当)容易被打破是不好的。再加上同样的标准在许多 SSL“安全”互联网交互中使用，事情就变得更糟了。简而言之，[科利·多克托罗](https://web.archive.org/web/20221207113441/http://boingboing.net/2013/09/07/90-percent-of-tor-keys-can-be.html#more-254473)写道，如果美国国家安全局能够做到这一点，那么我们可以肯定，其他不那么受欢迎的组织也拥有同样的技术。

这些工具是开源的，可以回收利用。目前用于 Tor 2.4 版本的密码对 NSA 来说比任何 1024 位密钥都要差得多，而且 Tor 式的有条不紊的加密比 NSA 式的使用暴力破解更容易。我们仍然会赢，但是需要一个村庄来保持加密的强大。