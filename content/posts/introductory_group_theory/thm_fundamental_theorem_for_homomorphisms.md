---
title: 準同型定理
date: 2024-10-15
lastmod: 2024-10-15
author: Author Name
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

{{% thm 準同型写像 %}}
$G, H$を群、$\phi: G \to H$を$G$から$H$への[準同型写像]({{< ref "def_homomorphism">}})とすると、

$$G / \mathrm{Ker}(\phi) \cong \mathrm{Im}(\phi)$$

{{% /thm %}}

## 注意

- $\mathrm{Ker}(\phi)$が$G$の正規部分群なので商群$G / \mathrm{Ker}(\phi)$が定まること、$\mathrm{Im}(\phi)$が$H$の部分群なので同型が意味をなすことに注意。
- 準同型定理という名前だが、その内容は**同型**を示す定理である。
- 準同型定理は第一同型定理とも呼ばれる。第二、第三同型定理もあり、よく知られている。まれに対応定理のことを第四同型定理と呼ぶこともある。

## 参考文献
