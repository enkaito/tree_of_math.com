---
title: 準同型定理
date: 2024-10-15
categories:
  - 代数学
  - 群論
tags:
  - 定理
draft: false
---

準同型定理について解説します。

<!--more-->

## 前提知識

- [商群]({{< ref "def_quotient_group">}})
- [準同型写像]({{< ref "prop_subgroup_test">}})
- [準同型写像の核・像]({{< ref "prop_kernel_image">}})

## 主張

{{% thm "準同型写像 (fundamental theorem on homomorphisms)" %}}
$G, H$を群、$\phi: G \to H$を$G$から$H$への[準同型写像]({{< ref "def_homomorphism">}})とすると、
$$G / \ker(\phi) \cong \mathrm{im}(\phi)$$

{{% /thm %}}

## 証明

写像$\psi: G / \ker(\phi) \to \mathrm{Im}(\phi)$を
$$
 \psi([g]) = \phi(g)
$$
で定める。
まず$\psi$がwell-definedであることを示す。
$[g] = [g']$とすると$g^{-1}g' \in \ker(\phi)$である。
よって$\phi(g)^{-1}\phi(g') = \phi(g^{-1}g') = e_H$なので$\phi(g) = \phi(g')$である。
したがって$\psi$はwell-definedである。

次に$\psi$が準同型であることを示す。
任意の$g, g' \in G$について
$$
\psi([g][g']) = \psi([gg']) = \phi(gg') = \phi(g)\phi(g') = \psi([g])\psi([g'])
$$
が成り立つ。
よって$\psi$は準同型である。

次に$\psi$が単射であることを示す。
$\psi([g]) = e_H$とすると$\phi(g) = e_H$であり、$g \in \ker(\phi)$である。
したがって$[g] = [e_G]$である。
よって$\ker(\psi) = \set{[e_G]}$であり、[準同型写像が単射である条件]({{< ref "prop_kernel_injective">}})より$\psi$は単射である。

最後に全射性を示す。
任意の$y \in \mathrm{Im}(\phi)$について、ある$g \in G$が存在して$y = \phi(g)$と書ける。
このとき$y = \psi([g])$である。
よって$\psi$は全射である。
以上より$\psi$は同型であり、$G / \ker(\phi) \cong \mathrm{im}(\phi)$が成り立つ。

## 注意

- $\ker(\phi)$が$G$の[正規部分群]({{< ref "def_normal_subgroup">}})なので[商群]({{< ref "def_quotient_group">}})$G / \ker(\phi)$が定まること、$\mathrm{im}(\phi)$が$H$の部分群なので同型が意味をなすことに注意。
- 準同型定理という名前だが、**同型**の構成を主張する定理である。
- 準同型定理は第一同型定理とも呼ばれる。第二、第三同型定理もあり、よく知られている。
  まれに対応定理のことを第四同型定理と呼ぶこともある。

## 参考文献
