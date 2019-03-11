---
title: iOS Workflow 划词制卡助手
tags:
  - anki
categories:
  - 学习工具
date: 2017-03-11 02:16:26
---

_==== 2017年12月更新 ====_ 
注：本文完成以后，因ankimobile(anki的iOS版)从2.0.30版开始已经支持URL Schema直接在手机上制卡，所以下文中dropbox和ankiconnect的方式虽然任然可用，但都没有iOS原生URL Schema的方式来的方便快捷。 

【最新视频教程】 [iOS版Anki(带URL schema功能) workflow 划词制卡助手介绍](https://www.bilibili.com/video/av16814975/) 

【模块下载地址】 
[iOS划词助手主程序](https://workflow.is/workflows/37318527846b492598d312f3d0dddcc4) 
[词典模块](https://workflow.is/workflows/28cf38495f6b432c9ed4ee7271625103) 

【本教程用的划词原句模板】 
[划词原句模板下载链接](/files/划词原句模板.zip) 

_==== 2017年3月原文 ====_

#### 划词制卡助手 for iOS

在之前的文章《[Chrome Anki 划词制卡助手 使用说明(含视频教程)](http://www.laohuang.net/20160817/anki-dict-helper-chrome-extension/)》里所提到的插件工具，只能在电脑端使用。而我们大部分的碎片时间可能在路上，在等电梯的时候，在地铁里。我们的阅读工具，可能是手机。所以，一直在想，怎么在自己的手机上也实现划词助手，一键制卡的功能。
<!-- more -->
因为iOS应用的权限限制，一直没找到好的办法。直到最近看见少数派作者JailBreakHum的一篇有关iOS workflow的教程《[Workflow 教程（八）：利用新的请求方法打造 Web 小程序](https://sspai.com/post/35857#03)》，其中有讲到怎么将单词存放到扇贝网。这让我找到了思路：本地存储和应用间通讯不行，那可以在存到网络盘再导入嘛。同时，iOS workflow的强大功能，使取词，翻译，网络存储，都成为了可能。大概的思路如下：

1.  从新闻应用或者浏览器中选中句子，或者直接分享到workflow，或者复制到剪贴板，然后从通知中心启动workflow 脚本。
2.  在脚本中，用正则表达式将句子打散成单词，然后提示用户选中要翻译制卡的单词（相当于划词了，只不过选的是句子）
3.  将选中的单词，通过网络API，翻译后获得音标，解释，并将上下文例句做简单处理。
4.  通过调用dropbox API(workflow现成模块)，或者Ankiconnect(Anki插件)，或者扇贝单词API，将制卡信息存入相应的目的端。
5.  通过Anki电脑端的文本文件导入功能，或者扇贝单词的客户端，进一步学习含上下文例句的情景化单词，印象深刻，有助于记忆。 
![](/images/iOS_workflow_screen.jpg)

#### iOS workflow 视频教程

1.  演示视频： [iOS workflow 划词制卡助手演示](http://www.bilibili.com/video/av9291591/)
2.  制作简介： [iOS workflow 划词制卡助手制作简介](http://www.bilibili.com/video/av9291708/)

#### iOS workflow 工作流

考虑到单词查询模块和制卡目的端的课替换性。将iOS workflow的脚本做成了可层级调用的子脚本。以方便将来的替换。 ![](/images/iOS-workflow-dict-helper.jpg)

#### iOS workflow 脚本下载

请先装好workflow，然后用iOS浏览器Safari打开下面附件中的链接。 链接：[http://pan.baidu.com/s/1jHRqfsE](http://pan.baidu.com/s/1jHRqfsE) 密码：wbim 另外，扇贝网token的获取方式，详见少数派作者JailBreakHum的文章《Workflow 教程（八）：利用新的请求方法打造 Web 小程序》