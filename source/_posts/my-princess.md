---
title: next 内嵌标签demo
date: 2019-01-19 14:43:24
tags:
 - next
categories:
 - hexo
---
<!-- HTML方式: 直接在 Markdown 文件中编写 HTML 来调用 -->
<!-- 其中 class="blockquote-center" 是必须的 -->
<blockquote class="blockquote-center">blah blah blah</blockquote>

<!-- 标签 方式，要求版本在0.4.5或以上 -->
{% centerquote %}blah blah blah{% endcenterquote %}

<!-- 标签别名 -->
{% cq %} blah blah blah {% endcq %}
<!--more--> 
<!-- HTML方式: 直接在 Markdown 文件中编写 HTML 来调用 -->
<!-- 其中 class="full-image" 是必须的 -->
<img src="http://pkyddcyaj.bkt.clouddn.com/1gk2b6atw4ekecufreb9.jpg" class="full-image" />

<!-- 标签 方式，要求版本在0.4.5或以上 -->
{% fullimage http://pkyddcyaj.bkt.clouddn.com/1gk2b6atw4ekecufreb9.jpg, alt, title %}

<!-- 别名 -->
{% fi http://pkyddcyaj.bkt.clouddn.com/1gk2b6atw4ekecufreb9.jpg, alt, title %}


{% note default %} 1 {% endnote %}

{% note primary %} 2 {% endnote %}

{% note success %} 3 {% endnote %}

{% note info %} 4 {% endnote %}

{% note warning %} 5 {% endnote %}

{% note danger %} 6 {% endnote %}

#### 《告白气球》
<audio id="audio" controls="" preload="none">
      <source id="mp3" src="http://211.97.73.141/amobile.music.tc.qq.com/C400003OUlho2HcRHC.m4a?guid=5779674855&vkey=0313A344E3B6554A2B98C1E0E04DB98F5ABEC82B6D67567D975C1D96A2F7A3771B4CF480486BE15B0045F9AE4E2BEAF4B85778A076B1328C&uin=0&fromtag=66">
</audio>