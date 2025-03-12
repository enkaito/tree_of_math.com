---
title: サラマンダーの補題
date: 2025-03-11T20:28:43+13:00
categories:
  - 
tags:
  - 補題 
draft: false
---

サラマンダーの補題と対象が元を持つ場合の証明を紹介します。

<!--more-->

$$
\gdef\im{\operatorname{im}}
\gdef\rcp#1{{}^\square \! #1}
\gdef\don#1{#1_\square}
$$

## 記号の定義

{{% def %}}
二重複体の中の加群$A$に対して、以下のように記号を定義する。

{{< img src="definitions.svg" >}}

- $A_= := \ker c / \im b$: $A$での水平ホモロジー
- $A_\| := \ker d / \im a$: $A$での垂直ホモロジー
- $\rcp A := (\ker c \cap \ker d) / \im p$: $A$でのreceptor
- $\don A := \ker q / (\im a + \im b)$: $A$でのdonor

ただし、$p, q$は二重複体に現れる射の合成で得られるものとする。

{{% /def %}}

## 補題

{{% lem "The Intramural Maps" %}}
恒等写像$1_A: A \to A$は以下の可換図式を誘導する。
可換図式に現れる4つの射を、$A$に関するintramural mapsという。

{{< img src="intramural_maps.svg" >}}

{{% /lem %}}

{{% pf %}}
$$
\begin{align*}
  (\ker c \cap \ker d) &\subset \ker d &&\subset \ker q \\
  \im p &\subset \im a &&\subset (\im a + \im b)
\end{align*}
$$
より、$\rcp A \to A_= \to \don A$はwell-defined.

同様に、
$$
\begin{align*}
  (\ker c \cap \ker d) &\subset \ker c &&\subset \ker q \\
  \im p &\subset \im b &&\subset (\im a + \im b)
\end{align*}
$$
より、$\rcp A \to A_\| \to \don A$はwell-defined.

{{% /pf %}}

{{% lem "The Extramural Maps" %}}
二重複体に現れる射$f: A \to B$は射$\don A \to \rcp B$を誘導する。
この射を、$f$に関するextramural mapという。

{{< img src="extramural_maps.svg" >}}

{{% /lem %}}

{{% pf %}}

$f$が水平射の場合を示す。下図のように射に名前をつける。

{{< img src="extramural_pf.svg" >}}

このとき、
$$
\begin{align*}
  \don A &:= \ker q / (\im a + \im b) \\
  \rcp B &:= (\ker c \cap \ker d) / \im p
\end{align*}
$$
である。

$\forall x \in \ker q$について、

- 二重複体で隣り合う射の合成は0写像なので、$cf = 0$。よって$f(x) \in \ker c$。
- $q = df$かつ$x \in \ker q$より、$f(x) \in \ker d$。

したがって、$f(x) \in \ker c \cap \ker d$。

$\forall x \in \im a, \forall y \in \im b$について、

- $p = fa$より$f(x) \in \im p$。
- $fb = 0$より$f(y) = 0$。

したがって、$f(x + y) = f(x) \in \im p$。

以上より、$x + (\im a + \im b) \mapsto f(x) + \im p$により射$\rcp{A} \to \don{B}$を定義できる。

{{% /pf %}}

## サラマンダーの補題

{{% lem "Salamander Lemma" %}}
二重複体において、水平射$A \to B$があり、$A$の上に$C$が、$B$の下に$D$があるとする。

{{< img src="salamander_assumption.svg" >}}

このとき、以下の列は完全。
ただし、両端の射はそれぞれ$\rcp A, \don B$を経由するようなintra/extramural map の合成。
$$\don{C} \xrightarrow{\rcp A} A_= \to \don{A} \to \rcp{B} \to B_= \xrightarrow{\don B} \rcp{D}$$

また、垂直射$A \to B$があり、$A$の左に$C$が、$B$の右に$D$がある時、以下の列は完全となる。
$$\don{C} \xrightarrow{\rcp A} A_\| \to \don{A} \to \rcp{B} \to B_\| \xrightarrow{\don B} \rcp{D}$$

{{% /lem %}}

{{% pf %}}

水平射の場合を示す。
下図のように射に名前をつける。

{{< img src="salamander_pf.svg" >}}

- $\forall x \in \ker p$について、$a(x) \in \im a + \im b$より、
  $$\im (\don C \to A_=) \subset \ker(A_= \to \don A)$$
- $\forall x \in \ker f$について、$x \in \im a + \im b$とすると、
  $\exists x' \in \im a$ s.t. $x - x' \in \im b$。
  すると、$fb = 0$より、$f(x) - f(x') = f(x - x') = 0$。
  $x' \in \im a$より$\exists y \in C$ s.t. $a(y) =  x'$。
  このとき、$p(y) = fa(y) = f(x') = f(x) = 0$。
  したがって、
  $$\im (\don C \to A_=) \supset \ker(A_= \to \don A)$$

- $A_= = \ker f / \im b$より、以下は明らか。
  $$\im (A_= \to \don A) \subset \ker (\don A \to \rcp B)$$
- $x \in \ker q$が$f(x) \in \im p$を満たすとすると、
  $\exists y \in C$ s.t. $p(y) = fa(y) = f(x)$。
  よって、$x' = x - a(y)$と置くと、$x' \in \ker f$かつ$x - x' = a(y) \in \im a + \im b$より、
  $$\im (A_= \to \don A) \supset \ker (\don A \to \rcp B)$$

- $\forall x \in \ker q, f(x) \in \im f$より、
  $$\im(\don A \to \rcp B) \subset \ker(\rcp B \to B_=)$$
- $\forall x \in \ker c \cap \ker d$が$x \in \im f$を満たすとき、$\exists y \in A, f(x) = x$であるが、$q(y) = c(x) = 0$より、$y \in \ker q$。
  $$\im(\don A \to \rcp B) \supset \ker(\rcp B \to B_=)$$

- $\forall x \in \ker c \cap \ker d$ について、$c(x) = 0$より、
  $$\im(\rcp B \to B_=) \subset \ker(B_= \to \rcp D)$$
- $x \in \ker d$について、$cx \in \im q$の場合、
  $\exists y \in A$ s.t. $q(y) = cf(y) = c(x)$。
  よって、$x' := x - f(y)$とおくと、$x - x' \in \im f$かつ$x' \in \ker c$。
  さらに、$d(x') = d(x) - df(y) = 0$なので、$x' \in \ker d$。
  つまり、$x' = \ker c \cap \ker d$である。
  したがって、
  $$\im(\rcp B \to B_=) \supset \ker(B_= \to \rcp D)$$

{{% /pf %}}

## 系

{{% cor %}}
下図で$A, B$において水平射が完全ならば、その誘導する extramural maps $\don A \to \rcp B$は同型。

{{< img src="salamander_cor1.svg">}}

同様に、$A, B$において垂直射が完全ならば、その誘導する extramural maps $\don A \to \rcp B$は同型。

{{% /cor %}}

{{% pf %}}
水平射の場合を示す。
仮定より、$A_= = 0, B_= = 0$。これと salamander lemma より、以下の完全列を得る。

$$0 \to \don{A} \to \rcp{B} \to 0$$

したがって、射$\don A \to \rcp B$は同型となる。

{{% /pf %}}

## 名前について

Salamander lemma で得られる完全列を図に表すと以下のようになる。
矢印がサラマンダーに見えることが名前の由来と思われる。

{{< img src="salamander_hol.svg" >}}
{{< img src="salamander_vert.svg" >}}

## 参考文献

- [On diagram-chasing in double complexes (arXiv)](https://arxiv.org/abs/1108.0958)
