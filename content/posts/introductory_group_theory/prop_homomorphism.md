---
title: 準同型写像の性質
date: 2024-10-16
categories:
  - 代数学
  - 群論
tags:
  - 命題
draft: false
---

準同型写像による単位元や逆元の行き先について解説します。

<!--more-->

## 前提知識

- [準同型写像]({{< ref "def_homomorphism">}})

## 主張

{{% prop 準同型写像による単位元の行き先は単位元 %}}
$G, H$を群、$\phi: G \to H$を準同型写像とすると、
$$\phi(e_G) = e_H$$
{{% /prop %}}

{{% prop 準同型写像による逆元の行き先は逆元 %}}
$G,BH$を群、$\phi: G \to H$を準同型写像とすると、
$$\forall g \in G, \phi(g^{-1}) = \phi(g)^{-1}$$
{{% /prop %}}

## 証明

### 準同型写像による単位元の行き先は単位元

準同型写像の定義より、
$$
\begin{equation}
  \begin{split}
    \phi(e_G) \phi(g) = \phi(e_G g) = \phi(g), \\
    \phi(g) \phi(e_G) = \phi(g e_G) = \phi(g).
  \end{split}
\end{equation}
$$
したがって、$\phi(e_G)$は$H$の単位元である。
[単位元の一意性]({{< ref "thm_uniqueness_unit">}})より、$\phi(e_G) = e_H$である。

### 準同型写像による逆元の行き先は逆元

任意の$g \in G$について、
準同型写像の定義、準同型による単位元の行き先は単位元より、
$$
\begin{equation}
  \begin{split}
    \phi(g^{-1}) \phi(g) = \phi(g^{-1} g) = \phi(e_G) = e_H, \\
    \phi(g) \phi(g^{-1}) = \phi(g g^{-1}) = \phi(e_G) = e_H.
  \end{split}
\end{equation}
$$
したがって、$\phi(g^{-1})$は$g$の単位元である。
[逆元の一意性]({{< ref "thm_uniqueness_inverse">}})より、$\phi(g^{-1}) = \phi(g)^{-1}$である。

## 注意

## 参考文献
