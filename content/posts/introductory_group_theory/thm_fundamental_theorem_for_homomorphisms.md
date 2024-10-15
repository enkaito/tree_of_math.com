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
$G, H$を群、$\phi: G \to H$を$G$から$H$への準同型写像とすると、

$$G / \mathrm{Ker}(\phi) \cong \mathrm{Im}(\phi)$$

{{% /thm %}}

## 注意

- $\mathrm{Ker}(\phi)$が$G$の正規部分群なので、商群$G / \mathrm{Ker}(\phi)$が定まること、$\mathrm{Im}(\phi)$が$H$の部分群なので、同型が意味をなすことに注意。

## 参考文献
