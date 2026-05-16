---
title: 準同型写像が単射である条件
date: 2026-05-17
categories:
  - 代数学
  - 群論
tags:
  - 命題
draft: false
---

準同型写像が単射であることと核が自明であることが同値であるという命題を解説します。

<!--more-->

## 前提知識

- [準同型写像]({{< ref "def_homomorphism">}})
- [準同型写像の核・像]({{< ref "prop_kernel_image">}})

## 主張

{{% prop "準同型写像が単射である条件" %}}
$G, H$を群、$\phi: G \to H$を準同型写像とする。
このとき、$\phi$が単射であることと$\ker(\phi) = \set{e_G}$は同値である。
{{% /prop %}}

## 証明

まず$\phi$が単射であると仮定する。
$g \in \ker(\phi)$とすると$\phi(g) = e_H = \phi(e_G)$である。
単射性より$g = e_G$となる。
よって$\ker(\phi) = \set{e_G}$である。

次に$\ker(\phi) = \set{e_G}$と仮定する。
$\phi(g) = \phi(g')$とすると$\phi(g^{-1}g') = e_H$である。
したがって$g^{-1}g' \in \ker(\phi)$より$g^{-1}g' = e_G$である。
よって$g = g'$となり、$\phi$は単射である。

## 注意

## 参考文献
