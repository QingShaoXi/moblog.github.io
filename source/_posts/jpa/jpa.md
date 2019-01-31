---
title: Java开发中MyBatis、Hibernate、Spring Data JPA应该如何选择？
date: 2019-01-31 13:30:30
tags:
 - 编程
 - SQL
 - Spring Data JPA
categories:
 - JAVA
---
# 引言
> 大家知道目前Java开发中MyBatis、Hibernate、Spring Data JPA是3个使用比较普遍的持久化框架，但是我们在实际项目中应该如何选择呢？我们对此做一下分析。
<!--more-->

## 一.简单介绍

1. Hibernate

Hibernate是将POJO通过Xml映射文件（或注解）提供的规则映射到数据库表上，是一种全表映射的模型，可以通过POJO直接操作数据库。我们不需要写SQL，只要使用HQL语言就可以了。

2. MyBatis

Mybatis是半自动的框架。之所以说它是半自动的，是因为它需要手工匹配提供POJO、SQL和映射关系，而Hibernate只需要提供POJO和映射关系即可。

3. Spring Data JPA

Spring Data JPA是在JPA规范的基础下提供了Repository层的实现，是对ORM框架的进一步抽象封装，它不直接代替ORM框架，默认底层使用的ORM框架是Hibernate，但可以灵活的在各种ORM框架之间切换，同时也简化了我们对ORM框架的使用。

综上，使用Hibernate的可以使用Spring Data JPA来简化开发了。
我们只需要在MyBatis和Spring Data JPA之间做选择，而这个选择还是得看MyBatis和Hibernate的对比。

## 二.优缺点

Java开发中MyBatis、Hibernate、Spring Data JPA应该如何选择？
### 1.MyBatis

#### 1.1.优点

它是一个半自动化的持久层框架，支持动态SQL，灵活可控。
更容易掌握，入门简单，即学即用，学习成本低。
#### 1.2.缺点

需要维护SQL和结果映射，增加了工作量。
移植性差，所有的SQL语句都依赖所用的数据库，对不同数据库类型的支持不好。

### 2.Hibernate

#### 2.1.优点

不需要维护SQL和结果映射，开发工作量少。
移植性好，所有的 HQL 语句与具体使用的数据库无关。
#### 2.2.缺点

性能相对较差。
学习门槛不低，精通门槛更高，学习成本高。

## 三.适用场景

Java开发中MyBatis、Hibernate、Spring Data JPA应该如何选择？
### 1.MyBatis

数据量大，高并发。
表关联比较复杂。
要求对于数据库可控性好， 可深度调优。

### 2.Hibernate

场景不太复杂。
需求变化不多。
性能要求不高。

## 四.总结

目前来看传统企业使用Spring Data JPA的比较多，而互联网行业更倾向于使用MyBatis，如阿里及其旗下的很多子公司都在用MyBatis。
在实际使用时可以结合各个框架的优缺点、项目情况、研发人员的技术情况等综合评估和选择。