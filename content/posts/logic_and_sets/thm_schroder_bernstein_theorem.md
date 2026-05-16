---
title: シュレーダー・ベルンシュタインの定理
date: 2024-10-25
categories:
  - 論理と集合
tags:
  - 定理
draft: false
---

シュレーダー・ベルンシュタインの定理について解説します。

<!--more-->

## 前提知識

- [全射・単射・全単射]({{< ref "def_surjection_injection_bijection">}})

## 主張

{{% thm "シュレーダー・ベルンシュタインの定理 (Schröder-Bernstein theorem)" %}}
$X, Y$を集合とする。2つの単射$f: X \to Y, g: Y \to X$が存在すれば、$X$から$Y$への全単射が存在する。

{{% /thm %}}

## 証明

自然数$n$について、$A_0 = X \setminus g(Y), A_{n+1} = g(f(A_n))$により帰納的に集合$A_n$を定める。
また、$A = \bigcup_{n \ge 0} A_n$ とおく。
このとき、 $X \setminus A \subset X \setminus A_0 = g(Y)$、
$$
\begin{aligned}
 g(f(A)) &= g\left(f\left(\bigcup_{n \ge 0} A_n\right)\right) \\
          &= \bigcup_{n \ge 0} f(g(A_n)) \\
          &= \bigcup_{n \ge 1} A_n
\end{aligned}
$$
が成り立つ。

写像$h: X \to Y$を
$$
 h(x) = \begin{cases}
   f(x) & (x \in A), \\
   g^{-1}(x) & (x \in X \setminus A)
 \end{cases}
$$
で定める。
上の等式より$x \in X \setminus A$ならば$x \in g(Y)$で、$g$は単射なので$g^{-1}(x) \in Y \setminus f(A)$がただ一つ定まり、$h$はwell-definedである。
以下、$h: X \to Y$が全単射であることを示す。

$f$、定義域を$X \setminus A$としたときの$g^{-1}$は単射であり、もし$x \in A_n, x' \in X \setminus A$について$f(x) = g^{-1}(x')$が成り立ったとすると、$x' = g(f(x)) \in A_{n+1} \subset A$となり矛盾。
したがって、その様な$x, x'$は存在せず、$h$は単射である。

任意の$y \in Y$について、$y \in f(A)$なら$y = f(x)$となる$x \in A$が存在し$y = h(x)$である。
一方、$y \notin f(A)$なら$g(y) \notin g(f(A))$であり、また$g(y) \notin X \setminus g(Y) = A_0$なので$g(y) \notin \bigcup_{n \ge 1} A_n \cup A_0 = A$である。
つまり、$g(y) \in X \setminus A$なので$h(g(y)) = y$となる。
よって$h$は全射であり、$X$から$Y$への全単射が存在する。

## 注意

- この定理は単にBernsteinの定理とも呼ばれる。
- この定理から、$X$から$Y$へ全射と単射が存在すれば全単射が存在することもわかる。全射$f: X \to Y$があれば各$y \in Y$に対して$f^{-1}(\set{y})$を1つずつ選んで$Y$から$X$への単射を作れるからである。
- 同様に、2方向の全射から全単射を作ることもできる。
- 双方向Borelな単射$X \to Y, Y \to X$が存在すれば、$X$から$Y$へのBorel同型が存在することもSchr&ouml;der-Bernsteinの定理と呼ぶことがある。証明は単なる写像の場合とほぼ同様である。単射Borelではうまく行かないことに注意。

## 参考文献
