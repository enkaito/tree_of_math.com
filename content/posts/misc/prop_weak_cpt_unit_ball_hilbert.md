---
title: 可分Hilbert空間の閉単位球は弱コンパクト
date: 2025-01-26
categories:
  - 関数解析学
tags:
  - 命題
draft: false
---

可分Hilbert空間の閉単位球が弱コンパクトであることの対角線論法を用いた証明を紹介します。

<!--more-->

## 前提知識

- Hilbert空間
- 弱収束

## 主張

{{% prop %}}
可分Hilbert空間の閉単位球は弱位相でコンパクトである。

{{% /prop %}}

実際には、Banach-Alaogluの定理と、Hilbert空間は回帰的であることから、一般のHilbert空間について閉単位球は弱コンパクトであることが示せる。

## 証明

一般に、可分Banach空間の弱位相の閉単位球への制限は距離化可能であるため、点列コンパクト性を示せば良い。

$H$を可分Hilbert空間, $B$をその閉単位球とする。
$B$の点列$\{x_n\}_{n=1}^\infty$について、部分列$\{x_{n_k}\}$が存在して、任意の$v \in H$について$\langle x_{n_k}, v \rangle$が収束することを示す。

$\{e_n\}_{n=1}^\infty$を$H$の完全正規直行系とする。
Cauchy-Schwarzの不等式より、$\forall n \in \mathbb{N}, |\langle x_n, e_1\rangle| \le \| x_n \| \| e_1 \| \le 1$。
よって、$|\langle x_n, e_1\rangle|$が収束するように$\{x_n\}$の部分列$\{x_{n^1_k}\}$をとることができる。

このとき、$\forall k \in \mathbb{N}, |\langle x_{n^1_k}, e_2\rangle| \le 1$なので、$|\langle x_{n^1_k}, e_1\rangle|$が収束するように$\{x_{n^1_k}\}$の部分列$\{x_{n^2_k}\}$をとることができる。
これを繰り返して、部分列の列$\{x_{n^l_k}\}$を作る。

ここで、部分列$\{x_{n^k_k}\}$を考えると、途中から収束列の部分列となるため、任意の$l \in \mathbb{N}$に対して$\langle x_{n^k_k}, e_l\rangle$が収束する。
$a_l := \lim_{k \to \infty} \langle x_{n^k_k}, e_l \rangle$とし、$y := \sum_l a_l e_l$と定義する。 定義から、任意の$e_l$について、$\lim_{k \to \infty} \langle x_{n^k_k}, e_l \rangle = a_l = \langle y, e_l \rangle$。

$x_{n^k_k}$が$y$へ弱収束すること、すなわち、任意の$v \in H$について、$\langle x_{n^k_k}, v \rangle$が$\langle y, v \rangle$へ収束することを示す。
任意の$\epsilon > 0$に対して、
完全直行基底の稠密性より$\tilde{v} \in \textrm{span} \{e_l\}$を$\| v - \tilde{v} \| < \epsilon$と取れる。また、$\textrm{span} \{e_l\}$での収束より、$\exists N \in \mathbb{N}, k \ge N \implies | \langle x_{n^k_k} - y, \tilde{v} \rangle | < \epsilon$。
したがって、$k \ge N$で、

$$
\begin{split}
  |\langle x_{n^k_k} - y, v \rangle| &\le |\langle x_{n^k_k} - y, \tilde{v} \rangle| + |\langle x_{n^k_k}, v - \tilde{v} \rangle| + |\langle y, v-\tilde{v} \rangle| \\
  & \le \epsilon + \|x_{n^k_k} \| \epsilon + \| y \| \epsilon \\
  & \le (2 + \|y\|) \epsilon
\end{split}
$$

以上より、確かに$x_{n^k_k}$は$y$へ弱収束する。

## 参考文献
