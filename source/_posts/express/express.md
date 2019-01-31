---
title: express安装
date: 2019-01-31 11:03:35
tags:
 - express
categories:
 - nodejs
---
# 前言
> 在你的windows上已经安装了node.js的基础上再安装express
<!--more-->
## 第一部分:安装express 

* 第一步:执行 npm install -g express-generator 

note:必须安装这个,不然创建express项目的时候会提示express命令没有找到

* 第二步:执行 npm install -g express

* 第三步:执行 express -V 或者 express --version

note:'V'是大写的,如果express安装成功会显示版本号

## 第二部分:创建一个express项目 

* 第一步:执行 express youProjectName

note:youProjectName是你的项目的名称,按照自己的要求选择合适的项目名称

* 第二步 :进入你的项目:cd youProjectName

* 第三步:在你的项目的目录下执行 npm install

* 第四步:启动你的项目,执行 npm start

## 第三部分:在浏览器中访问你的项目

> 打开你的浏览器,在地址栏中输入:http://127.0.0.1:3000

> 然后你会看到:express的欢迎信息 

> 最后:开启你的express之旅吧,祝君工作愉快! 