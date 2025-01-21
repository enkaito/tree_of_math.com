---
title: フェルマーの小定理
date: 2024-10-17
categories:
  - 代数学
  - 群論
tags:
  - 定理
draft: false
---

フェルマーの小定理について解説します。

<!--more-->

## 前提知識

- [ラグランジュの定理]({{< ref "thm_lagrange_theorem">}})

## 主張

{{% thm "フェルマーの小定理 (Fermat's little theorem)" %}}
$p$を素数とする。$a \in \mathbb{Z}$が$p$で割り切れないとき、$$a^{p-1} \equiv 1 \pmod{p}.$$

{{% /thm %}}

## 証明

上の主張は、「任意の$[a] \in (\mathbb{Z} / p \mathbb{Z})^{\times}$について$[a]^{p-1} = [1]$」と言い換えられる。
[Lagrangeの定理]({{< ref "thm_lagrange_theorem">}})より$[a]$の位数は$|(\mathbb{Z} / p \mathbb{Z})^{\times}|= p-1$の約数なので、確かに$[a]^{p-1} = [1]$である。

## 注意

- $p$は素数でないといけない。この条件は、$|(\mathbb{Z} / p \mathbb{Z})^{\times}|= p-1$のために必要である。
  - 実際に、例えば$(\mathbb{Z}/4\mathbb{Z})^{\times} = \lbrace |1|, |3| \rbrace$で、$|(\mathbb{Z} / 4 \mathbb{Z})^{\times}|= 2 \neq 4-1$
- $a$が$p$で割り切れるときは、もちろん$a^{p-1} \equiv 0 \pmod{p}.$
- 上のケースもまとめて、任意の$a$に対して$a^{p} \equiv a \pmod{p}.$

## 参考文献
