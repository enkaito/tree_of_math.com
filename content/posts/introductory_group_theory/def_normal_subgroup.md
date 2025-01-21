---
title: 正規部分群
date: 2024-10-15
categories:
  - 代数学
  - 群論
tags:
  - 定義
draft: false
---

正規部分群の定義を解説します。

<!--more-->

## 前提知識

- [部分群の定義]({{< ref "def_subgroup">}})

## 定義

{{% def "正規部分群 (normal subgroup)" %}}
$G$を群とする。$G$の[**部分群**]({{< ref "def_subgroup">}})$N$が以下の条件を満たすとき、$N$は$G$の**正規部分群**であるといい、$N \triangleleft G$とかく。

$$\forall g \in G, \forall n \in N, gng^{-1} \in N$$

{{% /def %}}

## 注意

上の条件で、$g$は$G$の任意の元であることに注意。$g \in N$の場合は、$N$が部分群であるため$\forall n \in N, gng^{-1} \in N$は必ず成り立つ。

また、上の条件は
$$\forall g \in G, gNg^{-1} \subset N$$
ともかける。

アーベル群（演算が可換な群）の場合、任意の部分群は正規部分群となる。実際、$H$が$G$の部分群ならば、任意の$g \in G, h \in H$について、
$$ghg^{-1} = hgg^{-1} = h \in H$$

## 参考文献
