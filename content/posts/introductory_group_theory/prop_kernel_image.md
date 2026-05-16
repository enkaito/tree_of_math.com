---
title: 準同型写像の核・像
date: 2024-10-15
categories:
  - 代数学
  - 群論
tags:
  - 命題
draft: false
---

準同型定理の核・像についての命題を解説します。

<!--more-->

## 前提知識

- [部分群]({{< ref "def_subgroup">}})
- [正規部分群]({{< ref "def_normal_subgroup">}})
- [準同型写像]({{< ref "def_homomorphism">}})

## 主張

{{% prop "準同型写像の核 (kernel) は正規部分群" %}}
$\phi: G \to H$を準同型とする。
このとき、集合
$$\ker(\phi) := \set{g \in G; \phi(g) = e_H}$$
を$\phi$の核という。
$\ker(\phi)$は$G$の[正規部分群]({{< ref "def_normal_subgroup">}})である。

{{% /prop %}}

{{% prop "準同型写像の像 (image) は部分群" %}}
$\phi: G \to H$を準同型とする。
このとき、集合
$$\mathrm{im}(\phi) := \set{\phi(g); g \in G}$$
を$\phi$の像（より正確には、$\phi$による$G$の像）という。
$\mathrm{im}(\phi)$は$H$の[部分群]({{< ref "def_subgroup">}})である。

{{% /prop %}}

## 証明

### 準同型写像の核 (kernel) は正規部分群

$\ker(\phi)$が正規部分群であることを示す。
部分群の判定法を用いる。

$e_G \in G$について$\phi(e_G) = e_H$なので$e_G \in \ker(\phi)$である。
したがって$\ker(\phi)$は空でない。

$x, y \in \ker(\phi)$とすると$\phi(x) = \phi(y) = e_H$である。
したがって$\phi(xy^{-1}) = \phi(x)\phi(y)^{-1} = e_H$より$xy^{-1} \in \ker(\phi)$である。
よって$\ker(\phi)$は部分群である。

次に$g \in G, x \in \ker(\phi)$とすると
$$
\phi(gxg^{-1}) = \phi(g)\phi(x)\phi(g)^{-1} = \phi(g)e_H\phi(g)^{-1} = e_H
$$
より$gxg^{-1} \in \ker(\phi)$である。
したがって$\ker(\phi)$は正規部分群である。

### 準同型写像の像 (image) は部分群

$\mathrm{im}(\phi)$が部分群であることを示す。
部分群の判定法を用いる。

$e_H = \phi(e_G)$より$e_H \in \mathrm{im}(\phi)$である。
したがって$\mathrm{im}(\phi)$は空でない。

$y, z \in \mathrm{im}(\phi)$とすると、ある$a, b \in G$が存在して$y = \phi(a), z = \phi(b)$と書ける。
このとき
$$
 y z^{-1} = \phi(a)\phi(b)^{-1} = \phi(ab^{-1})
$$
より$yz^{-1} \in \mathrm{im}(\phi)$である。
したがって$\mathrm{im}(\phi)$は部分群である。

## 注意

- $\ker(\phi) \subset G, \mathrm{im}(\phi) \subset H$なので、同じ群の部分群ではないこと注意。
- $\mathrm{im}(\phi)$は$\phi(G)$ともかく。
- 英語をカタカナ読みして、核はカーネル、像はイメージと呼ぶこともある。

## 参考文献
