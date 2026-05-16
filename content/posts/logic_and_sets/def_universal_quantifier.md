---
title: 全称量化子
date: 2026-05-17
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

述語に対する全称量化子の定義について解説します。

<!--more-->

## 前提知識

- [命題]({{< ref "def_proposition" >}})
- [述語]({{< ref "def_predicate" >}})

## 定義

{{% def "全称量化子 (universal quantifier)" %}}
集合$X$と述語$P(x)$に対し、「任意の$x \in X$について$P(x)$が成り立つ」ことを
$$\forall x \in X, P(x)$$
と書き、記号$\forall$を**全称量化子**という。

{{% /def %}}

## 注意

- $\forall x, P(x)$は$X$を省略した書き方で、文脈で定義域を定める。
- $\forall x \in X, P(x)$は$\forall x (x \in X \to P(x))$の省略とみなせる。
- $X = \empty$のとき、$\forall x \in X, P(x)$は虚無に真となる。

## 参考文献
