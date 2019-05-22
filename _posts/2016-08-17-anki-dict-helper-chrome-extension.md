---
layout: post
title: Anki 划词制卡助手
categories: 学习工具
description: Chrome 插件划词助手网页工具
keywords: anki, extension
date: 2016-08-17 01:21:43
---

[2019年2月更新]：Anki划词助手目前已经停止更新，想用浏览器配合anki划词的同学，可以关注作者的另一款插件《[在线词典助手](https://www.laohuang.net/20180213/online-dictionary-helper/)》，同时支持Chrome和Firefox版本，对于原句的摘取，词组的识别更好更准确

- 谷歌版下载地址：[谷歌商店](https://chrome.google.com/webstore/detail/online-dictionary-helper/lppjdajkacanlmpbbcdkccjkdbpllajb?hl=en)

- 火狐版下载地址：[火狐商店](https://addons.mozilla.org/en-US/firefox/addon/online-dictionary-helper/)


- 离线版下载地址：[老黄老巢](https://www.laohuang.net/20190523/odh-offline-package/)

---

英语学习者在新闻网站或者社交媒体上进行增量阅读(Incremental Reading)或者沉浸式阅读(Immersion Reading)时，往往需要能够随手翻译生词帮助理解，而阅读过后，又希望能将刚才阅读时遇到的生词和上下文语句作为笔记保存，以供日后复习。

Anki本身提供了不错的间隔式复习功能，但是制卡的过程略微繁琐。Anki划词制卡助手，就是为了帮助学习者在阅读的同时，将生词，释义，音标，语音音频和上下文例句一键保存并制作成Anki卡片，以供日后复习。 下面按步骤列出了Anki划词制卡助手的安装过程。

## 安装插件

- 安装ankiconnect 插件，然后重启Anki。 ankiconnect下载地址和安装方法详见另一片文章: [《Anki划词制卡助手》配套AnkiConnect.py文件](http://www.laohuang.net/20160817/ankiconnect-py-file/)

- 安装Chrome插件 [Anki划词制卡助手](https://chrome.google.com/webstore/detail/anki%E5%88%92%E8%AF%8D%E5%88%B6%E5%8D%A1%E5%8A%A9%E6%89%8B/ajencmdaamfnkgilhpgkepfhfgjfplnn?hl=zh-CN)，按Chrome浏览器提示安装。

## 选项设置

第一次使用时需要正确设置chrome插件才能和Anki连接.

- 首先请确保Anki PC客户端已经打开，并按上述步骤1完成anki connect插件的安装
-点击“启用Ankiconnect选项”

![](/images/anki-dict-helper-01.jpg)

- 正确选择牌组名称和模板名称，并做好区域标签的映射

![](/images/anki-dict-helper-02.jpg)

- 区域映射：就是定义Anki connect制卡时自动对应的卡片区域（字段），下图定义了单词，音标，释义和例句四个区域。

![](/images/anki-dict-helper-03.jpg)

- 可选区域标签，有如下图这8类选择，填入时请务必注意带两边的花括号：

![](/images/anki-dict-helper-04.jpg)

## 使用方法

- 在浏览需要翻译的英语网站时，将鼠标移动到英语单词处，按住Shift即可获取实时翻译。
- 按发音按钮(小喇叭图标)，可以听取单词发音。
- 按绿色加号按钮，将单词，词语，翻译的中文释义，单词在网页中所在句子（上下文），网址，和音频，按照之前设置的区域映射关系，自动在Anki 

PC端生成一张卡片。

![](/images/anki-dict-helper-05.jpg)

最后在Anki中自动生成的卡片，如下图所示。可见在选项里定义的四个字段，已经完全自动获取并填入相应区域。

![](/images/anki-dict-helper-06.jpg)

## 视频教程

[优酷视频:Anki划词制卡助手教程](http://v.youku.com/v_show/id_XMTgzMDgxODQ2NA==.html)  

## 模板下载

[划词原句模板](/files/ODH.zip)