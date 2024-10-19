---
title: 対称差
date: 2024-10-19
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

集合の対称差について解説します。

<!--more-->

## 前提知識

- [和集合]({{< ref "def_union">}})
- [共通部分]({{< ref "def_intersection">}})
- [差集合]({{< ref "def_set_difference">}})

## 定義

{{% def "対称差 (intersection)" %}}
$X, Y$を集合とする。$X$か$Y$に属するが、両方には属さない元の集合を$X$と$Y$の**対称差**といい、$X \triangle Y$とかく。つまり、
$$X \triangle Y := (X \cup Y) \setminus (X \cap Y)$$

{{% /def %}}

## 注意

- $X \triangle Y = (X \setminus Y) \cup (Y \setminus X)$である。こちらを定義とすることもある。
- De Morganの法則より、$X^c \triangle Y^c = X \triangle Y$が成り立つ。
- 対称差は排他的論理和 (exclusive or; xor)という論理演算と対応している。

## 参考文献
