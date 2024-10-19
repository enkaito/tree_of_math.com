---
title: 共通部分（積集合）
date: 2024-10-19
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

共通部分について解説します。

<!--more-->

## 前提知識

- [集合]({{< ref "def_set">}})

## 定義

{{% def "積集合（共通部分） (intersection)" %}}
$X, Y$を集合とする。$X$か$Y$のどちらにもに属する元の集合を$X$と$Y$の**共通部分（積集合）**\ といい、$X \cap Y$とかく。つまり、
$$X \cap Y := \set{x; x \in X \wedge x \in Y}$$

より一般に、集合族$\mathcal{F}$に対し、集合族の集合のすべてに属する元の集合を共通部分といい、$\bigcap \mathcal{F}$とかく。つまり、
$$\bigcap \mathcal{F} := \set{x; \forall X \in \mathcal{F}, x \in X}$$

集合族$\cal{F}$が$\mathcal{F} = \set{X_\lambda}_{\lambda \in \Lambda}$と添字付けられている場合、共通集合を$\bigcap_{\lambda \in \Lambda} X_\lambda$とかく。つまり、
$$\bigcap_{\lambda \in \Lambda} X_\lambda := \set{x; \forall \lambda \in \Lambda, x \in X_\lambda}$$

{{% /def %}}

## 注意

- 共通部分は交差、交わりとも呼ばれる。
- 記号$\cap$はキャップと読むことがある。
- ここでの積集合と直積集合は異なる概念である。

## 参考文献
