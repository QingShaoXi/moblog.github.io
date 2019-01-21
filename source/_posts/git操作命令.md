---
title: git操作命令
date: 2019-01-18 17:10:40
tags:
 - Git
categories:
 - 工具 
---
Git tag 给当前分支打标签
原文已经找不到出处，重新整理格式，仅作个人收藏！

标签(Tag)可以针对某一时间点的版本做标记，常用于版本发布。
<!--more--> 
列出tag
$ git tag # 在控制台打印出当前仓库的所有tag
$ git tag -l ‘v0.1.*’ # 搜索符合模式的Tag
打tag
git tag分为两种类型：轻量tag和附注tag。轻量tag是指向提交对象的引用，附注Tag则是仓库中的一个独立对象。建议使用附注Tag。

创建轻量Tag
$ git tag v0.1.2-light
创建附注Tag
$ git tag -a v0.1.2 -m “0.1.2版本”
创建轻量Tag不需要传递参数，直接指定Tag名称即可。

创建附注Tag时，参数a即annotated的缩写，指定Tag类型，后附Tag名。参数m指定Tag说明，说明信息会保存在Tag对象中。

切换到Tag
与切换分支命令相同，用git checkout [tagname]

查看Tag信息
用git show命令可以查看Tag的版本信息：

$ git show v0.1.2
删除Tag
误打或需要修改Tag时，需要先将Tag删除，再打新Tag。

$ git tag -d v0.1.2 # 删除Tag
参数d即delete的缩写，意为删除其后指定的Tag。

给指定的commit打Tag
打Tag不必要在head之上，也可在之前的版本上打，这需要你知道某个提交对象的校验和（通过git log获取）。

补打Tag

$ git tag -a v0.1.1 9fbc3d0
Tag推送到服务器
通常的git push不会将Tag对象提交到git服务器，我们需要进行显式的操作：

$ git push origin v0.1.2 # 将v0.1.2 Tag提交到git服务器
$ git push origin –-tags # 将本地所有Tag一次性提交到git服务器
注意：如果想看之前某个Tag状态下的文件，可以这样操作

1.git tag 查看当前分支下的Tag

2.git checkout v0.21 此时会指向打v0.21 Tag时的代码状态，（但现在处于一个空的分支上）

cat test.txt 查看某个文件
