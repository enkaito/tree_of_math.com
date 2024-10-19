---
title: 補集合
date: 2024-10-18
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

補集合について解説します。

<!--more-->

## 前提知識

- [集合]({{< ref "def_set">}})
- [部分集合]({{< ref "def_subset">}})

## 定義

{{% def "補集合 (complement)" %}}
$U$を集合、$X$を$U$の部分集合とする。$X$に属さない$U$の元の集合を、$U$に関する$X$の**補集合**といい、$X^{c}$や$\overline{X}$とかく。つまり、
$$X^{c} := \set{a \in U; a \notin X}$$

{{% /def %}}

## 注意

- 上の文脈で、$U$を全体集合と呼ぶ。文脈からわかる場合、$U$の説明は省略することが多い。
- $X^{c}$は差集合$U \setminus X$と同じものであるが、$U$を全体と考えている点でニュアンスが違う。一度固定した$U$を取り替えることは少ない。

## 参考文献
