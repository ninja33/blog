---
layout: post
title: AwesomeTTS (MDX Server版)
categories: 学习工具
description: 定制化的Anki插件AwesomeTTS插件
keywords: awesometts, anki
date: 2016-11-13 01:58:04
---

（2018年11月补充说明）很多同学会用awesometts配合mdx server来导入朗文真人发音。那么现在导入朗文音频的话，可以用fastwq这个anki插件。直接就把朗文音频导入了，也不用装mdx server，也不用装awesometts，一个插件就搞定了。速度还很快。mdx server这个方法很老了，大家可以尝试一下新方法 插件地址：[https://ankiweb.net/shared/info/1807206748](https://ankiweb.net/shared/info/1807206748)

## 使用说明

Anki用户在使用AwesomeTTS插件时，一般有两种选择：

- 一种是百度有道等国内服务商，速度快但发音质量一般。
- 另一种是选取Oxford, Collins等英英词典发音，但服务器在海外音频下载慢。

MDX Server通过读取词典文件，对外部提供标准的HTTP服务，为AwesomeTTS提供了音频下载接口。 现将AwesomeTTS修改，适配LDOCE6朗文英英词典，配合MDX Server，实现了朗文6单词音频的下载。使用方法如下：

## 运行MDX Server并选取朗文英英词典

- 将mdx-server.zip文件解压至任意目录后，点击运行mdx-server.exe(出于安全性考虑，不再直接提供exe可执行文件，目前仅在文章末尾提供源码，请自行下载python 运行环境运行，详情请见视频教程有关运行源码的说明)，弹窗内选择本地mdx文件。 

![](/images/awesometts-mdx-server-001.jpg)

- console窗口内显示port:8000 表明服务器运行成功，等待外部请求。 

![](/images/awesometts-mdx-server-002.jpg)

## 运行AwesomeTTS生成Anki卡片音频

- 将AwesomeTTS.zip文件解压至“我的文档\Anki\addons”目录后，重启anki激活插件。 

![](/images/awesometts-mdx-server-003.jpg)

- 在Anki浏览器AwesomeTTS界面，选择LDOCE6 on MDX server 服务，并选择英音或者美音生成音频。 

![](/images/awesometts-mdx-server-004.jpg)

## 运行AwesomeTTS视频教程 
链接：[优酷视频:Anki AwesomeTTS and MDX Server](http://v.youku.com/v_show/id_XMTgxMDIwODc3Ng==.html)

## MDX server 源码(含朗文6词典)下载

链接：[https://pan.baidu.com/s/1LhZasr6p7Fkn9aMuMc1RFA](https://pan.baidu.com/s/1LhZasr6p7Fkn9aMuMc1RFA) 密码：6gu1 

用法：请自行下载python运行环境，将上述压缩包解压到本地某目录后，双击目录内mdx_server.py运行(本版自带朗文词典，故无需像视频中那样选择mdx文件) 

_若百度链接失效，请留言请求更新_

## 定制版awesometts下载

链接：[AwesomeTTS.zip](/files/AwesomeTTS.zip) 

用法：解压复制到Anki插件addon目录(仅适用于anki 2.0版本，不可用于anki 2.1)。