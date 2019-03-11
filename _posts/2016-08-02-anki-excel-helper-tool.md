---
layout: post
title: Excel 批量制卡
categories: 学习工具
description: 利用Excel批量制作Anki卡片
keywords: excel, anki
date: 2016-08-02 00:31:03
---

（2018年更新）因为有Anki原生批量制卡插件WordQuery的出现，所以原来Excel批量制卡的方式已不再那么方便(需要另存为TXT再导入Anki)，下面是更新后的WordQuery批量制卡视频教程。 

- WordQuery视频教程：[背单词软件Anki之强力插件WordQuery的使用方法介绍](https://www.bilibili.com/video/av16816801/)

（2016年8月原文）该制卡工具由Excel VBA写成，主要用于批量制作anki英语单词类的卡片。

![](/images/anki-excel-tool-001.jpg)

## 制卡工具离线查询

将单词贴入”查询表格”A7开始的A列，后续各列会从离线词典中查出解释。(200行公式不够，请往下拖) 目前工具自带三本离线词典，分别是：

1. 牛津简明英汉词典：音标+简明中文解释。(2字段)(14万词条)
2. Vocabulary.com英英词典：简明+扩展，英英情景化解释。(2字段)(1万7千词条)
3. Collins五星分级双解词典: 五星分级+双解中文解释+例句。(2字段)(3万9千词条)

## 制卡工具在线查询

点击“在线词典”附加选项，唤出在线词典按钮，选择词典后，按”在线查询”按钮查询。 目前工具自带两本在线词典，分别是： a. 有道在线英汉词典：英美音标+中文解释+英语例句+中文例句。(4字段) b. 海词在线英汉词典：英美音标+中文解释+英语例句+中文例句。(4字段) 制卡工具输出结果 待查询完毕后，按”生成文件”按钮，产生文本文件，用于anki导入。 导入anki时以tab(\t)分隔，HTML格式导入。可配合zip包中附带的模板使用。 如需再次查询，可按”清空结果”后，从上述第1项开始重复查询步骤。 

![](/images/anki-excel-tool-002.jpg)

## 制卡工具注意事项

仅在Win7/MS Office 2013/IE9 以上版本测试运行通过。Mac和WPS未经测试。 请将zip包中的x64, sqlite3.dll, sqlite3_stdcall.dll等文件放在excel所处同一目录。 制卡工具视频解说 (从视频72分钟开始是制卡工具教程，之前部分是基础制卡教程。) 

[优酷视频:Anki手工及批量制卡教程](http://v.youku.com/v_show/id_XMTgyNjQxNDkxMg==.html)

## 制卡工具文件下载

链接：[http://pan.baidu.com/s/1miQMssw](http://pan.baidu.com/s/1miQMssw) 密码：kx0a