---
layout: post
title: Intellij IDEA SNV 切换分支
description: 使用Intellij IDEA进行开发，SNV上新建了分支之后，如何切换到新的分支。关键字：Java,IDEA,SNV,分支切换
category: blog
---

今天公司项目的SNV新建了分支，才使用IDEA开发不久，发现不能切换的新的SVN分支。自己研究半天，找到了解决方法。


IDEA自带的SVN插件没有切换分支的选项，所以不能再IDEA中直接切换分支。发现两种方法可以解决这个问题。

1. 用SVN工具，找到工程目录，在目录中使用点击右键->Tortoise SNV->switch,在弹出的窗口中选择或输入新的分支地址，点击确定，搞定。

2. 进入到工程目录使用命令行，使用SVN命令（需先安装subversion for windows）
svn switch <需要切换到的svn地址>