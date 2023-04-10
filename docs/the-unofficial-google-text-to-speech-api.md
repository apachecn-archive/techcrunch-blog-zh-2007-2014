# 非官方的谷歌文本到语音转换 API 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2009/12/14/the-unofficial-google-text-to-speech-api/>

# 非官方的谷歌文本到语音转换 API

上个月，谷歌[发布了谷歌翻译的](https://web.archive.org/web/20230307081839/http://googleblog.blogspot.com/2009/11/new-look-for-google-translate.html)增强功能。新功能中有一个简单的文本到语音转换功能。你可以[尝试一下](https://web.archive.org/web/20230307081839/http://translate.google.com/)，或者观看[这个视频](https://web.archive.org/web/20230307081839/http://www.youtube.com/watch?v=FijOWfO3Frk&feature=player_embedded)看看效果如何(跳到 0:45)。

文本到语音转换服务没有官方的 API。但是 Weston Ruter [注意到](https://web.archive.org/web/20230307081839/http://weston.ruter.net/projects/google-tts/)任何人都可以像 Google 一样访问该服务:*“查看 Firebug Net 面板以了解 TTS 数据的来源，我看到语音音频是 MP3 格式，并通过一个简单的 HTTP GET (REST)请求进行查询:http://translate.google.com/translate_tts?tl=en&q = text "*

翻译:只要把网址改成你想让它说的任何东西，你就会得到一个 MP3 文件。示例:复制 http://translate.google.com/translate_tts?的 URLq=I+love+techcrunch 到你的浏览器里。

这是目前唯一的英文版本，限制在 100 个字符以内。但除非谷歌关闭它，否则第三方应用程序现在可以以任何他们想要的创造性方式使用它。开始吧。

经由[阿贾西安](https://web.archive.org/web/20230307081839/http://ajaxian.com/archives/text-to-speech-via-html5-audio)。