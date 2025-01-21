---
title: 全順序
date: 2024-10-21
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

全順序の定義を解説します。

<!--more-->

## 前提知識

- [二項関係]({{< ref "def_binary_relation">}})
- [前順序]({{< ref "def_preorder">}})
- [半順序]({{< ref "def_partial_order">}})

## 定義

{{% def "全順序 (total order)・全順序集合 (totally ordered set)" %}}
$\preceq$を集合$X$上の[二項関係]({{< ref "def_binary_relation">}})とする。
$\preceq$が以下を満たすとき、$X$上の**全順序**という。

1. $\forall x \in X, x \preceq x$
2. $\forall x, y, z \in X, x \preceq y \; かつ  \; y \preceq z \implies x \preceq z$
3. $\forall x, y \in X, x \preceq y \; かつ \; y \preceq x \implies x = y$
4. $\forall x, y \in X, x \preceq y \; または \; y \preceq x$

言い換えると、全順序とは4を満たす[半順序]({{< ref "def_partial_order">}})のことである。

全順序を備えた集合を**全順序集合**という。

{{% /def %}}

## 注意

- 1の性質を**反射律**、2の性質を**推移律**、3の性質を**反対称律**、4の性質を**完全律**という。
- $\prec$を「$x \prec y :\iff x \preceq y \; かつ \; x \neq y$」で定めると、$\prec$は**三分律**と呼ばれる以下の性質を満たす。
  $$\forall x, y \in X \;について\; x \prec y, y \prec x, x = y \; のいずれか1つが必ず成り立つ$$

## 参考文献
