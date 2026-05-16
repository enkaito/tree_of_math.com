---
title: 含意・同値
date: 2026-05-17
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

命題に対する演算、含意と同値の定義について解説します。

<!--more-->

## 前提知識

- [命題]({{< ref "def_proposition" >}})
- [述語]({{< ref "def_predicate" >}})

## 定義

{{% def "含意 (implication)・同値 (equivalence)" %}}
命題$P, Q$に対し、次の命題を**含意**・**同値**という。

- **含意** $P \to Q$：$P$が真ならば$Q$が真。
- **同値** $P \leftrightarrow Q$：$P \to Q$かつ$Q \to P$が成り立つ。

{{% /def %}}

## 注意

- $P \to Q$は「$P$ならば$Q$」と読む。
- $P \leftrightarrow Q$は「$P$と$Q$は同値」と読む。
- $P \to Q$は$\neg P \vee Q$と同値であり、日常語の「ならば」と完全には一致しない。
- $P \leftrightarrow Q$は$P$と$Q$の真偽が一致することを意味する。
  これは$P \oplus Q$の否定、すなわち負の排他的論理和と同じ。

## 参考文献
