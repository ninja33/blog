---
title: Anki划词助手内置词典介绍
categories:
  - 学习工具
date: 2018-01-08 21:42:08
tags:
---

有同学问起划词助手的词典格式，记得以前写过一个，放这里存档
使用Chrome商店版本的划词助手时，内置词典是无法替换的，这在作者制作插件时，已经预先打包了。如果想使用自定义的内置词典，那么必须使用开发者版本。 如何下载Chrome插件的crx文件，并加载Chrome插件的开发者版本，这个请自行去网上查询。在开发者版本中，内置词典文件存放于 插件根目录\\bg\\data\\edict.json. 
![](/images/edict-location.png) 只要制作出符合格式的edict.json文件并同名替换原文件，就可以起到更换词典的作用。从文件名可以看到，该词典文件采用了JavaScript的JSON格式，这是因为Chrome和Firefox的插件本身就是JavaScript的脚本，词典文件采用JSON格式，更便于JavaScript脚本读取和处理。 附件是完整的词典格式说明，有需要的同学和开发者可以用以参照和二次开发。 

[Anki划词助手词典格式](/files/edict-json-format.zip)