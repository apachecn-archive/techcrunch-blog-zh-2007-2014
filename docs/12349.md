# 脸书页面行为艺术故障 chr 故意试图激活代码故障| TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2012/01/11/facebook-page-performance-art-glitchr-purposefully-tries-to-activate-code-glitches/>

# 脸书页面行为艺术故障 chr 有目的地试图激活代码故障

这个假期在硅谷的设计师中流传的是脸书粉丝页面 [Glitchr](https://web.archive.org/web/20230326025619/https://www.facebook.com/glitchr) ，它试图故意搞乱脸书代码。

虽然我之前[推测页面](https://web.archive.org/web/20230326025619/https://techcrunch.com/2012/01/09/facebug/)可能是由德高望重的前 Facebooker 用户[埃文·普里斯特利](https://web.archive.org/web/20230326025619/http://www.quora.com/Evan-Priestley)运营的，但实际上它是由某个希腊人莱莫纳斯·扎卡斯运营的。点击 Glitchr 帖子中的任何一个[链接](https://web.archive.org/web/20230326025619/https://www.facebook.com/glitchr?sk=app_249211051815180)，它们会做任何事情，从随机调出 Unicode 字符到多次加载脸书导航条。去吧，别害怕。

那么他是怎么做到的呢？嗯，Zakas 本质上是用 Unicode“绘画”,结合其非字符实体来打破布局引擎——创造了可能是社会上最模糊和最新的艺术形式。

“这些上下突出的符号是由许多发音符号组合而成的，”扎卡斯说，“你可以在那里看到它们的多样性[http://en.wikipedia.org/wiki/Diacritic](https://web.archive.org/web/20230326025619/http://en.wikipedia.org/wiki/Diacritic)。是的，这是一种艺术。有相当多的艺术家使用互联网或特定的社交网络作为他们的画布。”

Zakas 提出了 Zalgo meme 作为另一种融合 Unicode 的互联网艺术形式的例子。

当然，扎卡斯的努力在脸书遇到了朋友和敌人，那里有很多人是他的粉丝，也有一些人不是。Glitchr 的粉丝页面在去年 12 月被禁用，因为其名称中的 Unicode 字符存在问题，最终在 Zakas 联系了该页面的内部粉丝后重新恢复。

“我数过十多个来自 FB 总部的脸书员工，更不用说那些来自国际部门的员工(作为粉丝)，”他告诉我，“……他们可能喜欢 Glitchr 来检测 bug。我不知道有多少真实性，但是到目前为止，我在帖子中使用的以下错误已经被修复:在笔记中嵌入动画图片，在缩略图中共享动画图片，帖子中的文本无限扩展到右侧以及其他一些错误。”

你也可以喜欢 Glitchr，因为它看起来很酷，还因为你不太明白 Zakas 是怎么做到的。我还是有点不明白。