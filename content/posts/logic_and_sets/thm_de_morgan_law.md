---
title: ド・モルガンの法則
date: 2026-05-17
categories:
  - 論理と集合
tags:
  - 定理
draft: false
---

ド・モルガンの法則について解説します。

<!--more-->

## 前提知識

- [命題]({{< ref "def_proposition" >}})
- [論理和・論理積・否定・排他的論理和]({{< ref "def_logical_connectives" >}})
- [含意・同値]({{< ref "def_implication_equivalence" >}})

## 主張

{{% thm "ド・モルガンの法則 (De Morgan's law)" %}}
命題$P, Q$について次が成り立つ。
$$
\neg (P \wedge Q) \leftrightarrow (\neg P \vee \neg Q),
\quad
\neg (P \vee Q) \leftrightarrow (\neg P \wedge \neg Q)
$$

{{% /thm %}}

## 証明

$P, Q$の真理値の4通りを調べる。
各場合で$\neg (P \wedge Q)$と$\neg P \vee \neg Q$の真理値が一致するので、$\neg (P \wedge Q) \leftrightarrow (\neg P \vee \neg Q)$が成り立つ。

$\neg (P \vee Q) \leftrightarrow (\neg P \wedge \neg Q)$も同様に示せる。

## 注意

- 量化子に対しても$\neg \forall x \in X, P(x) \leftrightarrow \exists x \in X, \neg P(x), \neg \exists x \in X, P(x) \leftrightarrow \forall x \in X, \neg P(x)$などの形で同様の法則が成り立つ。

## 参考文献
