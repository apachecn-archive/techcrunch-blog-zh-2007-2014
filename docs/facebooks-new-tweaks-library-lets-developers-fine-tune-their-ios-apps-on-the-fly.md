# 脸书新的“调整”库让开发者可以随时调整他们的 iOS 应用程序 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/03/25/facebooks-new-tweaks-library-lets-developers-fine-tune-their-ios-apps-on-the-fly/>

假设您正在构建一个 iOS 应用程序。

你的 iOS 应用程序有许多小动画，你(或你的设计师)希望这些动画的时间安排恰到好处。这种奇特的扩展抽屉效果应该持续半秒钟，还是四分之三秒钟？

通常情况下，开发者会猜测合适的时机，编译他们的应用程序，测试，修改，重新编译，清洗，涂肥皂，重复。鉴于复杂的应用程序可能需要相当长的时间来编译，这些小变化开始吞噬你的时间。你开始讨厌进度条。

这么简单的东西为什么要重新编译？如果完善时间的人更多的是一个设计师而不是一个程序员呢？他们应该为了改变动画速度而挖掘源代码吗？

当然有各种各样的捷径。例如，你可以将动画速度的变量绑定到屏幕上的滑块，任何运行你的应用程序预发布版本的用户都可以动态调整它——但你必须手动编码，并记住在发布前将其取出。这是一个完全有效的选择——但是它不是非常标准化，并且您希望能够即时更改的每一件事情都意味着额外的代码行。可能会更好。

脸书认为他们做得更好。

他们刚刚发布了一个名为“Tweaks”的库，让开发人员可以轻松地标记某些东西，如动画的时间，按钮的颜色，或图像的透明度，一旦应用程序在设备上实际运行，这些东西就可以随时改变。该库将所有这些可调整的变量塞进一个时髦的小隐藏设置屏幕，然后在实际发布应用程序时将其全部清理干净。

**正如脸书所说:** 

> 提高一个 app 最好的方法就是每天使用。即使想法可以提前测试出来，例如折纸，它仍然需要一些时间来观察应用程序在实践中的效果。
> 
> 偶尔，第一次尝试是完美的。有时候，这个想法根本行不通。但通常，它只需要一些小的调整。最后一种情况正是 Tweaks 适合的地方。Tweaks 使这些小的调整变得容易:无需修改代码和计算机，您可以尝试不同的选项并决定哪一个效果最好。

当应用程序在调试模式下编译时，摇动手机会弹出一个屏幕，允许用户修改开发者暴露的任何设置。当它被编译成正常的“发布”模式时(例如，当它为 App Store 做准备时)，“Tweak”值被一个正常的、不可更改的值所取代，隐藏的配置屏幕永远消失了。需要添加的额外代码很少，需要删除的代码也很少。

开发人员必须在代码中做出的唯一真正的改变是:他们将值设置为“调整”，而不是硬编码值。在代码中，代替:

> CGFloat 动画持续时间= 0.5

你会用:

> CG float animation Duration = FB tweak value(@“类别”，@“组”，@“持续时间”，0.5)；

那么这有什么意义呢？

对于开发人员来说，这意味着能够用更少的代码更快地微调应用程序。作为一个额外的好处，它可以让任何不喜欢编码的设计人员帮助找出最佳设置，而不必进入源代码或纠缠开发团队进行一百万次新的构建。大家都赢了！万岁！

脸书已经在 GitHub 上发布了调整(在一个相当非限制性的 BSD 许可下免费)[就在这里](https://web.archive.org/web/20221225042845/https://github.com/facebook/Tweaks)。