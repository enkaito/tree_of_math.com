---
title: ラグランジュの定理
date: 2024-10-16
categories:
  - 代数学
  - 群論
tags:
  - 定理
draft: false
---

ラグランジュの定理について解説します。

<!--more-->

## 前提知識

- [群の位数]({{< ref "def_order_group">}})
- [指数]({{< ref "def_index">}})
- [左、右剰余類]({{< ref "def_coset">}})

## 主張

{{% thm "ラグランジュの定理 (Lagrange's theorem)" %}}
$G$を群、$H$をその部分群とする。このとき、
$$|G| = [G:H] |H|$$
ただし、$|G|, |H|$はそれぞれ$G, H$の位数、$[G:H]$は（$G$における）$H$の指数である。

{{% /thm %}}

## 証明

$H$の左剰余類全体を$G/H$とする。
$G$は左剰余類の互いに素な和集合
$$G = \bigsqcup_{gH \in G/H} gH$$
に分解される。
任意の$g \in G$について、写像$H \to gH, h \mapsto gh$は全単射なので$|gH| = |H|$である。
したがって
$$|G| = \sum_{gH \in G/H} |gH| = [G:H]|H|$$
が成り立つ。

## 注意

- Lagrangeの定理から即座に以下がわかる。
  - $|G| < \infty$のとき、部分群$H$の位数$|H|$、指数$[G:H]$はともに$G$の位数$|G|$の約数である。
  - $|G| = \infty \iff [G:H] = \infty$または$|H| = \infty$。

## 参考文献
