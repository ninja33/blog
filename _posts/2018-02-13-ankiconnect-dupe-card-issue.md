---
layout: post
title: duplicated cards creation for ankiconnect
categories: 学习工具
description: 缺省的Ankiconnect不能重复制卡
keywords: ankiconnect
date: 2018-02-13 21:58:26
tags:
---

2019/2/10 update: Sometime, you occasionally can not create cards(not always), actually it's not extension's problem. Because it does not allow duplicated cards(with same sorted field) creation in ankiconnect by default. To solve this problem, you can manually edit ankiconnect source, and change it's default behavior. 

It's different way to find ankiconnect source in anki 2.0 and 2.1 In anki 2.0, you may find it by click menu: tool -> add-ons -> open add-ons folder, then find file named **ankiconnect.py** 

![](/images/anki_duplication_for_20.png) 

In anki 2.1, you may find it by click menu: tool -> add-ons -> select Ankiconnect in list -> view files, then find file named **__init__.py** 

![](/images/anki_duplication_for_21.png) 

No matter it's named ankiconnect.py or \_init\_.py, actually it's same file for different version(v2.0 and v2.1), you may use your favorit text edtor open it and go to line around #452. then change code from `allowDuplicate = False` to `allowDuplicate = True`. That's it. You can restart anki and try if your work can be continued. Any further questions, please leave your comment and let me know. 

![](/images/anki_duplication.png)

2019年2月10日更新 有时候，你会发现插件偶尔会制卡失败(并不是总是失败)，事实上这个不是插件的问题。Anki的Ankiconnect插件在缺省情况下，是不允许重复制卡的(有相同的排序字段)。为了解决这个问题，你可以直接修改ankiconnect的源文件以改变它的缺省行为。在anki 2.0和2.1中，可以用不同的方法找到ankiconnect的源文件。 在anki 2.0中，你可以点选菜单 tool(工具) -> add-ons(插件) -> open add-ons folder(打开插件目录)，然后找到一个名为 **ankiconnect.py** 的文件。

![](/images/anki_duplication_for_20.png)

 在anki 2.1中，你可以点选菜单 tool(工具) -> add-ons(插件) -> 在列表中点选Ankiconnect->view file (检视文件)，然后找到一个名为 **__init__.py** 的文件。 
 
 ![](/images/anki_duplication_for_21.png) 
 
 不管叫什么名称，其实他们是不同版本(v2.0 and v2.1)下的同一个文件，你可以用你常用的文本编辑器打开此文件，然后在大约452行左右的地方，把代码从 `allowDuplicate = False` 改成 `allowDuplicate = True` 好了，然后重启anki，看看还有没有类似问题。 如果还有任何问题，请在下方留言告知。 
 
 ![](/images/anki_duplication.png)