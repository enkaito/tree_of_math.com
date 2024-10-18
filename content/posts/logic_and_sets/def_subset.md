---
title: 部分集合
date: 2024-10-18
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

部分集合について解説します。

<!--more-->

## 前提知識

- [集合]({{< ref "def_set">}})

## 定義

{{% def "部分集合 (subset)" %}}
$X, Y$を集合とする。$Y$に属する元がすべて$X$にも属するとき、$Y$は$X$の**部分集合**であるといい、$Y \subset X$とかく。

$Y \subset X$かつ$Y \neq X$のとき、$Y$は$X$の**真部分集合**であるといい、$Y \subsetneq X$とかく。

{{% /def %}}

## 注意

- 論理記号を用いて書けば、$$Y \subset X \iff \forall a \in Y, a \in X$$
- $Y \subset X$は$Y \subseteq X$ともかく。この記法を採用する場合、まれに$Y \subsetneq X$のことを単に$Y \subset X$とかくことがある。

## 参考文献
