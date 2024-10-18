---
title: 群
date: 2024-08-22T19:09:29+09:00
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 代数学
  - 群論
tags:
  - 定義
draft: false
---

群の定義について解説します。

<!--more-->

## 定義

{{% def "群 (group)" %}}
空でない集合$G$と、その上の二項演算$\cdot: G \times G \to G$が以下を満たすとき、$(G, \cdot)$は **群**であるという。

1. $\exists e \in G, \forall g \in G, g \cdot e = e \cdot g = g$
2. $\forall g \in G, \exists g^{-1} \in G, g \cdot g^{-1} = g^{-1} \cdot g = e $
3. $\forall g, h, k \in G, (g \cdot h) \cdot k = g \cdot (h \cdot k)$
{{% /def %}}

## 注意

- 演算$\cdot$が明確にわかるとき、省略して$G$は群であるいう。
- 演算子$\cdot$を書かず、単に並べて書くことで演算結果を表すことも多い。
- 群の演算のことをを積、掛け算と呼ぶことも多い。演算が可換の場合は和、足し算とも呼ばれる。
- 上に上げた3つの条件を**群の公理**という。
- 条件1の元$e \in G$を群$G$の**単位元**という。実は、[単位元は一意に定まる]({{< ref "thm_uniqueness_unit">}})。
- 条件2から存在がわかる$g^{-1} \in G$を $g$ の**逆元**という。実は、[逆元は$g$に対して一意に定まる]({{< ref "thm_uniqueness_inverse">}})。
- 条件3を**結合法則**という。
- 特に断りなく$e$や$1$を話題となっている群の単位元のこととすることがある。また、$e_G, 1_G$のように、どの群の単位元かを下付き添字により明確にすることもある。

## 参考文献
