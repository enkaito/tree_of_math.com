---
title: $\mathbb{F}_p$上の既約多項式の個数
date: 2025-01-19
categories:
  - その他
tags:
  - 命題
draft: false
---

$$
\gdef\Fp{\mathbb{F}_p}
\gdef\FpX{\mathbb{F}_p[X]}
$$

素数位数の有限体$\Fp$上の既約多項式の個数について解説します。

<!--more-->

## 前提知識

- 既約多項式
- Euclidの互除法

## 主張

以下、$p$は素数とする。

{{% prop %}}
$\FpX$における$d$次monic既約多項式の個数を$n_p(d)$とおくと、

$$ p^n = \sum_{d \mid n} d \cdot n_p(d) $$

特に、$d$が素数の場合、

$$ n_p(d) = \frac{p^d - p}{d} $$

{{% /prop %}}

## 補題

{{% lem "既約多項式の生成するイデアルによる$\FpX$の商環は体" %}}
$f(X) \in \FpX$を次数$d$の既約多項式とし、$F := \FpX / (f(X))$とおく。$F$は位数$p^d$の体である。

{{% /lem %}}

{{% pf %}}
$f(X)$による割り算のあまりを考えることで、$F$の代表元は、$d-1$次以下とすることができる。
逆に、2つの$d-1$次以下の多項式の同値類は異なるため、$F$は位数$p^d$の環となる。

各$d-1$次以下の多項式$g(X) \neq 0$について、$f(X)$は既約より$\gcd(f(X), g(X)) = 1$である。  
$\therefore$ 多項式$p(X), q(X)$が存在して、$f(X) p(X) + g(X) q(X) = 1$とできる。  
$\therefore \overline{g(X)} \cdot \overline{q(X)}= 1 \text{ in } F$

以上で、$F$の$0$でない元について逆元の存在が示せたので、$F$は体である。

{{% /pf %}}

{{% lem "$\gcd(p^m-1, p^n-1) = p^{\gcd(m, n)} - 1$" %}}
任意の素数$p$、自然数$m, n$について、

$$\gcd(p^m-1, p^n-1) = p^{\gcd(m, n)} - 1$$
が成り立つ。

{{% /lem %}}

{{% pf %}}
$m \le n$として示す。
$n$を$m$で割った商を$q$、余りを$r$とすると、$n = m q + r$が成り立つ。

$$a := p^r (p^{(q-1)m} + p^{(q-2)m} + ... + p^m + 1)$$
とおくと、

$$
\begin{split}
  (p^m - 1) a + p^r - 1 &= p^r (p^{qm} - 1) + p^r - 1 \\
  &= p^{qm+r} - p^r + p^r - 1 \\
  &= p^n - 1
\end{split}
$$
$\therefore \gcd(p^m-1, p^n-1) = \gcd(p^m-1, p^r-1)$  

これを$r = 0$となるまで繰り返せば、Euclidの互除法より、

$$\gcd(p^m-1, p^n-1) = p^{\gcd(m, n)} - 1$$
とわかる。

{{% /pf %}}

## 証明

$q(X) := X^{p^n} - X$とおく。
$q(X)$が$n$を割り切る$d$次のmonic既約多項式を全て1回ずつ掛けて得られることを示す。
これが示せれば、次数を比較することにより結論を得る。

$K$を$q(X)$の分解体とすると、$p = 0 \text{ in } K$なので、$q(X)$の微分について
$q'(X) = p^n X^{p^n - 1} - 1 = -1 \neq 0 \text{ in } K$。
特に、$q(X)$は$K$で重根を持たない。
よって、$\FpX$に$q(X)$を2回割り切る多項式は存在しない。

$f(X)$を既約多項式とし、$d = \deg f$が$n$を割り切るとする。  
1つ目の補題より、$F := \FpX / (f(X))$は位数$p^d$の体なので、乗法群$\FpX^\times$についてのLagrangeの定理より、
$X^{p^d - 1} = 1 \text{ in } F.$  
よって、2つ目の補題より、$p^d - 1 \mid p^n - 1$なので、$X^{p^n - 1} = 1 \text { in } F$  
$\therefore f(X)  \mid X^{p^n - 1} - 1$  
$\therefore f(X)  \mid X^{p^n} - X = q(X)$  

$f(X)$を既約多項式とし、$d = \deg f$が$n$を割り切らないとする。
$f(X) \mid q(X)$と仮定し、矛盾を導く。
このとき、先ほどと同様に、任意の$a \in F^\times$について、
$a^{p^d - 1} = 1 \text{ in } F.$  
仮定より、$q(X) = 0 \text{ in } F$なので、
$a^{p^n} - a = 0 \text{ in } F$  
$\therefore a^{p^n - 1} = 1 \text{ in } F$  
$\therefore a^{\gcd(p^n - 1, p^d - 1)} - 1 = a^{p^{\gcd(d, n)} - 1} = 1 \text { in } F$  
したがって、$p^d - 1$未満次多項式$X^{p^{\gcd(d, n)}} - 1$が$p^d - 1$個の相異なる解を持つことになる。これは矛盾。
よって、次数$d \mid n$の既約多項式は$q(X)$を割り切らない。

以上より、 $q(X)$が$n$を割り切る$d$次のmonic既約多項式を全て1回ずつ掛けて得られることが示せた。

## 参考文献
