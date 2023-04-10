# 通过声波传输文件 TechCrunch

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/04/24/file-transfers-via-soundwave/>

# 通过声波传输文件

![soundwave file transfer](img/fdee36c5ced6a9007918d4095dac7cb9.png "soundwave file transfer")
还记得调制解调器吗？不，不是电缆调制解调器或 DSL 调制解调器，它们在技术上更像是网桥。我说的是真正的、真正的模拟*调制解调器*，那种确实会发出噪音的那种。如果你在上网的时候拿起电话的话！，你会听到刺耳的尖叫声，你正在下载的萨曼莎·福克斯的裸照会被毁掉！Modem 代表“调制/解调”，这个名称很好地描述了调制解调器的工作原理:发送方调制解调器将数据调制成声音，以便通过电话传输，接收方调制解调器将声音解调回数据。你猜怎么着:你可以用同样的原理在 pc 机之间传输文件，只需要一个声卡和一些巧妙的编程。

维克多·洛夫格伦详细描述了[如何使用声卡传输文件](https://web.archive.org/web/20230203003144/http://awesomegeekblog.blogspot.com/2009/04/file-transfer-over-sound-card.html)。不过，洛夫格伦先生给你提个醒:

> 千万不要戴着耳机尝试这些程序。他们制造很大的噪音！有可能配置这些程序使噪音比你想象的耳机能发出的声音大得多。播放音频节目可能会损害您的听力。耳鸣可不好玩。

基本上，这是你如何通过声波发送文件:

> 对于每个字符:
> 对于每个位:
> 如果该位为 1，发送一个短脉冲。
> 如果该位为 0，则发送一个长脉冲。
> 寄沉默。
> 发送很长的脉冲(是最短脉冲的 4 倍)。
> 送一份沉默。

产生声音并通过扬声器发出来很容易。通过连接到另一台计算机上的麦克风接收和解释声音要稍微困难一些。阅读[整篇](https://web.archive.org/web/20230203003144/http://awesomegeekblog.blogspot.com/2009/04/file-transfer-over-sound-card.html)了解详情，一定要给 Lofgren 先生一些作为聪明极客的道具！