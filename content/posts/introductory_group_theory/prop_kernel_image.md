---
title: 準同型写像の核・像
date: 2024-10-15
author: Enklht
avatar: img/avatars/enklht.webp
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

{{% prop 準同型写像の核は正規部分群 %}}
$\phi: G \to H$を準同型とする。このとき、集合
$$\ker(\phi) := \set{g \in G; \phi(g) = e_H}$$
を$\phi$の核という。$\ker(\phi)$は$G$の[正規部分群]({{< ref "def_normal_subgroup">}})である。

{{% /prop %}}

{{% prop 準同型写像の像は部分群 %}}
$\phi: G \to H$を準同型とする。このとき、集合
$$\mathrm{Im}(\phi) := \set{\phi(g); g \in G}$$
を$\phi$の像（より正確には、$\phi$による$G$の像）という。$\mathrm{Im}(\phi)$は$H$の[部分群]({{< ref "def_subgroup">}})である。

{{% /prop %}}

## 注意

- $\ker(\phi) \subset G, \mathrm{Im}(\phi) \subset H$なので、同じ群の部分群ではないこと注意。
- $\mathrm{Im}(\phi)$は$\phi(G)$ともかく。
- 核はカーネル、像はイメージとも呼ぶ。

## 参考文献
