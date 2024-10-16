---
title: 生成された部分群の定義
date: 2024-10-17
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 代数学
  - 群論
tags:
  - 定義
draft: false
---

生成された部分群の定義を説明します。

<!--more-->

## 前提知識

- [部分群]({{< ref "def_subgroup">}})
- [部分群の共通部分は部分群]({{< ref "thm_subgroup_intersection">}})

## 定義

{{% def 生成された部分群 %}}
群$G$の部分集合$S$に対して、すべての$S$を含む$G$の部分集合の共通部分を **$S$によって生成された$G$の部分群**とよび、$\langle S \rangle$とかく。つまり、
$$\langle S \rangle \colonequals \bigcap \set{H; HはGの部分群でSを含む。}.$$

特に、$S$が有限で、$S = \set{g_1, g_2, ..., g_n}$のとき、$S$の生成する部分群を$\langle g_1, g_2, ..., g_n \rangle$とかく。

{{% /def %}}

## 注意

- $G$は$G$の部分群なので、共通部分を取る集合族は空でなく、部分群の共通部分は必ず部分群なので、確かに定義の集合は部分群になっている。
- $\langle S \rangle$は$S$を含む$G$の最小の部分群である。特に、$S$が部分群のとき、$\langle H \rangle = H$となる。
- 一つの元$g \in G$によって生成された群$\langle g \rangle$は、具体的には$\set{g^i; i \in \mathbb{N}}$とかける。（今、$\mathrm{N}$は$0$を含むという立場をとっている。）これは一見無限群のようだが、$g^i = e$となる$i$が存在すれば、周期$i$の繰り返しが起きて実際には有限群となる。最小周期が$\langle g \rangle$の位数に一致し、$g$の位数と呼ばれる。

## 参考文献
