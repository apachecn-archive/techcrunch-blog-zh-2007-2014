# Cane 2.0:默契是为视力受损者设计的手持式声纳 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/08/19/cane-2-0-the-tacit-is-hand-mounted-sonar-for-the-vision-impaired/>

每隔一段时间，你就会看到一项似乎姗姗来迟的发明。默契的 T1 就是其中之一，它是一个手持系统，可以探测周围环境并向用户传输距离信息。虽然可靠的白色拐杖和为盲人和视力受损者提供的临时住宿改善了在没有视觉的世界中导航的困难，但既有用又随时可以部署的技术进步却少之又少。

我们已经看到了很多关于[人工视觉系统](https://web.archive.org/web/20230205043951/https://techcrunch.com/2010/04/02/and-now-the-aussies-are-making-bionic-eyes-too/)的研究，而且经常有一些由个人关注视觉或行动能力等问题的人拼凑的项目——我们已经看到了 [Kinect 驱动的导航系统](https://web.archive.org/web/20230205043951/https://techcrunch.com/2011/03/16/kinect-hack-head-mounted-kinect-makes-for-rudimentary-artificial-vision/)、 [Eyewriter](https://web.archive.org/web/20230205043951/https://techcrunch.com/2010/12/13/video-eyewriter-2-0-eye-tracking-hardware/) 和 Ken Yankelvitz 的[截瘫无障碍控制器](https://web.archive.org/web/20230205043951/https://techcrunch.com/2011/06/14/engineer-has-been-helping-paraplegic-gamers-play-using-modified-controllers-for-30-years/)。这个项目是一个惊人的例子，说明一个人可以用烙铁、一些现成的零件和一个有创造力的头脑做什么。

[维梅奥·http://www.vimeo.com/27675622 w = 640 & h = 360]

该系统使用两个[超声波传感器](https://web.archive.org/web/20230205043951/http://www.parallax.com/tabid/768/ProductID/92/Default.aspx)，可以探测 2 厘米到 3 米之间的物体距离。面向左右安装，它们可以扫过一个房间，并能够感知最常见的障碍和危险物体。他们通过一个 [Arduino 迷你控制器](https://web.archive.org/web/20230205043951/http://www.sparkfun.com/products/9218)发送信号，该控制器控制一对伺服系统。这些伺服系统都在手腕上压下一圈泡沫:物体越近，它们压得越紧。整个装置由一个 9V 电池供电，可以绑在任何一只手上。

像这样的设计是我们拥有专利系统的原因。虽然科技公司正在为琐碎的 UI 项目和软件方法申请数千项专利，但发明者史蒂夫·霍弗(Steve Hoefer)却选择在知识共享许可下免费赠送他的发明。像这种有趣的黑客发明越来越常见，他已经[公布了零件清单](https://web.archive.org/web/20230205043951/http://grathio.com/2011/08/meet-the-tacit-project-its-sonar-for-the-blind/)，详细说明，电路图和 Arduino 控制器的源代码。

![](img/f3160a9eae9614f4766b5bce1e7f17f7.png "tacit_haptic_glove_electronics")

Hoefer 说这个系统有一个“秒”的学习曲线，我看不出为什么不应该是这样。没有什么是天生的直觉；一切都是学来的，甚至视觉和我们对空间和导航的概念。基于手的触觉反馈是许多盲人伴随着成长起来的，增加这种额外的信息，虽然起初是陌生的，但可能会受到欢迎，因为非常有益。他们也证明了自己非常有能力将这类信息综合成一个有凝聚力的心智地图——有时令人难以置信。

还有一些其他的触觉视觉项目，如[光环](https://web.archive.org/web/20230205043951/http://www.instructables.com/id/Haptic-Feedback-device-for-the-Visually-Impaired/)系统——但这对我来说似乎更实用。手的扫动模拟了眼睛的路径，与头戴式系统不同，这种系统可以用来在桌子上定位一支笔。由于成本如此之低，它可以很容易地制造并成为一种普通的援助物品，不像视觉替代这样迷人但昂贵且不切实际的想法。

看到真正的发明家发明真正的东西总是令人振奋的，不为别的，只为一个需要解决的问题。

[via [黑一天](https://web.archive.org/web/20230205043951/http://hackaday.com/2011/08/19/the-hand-mounted-haptic-feedback-sonar-obstacle-avoidance-asstance-device-or-the-tacit)