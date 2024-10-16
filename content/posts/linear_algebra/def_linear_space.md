---
title: ベクトル空間の定義
date: 2024-08-24T16:46:02+09:00
author: Author Name
# avatar: /img/author.jpg
# authorlink: https://author.site
# cover: /img/cover.jpg
# images:
#   - /img/cover.jpg
categories:
  - 線形代数
tags:
  - 定義
# nodraft: false
---

ベクトル空間の定義について解説します。

<!--more-->

## ベクトル空間の定義

{{% def ベクトル空間 %}}
体 $K$, 集合 $V$, に対して加法 $V \times V \to V$, スカラー倍 $K \times V \to V$ が定義されていて以下の条件を満たすとき、$V$ は $K$上の**ベクトル空間**であるという。

1. $\forall x, y, z \in V, (x + y) + z = x + (y + z)$
2. $\forall x, y \in V, x + y = y + x$
3. $\exists\bm{0} \in V, \forall x \in V, x + \bm{0} = x$
4. $\forall x \in V, \exists -x \in V, x + (-x) = \bm{0}$
5. $\forall x \in V, \forall a, b \in K, (ab)x = a(bx)$
6. $\forall x \in V, 1x = x$
7. $\forall x, y \in V, \forall a \in K, a(x+y) =  ax + ay$
8. $\forall x \in V, \forall a, b \in K, (a+b)x = ax + bx$
{{% /def %}}

## 注意

- ベクトル空間の元をベクトルという。
- 3.の$\bm{0}$を零ベクトルという。
- 4.の$-x$を$x$の逆ベクトルという。

## 参考文献
