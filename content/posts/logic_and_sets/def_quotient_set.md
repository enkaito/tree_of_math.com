---
title: 同値類・商集合
date: 2024-10-15
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

商集合の定義を解説します。

<!--more-->

## 前提知識

- [同値関係の定義]({{< ref "def_equivalence">}})

## 定義

{{% def "同値類 (equivalence class)・商集合 (quotient set)" %}}
$\sim$を集合$X$上の[同値関係]({{< ref "def_equivalence">}})とする。
$x \in X$に対して、$X$の部分集合
$$[x] := \set{y \in X; x \sim y}$$
を$x$の**同値類**という。

また、同値類の集合
$$\set{[x]; x \in X}$$
を$X$の$\sim$による商集合といい、$X/\sim$とかく。

{{% /def %}}

## 注意

- $X/\sim$は$X$の「部分集合の集合」である。ところで、「集合の集合」をよく族と呼ぶ。この言葉を用いて、$X/\sim$は$X$の「部分集合の族」、あるいはより短く「部分集合族」ということも多ことも多い。

## 参考文献
