# 在即将到来的 HTML5 浏览器大战中，标记应该保持不变

> 原文：<https://web.archive.org/web/https://techcrunch.com/2010/09/02/html5-browser-wars/>

![](img/f909b688aef43a3bd197afa9b2a20060.png)

周一，谷歌通过定制的 [Arcade Fire 视频页面](https://web.archive.org/web/20221206215757/http://www.chromeexperiments.com/arcadefire/)引起了[的巨大轰动](https://web.archive.org/web/20221206215757/https://beta.techcrunch.com/2010/08/30/google-chrome-html5-arcade-fire/)，展示了 HTML5 可以做的所有很酷的事情，从视频、动画和 3D 渲染到华丽的字体和精心设计的窗口。就网络浏览器而言，这都是最前沿的东西，但有一个非常大的问题。它并不是在所有的浏览器中都能很好地工作，即使是那些据称支持 HTML5 的浏览器。如果你在 Firefox 甚至即将发布的 IE9(尚未发布，但对 HTML5 非常友好)中打开视频的[登陆页面](https://web.archive.org/web/20221206215757/http://www.thewildernessdowntown.com/)，它会检测你的浏览器并建议你使用 Chrome。我在 Firefox 上收到了以下消息:

> 该网站设计时考虑到了谷歌浏览器，因此无法在您的浏览器中正常显示。为了获得最佳观看体验，我们建议下载 Google Chrome 并再次尝试该网站。

但是等等，火狐不就是那些[支持 HTML5](https://web.archive.org/web/20221206215757/https://beta.techcrunch.com/2009/06/09/demo-firefox-35-treats-videos-like-web-pages-why-cant-flash-do-that/) 的“现代浏览器”之一吗？这不是第一次出现 HTML5 兼容性的问题。问题是 HTML5 太年轻了，标准还没有在所有浏览器中形成。对于不同的浏览器，产生相同效果所需的标记语言是不同的。

“拱廊之火的事情。。。他们在给浏览器写信，”微软负责 Internet Explorer 的总经理迪安·哈查莫维奇指出。"他们使用专有的 Javascript . "他认为 HTML5“做得好”，将会在不同的浏览器中使用相同的标记语言。似乎很合理。这就是开放网络的意义所在。这就是为什么我们有标准。但是 HTML5 太新了，以至于我们回想起 20 世纪 90 年代末，网站拒绝接受某些浏览器。

为了说明这一点，微软有一个[浏览器测试页面](https://web.archive.org/web/20221206215757/http://ie.microsoft.com/testdrive/Default.html)来展示不同浏览器之间的区别。在一组名为 HTML5 Demos 的测试中，有一个“[边框半径”测试](https://web.archive.org/web/20221206215757/http://ie.microsoft.com/testdrive/HTML5/01BorderRadius/Default.html)，可以改变文本块周围的边框。在文本块内部，它显示了创建不同效果所需的标记代码，如动画或创建点而不是实线。(**更新**:正如评论中指出的，这在技术上是 CSS3，和 HTML5 不完全一样，但两者齐头并进)。下面是代码在 Chrome 中的样子:

![](img/02ca8794e8ca64e9ed591ed69c8b9b08.png)

这是它在 Firefox 中的样子

![](img/867645e26354940573b79bed819f86e5.png)

这些图片有什么问题？一个要 16 行代码，一个要 4 行，完全不一样。甚至创建的点也不匹配(Chrome 的点是方形的)。IE9 需要一组不同的代码。“我们想让同样的标记在任何地方都能工作，”哈查莫维奇说。“如果你必须为每个浏览器编写不同的代码，那就有点跑题了。”

微软正在与标准机构合作，所有其他浏览器制造商也是如此，但真正需要的是更好的定义和每种可能的 HTML5 功能的完整参考示例集。工作量很大。最终，我们会到达那里。但在那之前，期待看到哗众取宠的关于哪个浏览器做 HTML5 更好。当你听到这些，问问你自己，他们说的是哪个版本的 HTML5。

**更新**:正如很多读者在评论中指出的，上面的 Radius 边框例子在技术上并不是 HTML5。就是 [CSS3](https://web.archive.org/web/20221206215757/http://en.wikipedia.org/wiki/Cascading_Style_Sheets) (层叠样式表)。然而，这是一项相关的技术。微软将它列在 HTML5 演示[下面](https://web.archive.org/web/20221206215757/http://ie.microsoft.com/testdrive/Default.html)(尽管它在实际演示页面上正确地将其识别为 CSS3)，苹果将其作为相关的现代网络标准包含在其 [HTML5 展示中](https://web.archive.org/web/20221206215757/http://www.apple.com/html5/)，谷歌将其包含在其 [HTML5 工作室](https://web.archive.org/web/20221206215757/http://studio.html5rocks.com/)(“展示 HTML5、CSS3 和朋友们的一些奇特方面的九个演示”)。虽然 CSS3 是一种不同于 HTML5 的规范，但它是现代 Web 技术家族的一部分，应该可以在所有浏览器中工作。

CSS3 边框半径测试是一个很好的例子，因为它直观地展示了非常简单的事情需要不同的标记。HTML5 通常也是如此:相同的标记不会产生相同的结果，要获得相同的结果，需要编写不同的标记。

这是更大的问题。正如 Mozilla 的 Christopher Blizzard 在一篇启发性的文章中所说的那样，当时苹果的 HTML5 Showcase 只支持 Safari:

> HTML5 最重要的方面不是像视频和画布这样的新东西(Safari 和 Firefox 都已经推出多年了),而是真正的互操作性承诺。即使是古板的老微软，近十年来一直竭尽全力阻止网络发展，也明白这一点，你会在他们的 IE9 营销中看到这一点。(他们的营销用语是“相同的标记”——留意它，你会在他们的信息中随处可见。)相同的标记，即使有错误，也会被完全相同地呈现。HTML5 代表了浏览器一起工作并找到共同点的机会。

同样的道理也适用于 CSS3、Javascript 和其他任何东西。