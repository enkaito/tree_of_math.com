---
title: 左、右剰余類
date: 2024-10-16
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 代数学
  - 群論
tags:
  - 定義
draft: false
---

左、右剰余類について解説します。

<!--more-->

## 前提知識

- [部分群]({{< ref "def_subgroup">}})
- [同値類・商集合]({{< ref "def_quotient_set">}})

## 定義

{{% def "左剰余類 (left coset)" %}}
$G$を群、$H$を$G$の部分群とする。$G$上の関係$\sim$を
$$g \sim g' :\iff g^{-1}g' \in H$$
により定めると、$\sim$は同値関係となる。

$\sim$による$G$の商集合を$G/H$とかく。また、$g\in G$の同値類$[g]$を$gH$とき、$g$の**左剰余類**という。

{{% /def %}}

{{% def "右剰余類 (right coset)"%}}
$G$を群、$H$を$G$の部分群とする。$G$上の関係$\sim$を
$$g \sim g' :\iff gg'^{-1} \in H$$
により定めると、$\sim$は同値関係となる。

$\sim$による$G$の商集合を$H\backslash G$とかく。また、$g\in G$の同値類$[g]$を$Hg$とかき、$g$の**右剰余類**という。

{{% /def %}}

## 注意

- $H$が正規部分ではない場合、$G/H$や$H \backslash G$に演算はうまく引き継がれないことに注意。特に両者は**群にならない**。
- 正規部分群の場合には左右剰余類が一致し、商集合も一致する。

## 参考文献
