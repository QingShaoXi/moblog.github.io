---
title: 最实用的 Markdown 语法教程
date: 2019-01-31 09:47:45
tags:
 - markdown语法
categories:
 - 工具
---
# 前言 
> 最近不是很忙,仔细研究了一下Markdown语法,忽然有种相见恨晚的感觉,因为用它来写文档，那是相当的舒服，特别feeling。废话少说，咱们开始正题吧〜
<!--more-->


## 培训内容：
* Markdown 是什么？
* Markdown 是谁创造的？
* 为什么要使用Markdown?
* Markdown怎么使用？
* Markdown 都有哪些人在用？
* 尝试一下Markdown的使用！
* Markdown 进阶语法！


{% note success %} 学习目标 {% endnote %}
  通过学习，能对Markdown语法有个比较全面的认知，对日常工作写作排版尽量放弃Word、txt等文本工具，改直接用Markdown语言写文档。

{% note success %} 学思路 {% endnote %}
```
1.一开始，先记住 # 这是标题、## 这是二级标题、### 这是三级标题、...这时候你写一般小文章会开始感觉 MD 不错。

2.然后，你发现标题不适合做列表，记住了用1. 第一点、- 这一点来列表超级方便。

3.好吧，写作总要有些重点吧，**加粗**、*斜体*、~~删除线~~开始派上用场了。这时你基本不会打开 Word 那样的笨重软件了。

4.> 这是引用

5.你越来越喜欢，自然会去查查维基（Markdown）还有什么语法，加上多用，很快就基本掌握了。MD 还有表格、锚、注脚、贴图等。强烈推荐 Mou，按 ⌘＋R 可以快速查看语法。

6.慢慢，你会发现，总有小「bugs」，如列表内无法内嵌代码段。上网查查，你开始理解 MD 的缩进内嵌机制等高级隐形内容，这样你就 Master 了！
```
以下是 Mou 下面的效果，多么漂亮：

