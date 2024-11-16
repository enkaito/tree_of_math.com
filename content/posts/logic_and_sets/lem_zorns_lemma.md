---
title: ツォルンの補題
date: 2024-10-26
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 補題
draft: false
---

ツォルンの補題について解説します。

<!--more-->

## 前提知識

- [半順序]({{< ref "def_partial_order">}})
- [全順序]({{< ref "def_total_order">}})
- [選択公理]

## 定義

{{% lem "ツォルンの補題 (Zorn's lemma)" %}}
$(X, \preceq)$を以下の条件を満たす[半順序集合]({{< ref "def_partial_order">}})とする。

> 任意の全順序部分集合$\mathcal{T} \subset X$に対して、「$\forall t \in \mathcal{T}, t \preceq x_\mathcal{T}$」を満たす$x_\mathcal{T} \in X$が存在する。

このとき、任意の$y \in X$に対して$y \preceq x$を満たす$X$の極大元$x \in X$が存在する。

{{% /lem %}}

## 注意

- ある性質を満たす集合族（例：イデアル）の中に極大なものが存在することの証明によく用いられる。このとき、全順序部分集合の極大元としてそれらの和集合を取るということが多い。この場合、和集合が性質を満たしていること（上で言う$X$の元であること）を示す必要があることに注意。
- Zornの補題として、条件を満たす半順序集合が極大元を持つという主張を採用することも多い。
- Zornの補題は（ZFの下で）選択公理と同値である他、整列可能定理やTukey（テューキー・タッキー）の補題、「任意のベクトル空間には基底が存在する」という主張などとの同値性が知られている。

## 参考文献
