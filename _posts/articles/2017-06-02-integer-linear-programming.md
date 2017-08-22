---
layout: post
title: "整数线性规划"
excerpt: "介绍如何解整数线性规划"
modified: 2017-06-2
categories: articles
tags: [LP, ILP, Algorithm]
comments: true
share: true
---

分支定界法

首先求出ILP对应的LP问题的解。如果解中存在非整数，则按照非整数的上下求整，将ILP原问题划分为两个LP问题，并且添加边界的约束条件，直到求得整数解。

对于特定的0-1规划问题，可以采用枚举法。而枚举的过程中，可以将当前目标函数的最大值作为约束放入其中，从而加快枚举过程。


[参考课件 http://cse.seu.edu.cn/PersonalPage/yangwu/](../../images/20170602/ILP.pdf)