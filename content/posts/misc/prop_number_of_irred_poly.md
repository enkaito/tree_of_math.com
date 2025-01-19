---
title: $\mathbb{F}_p$上の既約多項式の個数
date: 2025-01-19
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - その他
tags:
  - 命題
draft: true
---

$$
\newcommand{\Fp}{\mathbb{F}_p}
\newcommand{\FpX}{\mathbb{F}_p[X]}
$$

素数位数の有限体$\Fp$上の既約多項式の個数について解説します。

<!--more-->

## 前提知識

- 既約多項式
- Euclidの互除法

## 主張

以下、$p$は素数とする。

## 補題

{{% lem "既約多項式の生成するイデアルによる$\FpX$の商環は体になる" %}}

$f(X) \in \FpX$を次数$d$の既約多項式とし、$F := \FpX / (f(X))$とおく。

$f(X)$による割り算のあまりを考えることで、$F$の代表元は、$d-1$次以下とすることができる。逆に、2つの$d-1$次以下の多項式の同値類は異なるため、$F$は次数$p^d$の環となる。

各$$

{{% /lem %}}

## 参考文献
