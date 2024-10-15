---
title: 群の定義
date: 2024-08-22T19:09:29+09:00
lastmod: 2024-08-22T19:09:29+09:00
author: Author Name
# avatar: /img/author.jpg
# authorlink: https://author.site
# cover: /img/cover.jpg
# images:
#   - /img/cover.jpg
categories:
  - 代数学
tags:
  - 定義
# nolastmod: true
draft: false
---

群の定義について解説します。

<!--more-->

## 群の定義

{{% def 群 %}}
空でない集合$G$と、その上の二項演算$\cdot: G \times G \to G$が以下を満たすとき、$(G, \cdot)$は **群**であるという。

1. $\exists e \in G, \forall g \in G, g \cdot e = e \cdot g = g$
2. $\forall g \in G, \exists g^{-1} \in G, g \cdot g^{-1} = g^{-1} \cdot g = e $
3. $\forall g, h, k \in G, (g \cdot h) \cdot k = g \cdot (h \cdot k)$
{{% /def %}}

## 注意

- 演算$\cdot$が明確にわかるとき、省略して$G$は群であるいう。
- 条件1の元$e \in G$を群$G$の**単位元**という。実は、単位元は一意に定まる。
- 条件2から存在がわかる$g^{-1} \in G$を $g$ の**逆元**という。実は、逆元は$g$に対して一意に定まる。
- 条件3を**結合法則**という。

## 参考文献
