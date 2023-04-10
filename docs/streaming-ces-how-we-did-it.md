# 流媒体消费电子展:我们是如何做到的 TechCrunch

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/01/09/streaming-ces-how-we-did-it/>

随着 2011 年[消费电子展](https://web.archive.org/web/20230202234521/http://cesweb.org/)今天落下帷幕，我们想分享一些秘密。在 [TechCrunch TV](https://web.archive.org/web/20230202234521/http://techcrunch.tv/) 的支持下， [CrunchGear](https://web.archive.org/web/20230202234521/http://www.crunchgear.com/) [写作团队](https://web.archive.org/web/20230202234521/http://www.crunchgear.com/about/)提供了超过 20 小时的现场 CES 视频报道，将我们的观众直接带到了行业和媒体专用展区。要看视频集锦，请查看[ces.crunchgear.com](https://web.archive.org/web/20230202234521/http://ces.crunchgear.com/)。数百个 Twitter 问题得到了实时回答，让我们的观众有机会与公司代表互动并赢得一些赠品。我们也收到了很多关于我们是如何做到的问题。

传统的、老派的现场直播方式包括驾驶一辆装有 C 波段或 Ku 波段发射机的卫星卡车。或者，在会场连接一个特别昂贵的视频光纤电路。但是，这将只允许从一个单一的位置视频饲料。否则，我们将需要多条线路或时间在不同地点驾驶和设置 sat 卡车。

我们希望在接到通知的瞬间，从 CES 揭幕期间的金沙博览会和接下来的媒体日，从拉斯维加斯会议中心内外，从拉斯维加斯大道各地的酒店派对和活动中进行直播。另外，我们想在没有任何有线连接的情况下在大厅里漫游。我们研究了一些 RF 和微波发射机选项，但它们涉及巨大的费用和生产限制。我们最终选定了一个移动流媒体解决方案，以及一个备用的“近乎实时”有线解决方案。我们从来不需要求助于录音备份。

我们使用了由我们的直播合作伙伴 [Ustream](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/ustream) 提供的 [LiveU](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/liveu) [移动包](https://web.archive.org/web/20230202234521/http://www.ustream.tv/production-services/mobile-package)。livepack 适合放在定制设计的背包中。它接受来自摄像机的包含视频和音频的 firewire 输入。我们使用了我们的[松下](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/panasonic) HVX200a 相机和一些无线麦克风和一个相机 LED 灯。livepack 有 6 个数据调制解调器，并试图连接到 3 个不同的移动电话网络( [ATT](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/at-t) 、[威瑞森](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/verizon)和[斯普林特](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/sprint-nextel))。信号由 LiveU 重新组合在一起，然后发送到 Ustream 进行实时流分发。

考虑到带宽问题，当 125，000 名精通技术的人聚集在一个地方时，我们有些担心这项技术是否可行。当我们尝试不成功地使用手机时，这些担忧就增加了。但是，通过它的 6 个调制解调器，livepack 能够在 95%的时间里保持连接。带宽是不断变化的。在最好的时候，我们的上行速度超过 1Mbps。在一些地方，例如 CES 媒体日期间的金沙博览中心的下层，以及少数参展商的私人会议室，我们没有足够的带宽。因此，该流有时会冻结、断断续续或变成音频。

在 livepack 上，我们选择了小的 [CIF](https://web.archive.org/web/20230202234521/http://en.wikipedia.org/wiki/Common_Intermediate_Format) 视频窗口设置。虽然牺牲了质量，但这允许更一致的流性能。Ustream 发布了一个 400k 的编码提要，窗口为 480×270，视频为 h.264。我们没有收到任何观众对视频图像质量的投诉。

电池和电池规划是关键。livepack 有一个内置电池，也可以使用热插拔外部电池。我们有大约 2 个小时的完全外部电池，并携带了许多备件。我们还有许多相机电池(不可热插拔)、无线麦克风和 LED 灯电池。

大多数时候，这个系统的运行远远超出了我们的预期。但是，我们还有另外两个非传输问题。摄像机使用 firewire 插头连接到 livepack。不是最好的，健壮的连接。即使用胶带固定，也有几次松脱，但包装上有一个监视器屏幕，提醒我们注意这个问题。

一天晚上，狼群无法启动。在美国东部时间晚上 10 点，快速拨打 LiveU 包装上的电话号码，帮助我们确认了硬件问题，很可能是电路板松动。我们刚刚带着它在繁忙的会议大厅里走了几英里。轻轻一推，livepack 又开始工作了。但是，我们还没有准备好相信它，并在那天晚上使用了一个固定位置的备用有线解决方案。但是随着又一天的报道，Ustream 连夜给我们送来了一个新的 livepack，我们在周五就开始运行了。

我们用的 LiveU livepack 已经上市一年半了。除了广播网络，流媒体视频提供商 [Ustream](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/ustream) 和 [Livestream](https://web.archive.org/web/20230202234521/http://www.crunchbase.com/company/livestream) 也在使用它。它被用于各种体育赛事和格莱美奖。一款新的高清 livepack 上周开始发货。它包含 6 到 12 个蜂窝连接(包括 T-Mobile)，支持威瑞森 LTE 4G 和 Sprint 以及 ClearWire WiMax 4G。除 FireWire 外，这些新设备还具有 SDI、HDMI 和模拟输入功能。而且他们输出标清和高清到 1080i。

即使有了第一代 livepack，我们也成功地完成了将 CES 直接带给观众的使命。我们的观众听到了几十种新的电视、手机、平板电脑、相机和耳机，以及对福特和 [T-Pain](https://web.archive.org/web/20230202234521/http://ces.crunchgear.com/2011/01/greg-talks-to-t-pain-about-the-new-i-am-t-pain-microphone/) 首席执行官[的采访。以及](https://web.archive.org/web/20230202234521/http://ces.crunchgear.com/2011/01/we-interview-alan-mulally-ceo-of-ford/) [RED Scarlet](https://web.archive.org/web/20230202234521/http://ces.crunchgear.com/2011/01/hands-on-with-the-red-scarlet-video-coming/) 、[opinion Ink Adam table t](https://web.archive.org/web/20230202234521/http://ces.crunchgear.com/2011/01/our-hands-on-with-the-notion-ink-adam-tablet/)和[微软 Surface V2](https://web.archive.org/web/20230202234521/http://ces.crunchgear.com/2011/01/hands-on-video-surface-v2-at-ces/) 的幕后预告。他们有机会看到驾驶通用的 EN-V 未来派汽车兜风是什么感觉。

他们也诚实地看待 CES，包括所有的缺点。他们看到我们在排队等候迪士尼乐园后，没有参加媒体日的三星活动。他们来到几个展位，没有人想和我们或我们的观众交谈，即使展位代表站在那里和其他大会参观者交谈。我们的观众给了我们即时的反馈，告诉我们他们在看什么，该看哪个展位，甚至在我们迷路的时候给了我们一些帮助。总而言之，相当互动，前排，视频体验。