---
layout: post
title: "线性规划-单纯形算法"
excerpt: "介绍如何用单纯形法求解线性规划算法"
modified: 2017-05-12
categories: articles
tags: [LP, Algorithm]
comments: true
share: true
---

<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>

$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$

## 线性规划问题
最小化 
	$$-2x_1 + 3x_2$$
满足约束
	$$x_1 + x_2 = 7$$
	$$x_1 - 2x_2 ≤ 4$$
	$$x_1 >= 0$$

## 标准型定义

最大化 
	$$c^Tx $$
满足约束
$$ Ax ≤ b $$
$$ x ≥ 0$$

满足一下4个原因之一，则不是标准型:

* 目标函数可能是最小化
* 可能有变量<0
* 可能有等式约束
* 可能有≤约束

如何变为标准形式？

* 原来是min, 直接*-1求max
* 若原来约束为=，转为 >= 和<=
* 约束原来为 >= 同样的*-1，就改变了<=
* 若有变量 xi < 0 ，那么用 x‘ – x”来替代，其中 x’>=0 x”>=0

上述问题就变为了
最大化 
	$$2x_1 - 3x_2 + 3x_3 $$
满足约束
$$ x_1 + x_2 - x_3 ≤ 7 $$
$$ -x_1 - x_2 + x_3 ≤ -7$$
$$ x_1 - 2x_2 + 2x_3 ≤ 4$$


## 松弛型
最大化 
	$$c^Tx $$
满足约束
$$ Ax = b $$
$$ x ≥ 0$$



