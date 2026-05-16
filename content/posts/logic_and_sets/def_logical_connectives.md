---
title: 論理和・論理積・否定・排他的論理和
date: 2026-05-17
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

命題に対する演算、論理和、論理積、否定の定義について解説します。

<!--more-->

## 前提知識

- [命題]({{< ref "def_proposition" >}})
- [述語]({{< ref "def_predicate" >}})

## 定義

{{% def "論理和 (disjunction)・論理積 (conjunction)・否定 (negation)・排他的論理和 (exclusive or)" %}}
命題$P, Q$に対し、次の命題を**論理和**・**論理積**・**否定**・**排他的論理和**という。

- **論理和** $P \vee Q$：$P$または$Q$の少なくとも一方が真のときに真。
- **論理積** $P \wedge Q$：$P$と$Q$がともに真のときに真。
- **否定** $\neg P$：$P$が偽のときに真。
- **排他的論理和** $P \oplus Q$：$P, Q$のうちちょうど一方が真のときに真。

{{% /def %}}

## 注意

- $\vee$は「または」、$\wedge$は「かつ」と読む。
- 否定は$\neg P$のほかに$\lnot P$と書くこともある。
- $\TeX$では$\vee, \wedge, \neg, \oplus$はそれぞれ`\vee`、`\wedge`、`\neg`、`\oplus`で表示することができる。

## 参考文献
