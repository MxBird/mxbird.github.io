---
layout: post
title: "Ruby的<=>运算符"
description: "最近在重新梳理自己的ruby知识,很多都不牢靠啊!"
date: 2013-11-11
categories: code
---

最近在重新梳理自己的ruby知识,发现自己还是很多细节的知识不是很明了,比如今天要说到的 `<=>` 运算符.

```
#a <=> b
#如果a等于b 返回结果 0
#如果a大于b 返回结果 1
#如果a小于b 返回结果 -1
2.0.0p247 :001 > 1 <=> 1
 => 0
2.0.0p247 :002 > 1 <=> 0
 => 1
2.0.0p247 :003 > 1 <=> 2
 => -1
```  

虽然这是一个很基础的知识,但是刚看到还是不知所以然,足以说明自己的知识细节掌握的还是不全面.
通过文档查阅发现:其它比较操作符（>,>=,<,<=）均是调用<=>
