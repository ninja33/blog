---
layout: post
title: Antimoon 划词助手兼容模板 3.0
categories: 学习工具
description: 一种镂空句子来背单词的 Anki 模板
keywords: anki, antimoon
date: 2018-01-07 20:30:58
---

前一段时间在文章《[请找一个解释要配的上我这个单词](http://www.laohuang.net/20171213/anki-definition-word-template/)》中附带了Antimoon 模板1.0 的anki模板。因为很多同学在问，这个Antimoon模板，在划词助手里能不能用。其实模板和工具没有强制的关联要求，划词助手的选项里让你手动做字段映射，就是起到自定义的目的。

但是这也让我想到了，第一个，如果有以前用划词助手的同学，想转到这个模板来，那么最好字段名序列是兼容的。第二点要求是，在不特别指明的情况下，这个模板不会产生双面卡片(也就是不会产生definition-word所要求的拼写卡片)，最后为了避免音频媒体文件过多占用同步ankiweb个人卡片库的大小拖累同步时间，为iOS客户端和PC客户端做了跳转后欧路词典内播放音频，TTS音频，有道在线音频等三种音频播放方式。 模板预览和特色和下载链接如下 

![](/images/antimoon_3_03.jpg) 

## 字段兼容原划词助手模板

- 单词 : expression [原划词助手字段]
- 音标 : reading [原划词助手字段]
- 释义 : glossary [原划词助手字段]
- 句子 : sentence [原划词助手字段]
- 笔记 : note [原划词助手字段]
- 网址 : url [原划词助手字段\]
- 音频 : audio [原划词助手字段\]
- 柯林斯: collins [Antimoon新增字段\]
- Vocab : vocab [Antimoon新增字段\]
- Antimoon标志：add-dw [Antimoon新增字段]

注:请原来下载使用过chrome划词助手，安卓划词助手和iOS workflow划词助手的同学注意字段名对应 

## 自动产生单面或双面卡

- add-dw 字段为空，不可以有任何值，0也不可以，则产生单面word-definition卡片 （相当于原划词助手的单面卡）
- add-dw 字段非空，比如设置数字1，则产生双面word-definition/definition-word卡片 （相当于Antimoon的双面卡）

## 平台自适应三合一发音

- 如果下载过本地音频在audio字段，则audio字段显示发音按钮，点击发音按钮播放audio字段内的音频 
  注:[电脑端需安装插件 [#498789867(replay button on card)](https://ankiweb.net/shared/info/498789867) 才能显示发音按钮]
- 如果没有下载过本地在audio字段，则点击单词本身，模板会根据选项isTTS的取值，决定是TTS发音，还是在线音频发音
- 全局变量isTTS在模板的style(样式区)寻找，isTTS=false 有道在线发音；isTTS=true (iOS only)TTS发音

## 其他改变及新增特色

- 模板会根据iPhone还是iPad的屏幕大小进行字体大小设置 （iOS only: iPhone字体18点，iPad字体28点）
- 学习新单词用的word-definition 卡片会显示vocabulary.com的短解释和长解释
- 而复习旧单词拼写用的definition-word卡片仅显示vocabulary.com的短解释
- (Antimoon)definition-word卡片的正面，句中单词镂空，在原处以黑点替代。
- (Antimoon)definition-word卡片的反面，句中单词恢复原样，便于阅读理解。

## 下载链接

链接：[Antimoon.3.0](/files/Antimoon.3.0.zip) 

（2018/01/26更新）增加用于wordquery插件的collins和vocab mdx文件下载： 

链接：[https://pan.baidu.com/s/1pMZX0AB](https://pan.baidu.com/s/1pMZX0AB) 密码：23Pi