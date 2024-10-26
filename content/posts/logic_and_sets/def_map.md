---
title: 写像・定義域・終域
date: 2024-10-19
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

写像について解説します。

<!--more-->

## 前提知識

- [二項関係]({{< ref "def_binary_relation">}})

## 定義

{{% def "写像 (map)・定義域 (domain / source)・終域 (codomain / target)" %}}
$X, Y$を集合とする。二項関係$f \subset X \times Y$について以下が成り立つとき、$f$を$X$から$Y$への**写像**といい、$f: X \to Y$とかく。
$$\forall x \in X, \exists! y \in Y, (x, y) \in f$$

各$x \in X$に対して一意的に存在する、$(x, y) \in f$を満たす$y \in Y$のことを$f(x)$とかく。

写像$f: X \to Y$があるとき、$X$を$f$の**定義域**、$Y$を$f$の**終域**という。

{{% /def %}}

## 注意

- 上では形式的に定義したが、結局写像$f: X \to Y$とは各$x \in X$について$y \in Y$が1つ定まっているような対応関係のことである。
- 写像は関数とも呼ばれる。実数や複素数に値を取る写像を特に関数と呼び分けることもある。
- 写像が$x$を$y$へ送ることを、$x \mapsto y$とかいて表す。
- $X$から$Y$への写像の集合を$Y^{X}$とかく。
- $X$から$Y$への写像の数は、$X$の各元について$|Y|$通りの選択肢があるから、$|X|^{|Y|}$である。

## 参考文献
