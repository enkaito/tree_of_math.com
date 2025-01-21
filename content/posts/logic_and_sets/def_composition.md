---
title: 合成
date: 2024-10-20
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

合成ついて解説します。

<!--more-->

## 前提知識

- [写像]({{< ref "def_map">}})

## 定義

{{% def "合成 (composition)" %}}
写像$f: X \to Y, g: Y \to Z$に対し、$x \in X$を$g(f(x)) \in Z$へおくる写像を$f$と$g$の**合成**といい、$g \circ f$とかく。

{{% /def %}}

## 注意

- すべての2つの写像が合成できるわけではないことに注意。
- $f: X \to Y, g: Y' \to Z$が$Y \subset Y'$を満たすとき、$f$の終域を$Y'$だと思って合成写像$g \circ f$を考えることがある。

## 参考文献
