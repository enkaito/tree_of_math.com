---
title: 全射・単射・全単射
date: 2024-10-20
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

全射・単射・全単射について解説します。

<!--more-->

## 前提知識

- [写像]({{< ref "def_map">}})

## 定義

{{% def "全射 (surjection)・単射 (injection)・全単射 (bijection)" %}}
写像$f: X \to Y$について、

- $\forall y \in Y, \exists x \in X, f(x) = y$が成り立つとき、$f$は**全射**という。
- $f(x) = f(x') \implies x = x'$が成り立つとき、$f$は**単射**という。
- $f$が全射かつ単射のとき、$f$は**全単射**という。

{{% /def %}}

## 注意

- 写像が全射であることの証明は、任意の$y \in Y$に対して$f(x)$を満たす$x \in X$を見つける（作る）ことで行うことが多い。
- 写像が単射であることの証明は、任意の$f(x) = f(x')$を仮定して、$x = x'$を示すことで行うことが多い。
- $X, Y$が有限集合で、濃度（元の個数）が等しい場合、$f: X \to Y$が単射ならば全射、全射ならば単射である。

## 参考文献
