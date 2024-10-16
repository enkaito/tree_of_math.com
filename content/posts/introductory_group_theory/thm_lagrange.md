---
title: ラグランジュの定理
date: 2024-10-16
author: Enklht
avatar: img/avatars/enklht.webp
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

## 主張

{{% thm ラグランジュの定理 %}}
$G$を群、$H$をその部分群とする。このとき、
$$|G| = [G:H] |H|$$
ただし、$|G|, |H|$はそれぞれ$G, H$の位数、$[G:H]$は（$G$における）$H$の指数である。

{{% /thm %}}

## 注意

- ラグランジュの定理から即座に、**部分群$H$の位数$|H|$、指数$[G:H]$はともに$G$の位数$|G|$の約数である**ことがわかる。

## 参考文献
