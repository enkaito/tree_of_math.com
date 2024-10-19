---
title: 差集合
date: 2024-10-19
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

差集合について解説します。

<!--more-->

## 前提知識

- [集合]({{< ref "def_set">}})

## 定義

{{% def "差集合 (set difference)" %}}
$X, Y$を集合とする。$X$に属するが$Y$には属さない元の集合を$X$と$Y$の**差集合**といい、$X \setminus Y$とかく。つまり、
$$X \setminus Y := \set{x \in X; x \notin Y}$$

{{% /def %}}

## 注意

- 補集合の記号を用いて、$X \setminus Y = X \cap Y^c$ともかける。
- $X \setminus Y$は$X - Y$とも書かれることがある。しかし、$X, Y$が演算$-$をもつ場合、$X - Y$で$\set{x - y; x \in X, y \in Y}$を表すこともあるため注意。

## 参考文献
