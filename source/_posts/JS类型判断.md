---
title: JS类型判断
date: 2020-04-14 00:29:04
tags: ['JS','js类型']
---

我们都知道 JS 是弱类型语言，跟java等强类型语言不同，我们只能在运行时才真正知道某个变量是属于哪一种类型，因为在此之前，你可能有意无意的改变了变量的类型，因为变量的值及其数据类型可在声明周期内改变，这也是bug的来源，相信很多小伙伴都深有体会😆。
<!-- more -->
### 数据类型

我们都知道，JS 中变量分为两种类型。基本类型和引用类型。

#### 基本类型
基本类型包括```Undefined、Null、String、Number、Boolean、Symbol```。基本类型按值访问，所以我们可操作保存在变量中实际的值。

基本类型的值在内存中占据固定大小的空间，是被保存在栈内存中。从一个变量向另一个变量复制基本类型的值，会创建这个值的一个副本，这两个值完全独立地存放在栈内存中。

#### 引用类型
引用类型是对象类型，包括```Object、Array、Function、Data、Regexp、Error```。引用类型的值是保存在堆内存中的对象，JS不允许直接访问内存中的位置，也就是说不能直接访问操作对象的内存空间。

操作对象时，实际上是在操作对象的引用，所以说引用类型的值是按引用访问的。从而有```[1, 2] === [1, 2]```为```false```。