---
layout: post
title: "Machine Learning Algorithm"
excerpt: "机器学习算法的总结，持续更新"
modified: 2016-05-27
categories: articles
tags: [Machine Learning, Python]
image:
  feature: so-simple-sample-image-1.jpg
  credit: WeGraphics
  creditlink: http://wegraphics.net/downloads/free-ultimate-blurred-background-pack/
comments: true
share: true
---

# 机器学习算法总结

## 何为机器学习？
用机器去学习数据中的经验，利用数据构建策略模型。

### 其中机器学习分为：

* 有监督学习：有训练数据集
* 无监督学习：无训练数据集
* 半监督学习
* 强化学习

### 有监督机器学习主要解决的问题：

* 分类问题：文本情感倾向性分类、新闻（网页）自动分类、图像识别
* 回归问题：预测电影票房

### 开发及其学习应用的步骤：

1. 收集数据：爬虫数据、DPI数据、[公开数据集](https://www.kaggle.com/datasets)、传感器数据、
2. 数据预处理：数据清洗、规约、过滤
3. 探索数据：检查前两部的数据处理结果，探索数据基本情况，思考如何选择数据特征
4. 训练模型：选择合适的机器学习算法训练模型
5. 评估模型：评估模型效果，不满意需返回第4步优化
6. 应用模型：将算法转化为应用程序


## 内容提纲：

* 算法介绍

	* 有监督学习：

		* [K-近邻算法(KNN，K-nearest neighbors)](../../images/html/K-近邻算法.html)
		* [朴素贝叶斯](../../images/html/朴素贝叶斯.html)
		* [逻辑回归](../../images/html/Logistic.html)
		* [支持向量机](../../images/html/SVM.html)

* 案例解析：[利用scikit-learn实现文本分类](../../images/html/利用scikit-learn实现文本分类.html)

## 如何选择算法?
> [图片引用自这里](http://scikit-learn.org/stable/tutorial/machine_learning_map/index.html)

<img src="../../images/ml_map.png" width="2000px">
