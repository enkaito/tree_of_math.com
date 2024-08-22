---
title: 単位元の一意性
date: 2024-08-22T19:09:29+09:00
lastmod: 2024-08-22T19:09:29+09:00
author: Author Name
# avatar: /img/author.jpg
# authorlink: https://author.site
# cover: /img/cover.jpg
# images:
#   - /img/cover.jpg
categories:
  - 代数学
tags:
  - 定義
# nolastmod: true
draft: false
---

本稿では、群の単位元が一意に定まることを解説する。

<!--more-->

## 主張
{{% thm 群の単位元の一意性 %}}
群 $G$ の単位元は一つしかない。すなわち、
$e, e' \in G$ がともに群 $G$ の単位元とすると、$e = e'.$
{{% /thm %}}

## 証明
$e, e'$ がともに $G$ の単位元であったとすると、単位元の満たすべき性質より、
$$
  \forall g \in G, ge = g, \\
  \forall h \in G, e'h = h.
$$
ここで、$g = e', h = e$とすれば、
$$
  e'e = e', \\
  e'e = e.
$$
左辺が等しいので、$e = e'$ が成り立つ。

## 注意
- 群に限らず、環、体等の単位元も同様の理由で一意に定まる。

## 参考文献