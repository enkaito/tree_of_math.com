---
title: 写像
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

{{% def "写像 (map)" %}}
$X, Y$を集合とする。二項関係$f \subset X \times Y$について以下が成り立つとき、$f$を$X$から$Y$への**写像**といい、$f: X \to Y$とかく。
$$\forall x \in X, \exists! y \in Y, (x, y) \in f$$

各$x \in X$に対して一意的に存在する、$(x, y) \in f$を満たす$y \in Y$のことを$f(x)$とかく。

{{% /def %}}

## 注意

- 上では形式的に定義したが、結局写像$f: X \to Y$とは各$x \in X$について$y \in Y$が一つ定まっているような対応関係のことである。

## 参考文献