![效果](https://upload-images.jianshu.io/upload_images/1293430-55f1c047cf9a1011.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1000/format/webp)





Mou 写出的效果

# 正文
{% note success %} 一、Markdown是什么？ {% endnote %}

Markdwon 是一种轻量级 标记语言，它以纯文本形式（易读、易写、易更改）编写文档，并最终以HTLM格式发布。Markdown也可以理解为将以 MARKDOWN语法编写的语言转换成HTML内容的工具。

{% note success %} 二、Markdown是谁创造的？ {% endnote %}

它是由 Aaron Swartz 和 [John Gruber](https://baike.baidu.com/item/John Gruber/18550453?fr=aladdin) 共同设计， Aaron Swartz 就是那位（2013年1月11日）自杀，有着开挂一般人生经历的程序员。 维基百科对他的介绍是：软件工程师、作家、政治组织者、互联网活动家、维基百科人。
他有着足以让你跪拜的人生经历。

14岁参与RSS 1.0规格标准制订。

2004年入读斯坦福大学，之后退学。

2005年创建 Infogami,之后与Reddit合并成为其合伙人。

2010年创立示进会（Demand Preogress）,积极参与禁止网络盗版法案（SOPA）活动，最终该提案被撤回。

2011年7月19日,因被控从MIT和JSTOR下载480万篇学术论文并以免费形式上传于网络被捕。

2013年1月自杀身亡。

##### Aaron Swartz 大神照片

![大神](https://upload-images.jianshu.io/upload_images/1293430-67a409e21507d498.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/401/format/webp)

{% note success %} 三、为什么要使用Markdown? {% endnote %}

它是易读（看起来舒服😌）、易写（语法简单）、易更改（纯文本）。处处体现着极简主义的影子。
兼容HTML,可以转换为HTML格式发布。
跨平台使用。
越来越多的网站支持Markdown.
更方便清晰的组织你的电子邮件。（Markdown-here,Airmail）。
摆脱Word,txt！！！


{% note success %} 四、Markdown怎么使用？ {% endnote %}

如果不算扩展，Markdown的语法绝对简单到让你爱不释手！
Markdown语法分为如下几大部分：
▸ 标题
▸ 段落
▸ 区块引用
▸ 代码区块
▸ 强调
▸ 列表
▸ 分割线
▸ 链接
▸ 图片
▸ 反斜杠
▸ 符号
▸ 表格
▸ 流程图


#### 4.1 标题
####### 1）使用= 和 -，标记一级和二级 标题。

```
示例md代码:
一级标题
=
二级标题
-
```
示例效果：
![](https://upload-images.jianshu.io/upload_images/1293430-53ab03e9817c324b.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/385/format/webp)


####### 2）使用 #,可以表示 1-6级 标题。
```
示例md代码:
# 第一级标题 `<h1>` 
## 第二级标题 `<h2>` 
### 第三级标题 `<h3>` 
#### 第二四级标题 `<h4>` 
##### 第五级标题 `<h5>` 
###### 第六级标题 `<h6>` 
```
示例效果：
![](https://upload-images.jianshu.io/upload_images/1293430-53e892b81b908d00.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/475/format/webp)

#### 4.2 段落


段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用两个以上空格加上回车（引用中换行省略回车）


#### 4.3 区块引用


在段落的每行或者只在第一行使用符号 > ,还可使用多个嵌套引用，如：
```
示例md代码:
> 区块引用
> > 嵌套引用
> > >三嵌套引用
> > > > 四嵌套引用
```
示例效果：
![](https://upload-images.jianshu.io/upload_images/1293430-aa265ce53d458695.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/393/format/webp)

#### 4.4代码区块


代码区块的建立是在每行加上4个空格或者一个制表符（如同写代码一样）。如普通段落：
```
示例md代码:
fun main(args: Array<String>) {
   println("Hello World!")

   println("sum = ${sum(34, 67)}")
   println("sum = ${sum(34, 67)}")
   println("sum = ${sum(34, 6, 57, 34)}")

   printSum(237, 57)
   printSum(234, 567, 8)
   vars(1, 4, 6, 78, 0, 6, 9, 8)


   val sumLambda: (Int, Int) -> Int = { x, y -> x + y }
   println("sumLambda = ${sumLambda(3, 6)}")


//    if (args.size < 2) {
//        println("Two integers expected")
//        return
//    }
   testFor()


   val a: Int = 1000
   println(a === a)//true 值相等，对象地址相等

   //经过了装箱，创建了两个不同的对象
   val boxedA: Int? = a
   val anotherBoxedA: Int? = a

   //虽然经过了装箱，但是值是相等的，都是10000
   println(boxedA === anotherBoxedA) //  false，值相等，对象地址不一样
   println(boxedA == anotherBoxedA) // true，值相等
}
```
注意⚠️：需要和普通段落之间存在空行！


#### 4.5 强调


在强调内容两侧分别加上 *或者 -,如：
```
示例md代码:
*斜体* ，_斜体_
**加粗**，__粗体__
```
示例效果：
![](https://upload-images.jianshu.io/upload_images/1293430-a0818b2f5481a48d.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/475/format/webp)



#### 4.6 列表 （有序，无序）
使用 . 、+、或- 标记无序列表，如：
```
示例md代码:
-   第一项
+   第二项
-   第三项
+   第四项
-   第五项
+   第六项
```
示例效果:
![](https://upload-images.jianshu.io/upload_images/1293430-a214fe776adff15b.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/399/format/webp)
**注意：标记后面最少有一个_空格_或_制表符_。若不在引用区块 中，必须和前方段落之间存在空行。**
<font color ="red">示例md代码:</font>
```
 1. 第一项
 2. 第二项
 3. 第三项
 4. 第四项
 5. 第五项
 6. 第六项
```
示例效果:
![](https://upload-images.jianshu.io/upload_images/1293430-d66a2e0b2e504ec5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/475/format/webp)

#### 4.7 分割线


分割线最常使用就是三个或以上的 *  ， ======</font>还可以使用  - 和 _。
<font color ="red">示例md代码:</font>
```
***
---
_____ 
======
```
示例效果:
![](https://upload-images.jianshu.io/upload_images/1293430-44cbdb7aa7b063b3.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/745/format/webp)

#### 4.8链接


链接可以由两种形式生成，行内式 和 参考式。
###### 行内式：
<font color ="red">示例md代码:</font>
```
[GitHub](http://github.com)
自动生成连接  <http://www.github.com/>
```
示例效果:
![](https://upload-images.jianshu.io/upload_images/1293430-aad2a0468efc03a1.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/669/format/webp)
###### 参考试：
```
[GitHub][1]
[1]:http://github.com
自动生成连接  <http://www.github.com/>
```
示例效果:
![](https://upload-images.jianshu.io/upload_images/1293430-58c89b40f71f6079.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/684/format/webp)

注意：上述的 [1]:http://github.com 不出现在区块中。


#### 4.9 图片


添加图片形式和链接相似，只需要在链接的基础上前方加一个  ！号。
示例md代码:
```
![GitHub set up](http://zh.mweb.im/asset/img/set-up-git.gif)
格式: ![Alt Text](url)
```
![GitHub set up](http://zh.mweb.im/asset/img/set-up-git.gif)


#### 4.10 反斜杠  ''

相当于反转义作用。使符号成为普通符号。


#### 4.11 符号 ``


起到标记作用，如标签：
Ctrl+A 、Ctrl+C、Ctrl+V


#### 4.12 表格

```
示例md代码:
第一格表头 | 第二格表头
---------| -------------
内容单元格 第一列第一格 | 内容单元格第二列第一格
内容单元格 第一列第二格 多加文字 | 内容单元格第二列第二格
内容单元格 第一列第三格 多加文字 | 内容单元格第二列第三格
内容单元格 第一列第四格 多加文字 | 内容单元格第二列第四格
```
示例效果:
![](https://upload-images.jianshu.io/upload_images/1293430-8bf48379fc9c4b34.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/564/format/webp)

#### 4.12 流程图
```
示例
st=>start: Start:>https://www.jpjbp.com/
io=>inputoutput: verification
op=>operation: Your Operation
cond=>condition: Yes or No?
sub=>subroutine: Your Subroutine
e=>end

st->io->op->cond
cond(yes)->e
cond(no)->sub->io
```

更多语法参考：[流程图语法参考](http://adrai.github.io/flowchart.js/)

{% note success %} 五、Markdown都哪些人在用？ {% endnote %}
Markdown 的使用作者：
Github、
简书、
StackOverFlow、
Apollo、
Moodle、
Reddit、
CSDN
等等


{% note success %} 六、尝试一下Markdown的使用！{% endnote %}

Chrome下的插件诸如stackedit与markdown-here等非常方便，也不用担心平台受限。
在线的dillinger.io评价也不错
Windowns下的MarkdownPad也用过，不过免费版的体验不是很好
Mac下的Mou是国人贡献的，口碑很好。
Linux下的ReText不错。

>>>Github传送门
TOC
Markdown 语法：
[TOC]


## 总结：

通过这次学习，自己也对MD语法有一个全新的认识，万事开头难，只要你偿试用MD 写工作中的文档，从此告别Word ，TXT！！！我相信你也会喜欢上这门语言。此外，如有写的不对的地方，勿喷！！！  欢迎指正！


  作者：KKKnight_
  链接：https://www.jianshu.com/p/f3147a804368
  來源：简书
  简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。