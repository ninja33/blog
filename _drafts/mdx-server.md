---
title: 词典服务 MDX Server
tags:
  - anki
categories:
  - 学习工具
date: 2016-11-13 01:50:15
---

#### 2018年11月补充说明

很多同学会用awesometts配合mdx server来导入朗文真人发音。那么现在导入朗文音频的话，可以用fastwq这个anki插件。直接就把朗文音频导入了，也不用装mdx server，也不用装awesometts，一个插件就搞定了。速度还很快。mdx server这个方法很老了，大家可以尝试一下新方法 插件地址： 
[https://ankiweb.net/shared/info/1807206748](https://ankiweb.net/shared/info/1807206748)

* * *

#### 使用说明

目前流行的MDX词典文件只能在Mdict, GoldenDict, 欧路，深蓝等词典软件中使用，而不能将内容对外输出。MDX Server通过读取MDX、MDD格式的词典文件，对外部提供一个标准的HTTP服务接口。使得一些需要词典服务的软件，比如Kindlemate，Anki划词助手以及其他工具可以利用这个本地服务，灵活选取所需的MDX词典，批量或者单独获取单词的解释。 下面列出具体安装使用方法:
<!-- more -->

1.  将zip文件解压至任意目录后，点击运行mdx_server.exe，弹窗内选择本地mdx文件。 
![](/images/mdx-server-001.jpg)
2.  console窗口内显示port:8000 表明服务器运行成功，等待外部请求。 
![](/images/mdx-server-002.jpg)
3.  在浏览器输入 http://localhost:8000/{word}，{word}为待查单词，比如http://localhost:8000/test，通过mdx-server查询，浏览器内将显示相应词典的解释，并可点击播放词典内置音频。
4.  如需引用外部css或脚本等外部资源，可将资源放在mdx子目录。
5.  下面列出mdx-server运行状况(与GoldenDict对比)

*   柯林斯五星英汉双解 
![](/images/mdx-server-003.jpg)
*   朗文6 
![](/images/mdx-server-004.jpg)
*   麦克米兰 
![](/images/mdx-server-005.jpg)
*   牛津高阶学习词典第八版 
![](/images/mdx-server-006.jpg)
*   新牛津英汉双解第二版 
![](/images/mdx-server-007.jpg)
*   Vocabulary.com 
![](/images/mdx-server-008.jpg)

#### 视频教程

有关MDX Server的具体应用案例之一:配合Anki插件AwesomeTTS下载音频，可见另一篇文章 [AwesomeTTS (MDX Server版)使用说明(含视频教程)](http://www.laohuang.net/20161113/awesometts-mdx-server/)

#### 文件下载

链接：[https://pan.baidu.com/s/1jJG5LPW](https://pan.baidu.com/s/1jJG5LPW) 密码：h6kr