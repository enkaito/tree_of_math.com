---
title: 存在量化子
date: 2026-05-17
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

述語に対する存在量化子の定義について解説します。

<!--more-->

## 前提知識

- [命題]({{< ref "def_proposition" >}})
- [述語]({{< ref "def_predicate" >}})

## 定義

{{% def "存在量化子 (existential quantifier)" %}}
集合$X$と述語$P(x)$に対し、「ある$x \in X$が存在して$P(x)$が成り立つ」ことを
$$\exists x \in X, P(x)$$
と書き、記号$\exists$を**存在量化子**という。

{{% /def %}}

## 注意

- $\exists x, P(x)$は$X$を省略した書き方で、文脈で定義域を定める。
- $\exists x \in X, P(x)$は$\exists x (x \in X \wedge P(x))$の省略とみなせる。

## 参考文献
