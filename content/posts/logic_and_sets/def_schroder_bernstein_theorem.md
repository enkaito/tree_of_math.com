---
title: シュレーダー・ベルンシュタインの定理
date: 2024-10-25
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

シュレーダー・ベルンシュタインの定理について解説します。

<!--more-->

## 前提知識

- [全射・単射・全単射]({{< ref "def_surjection_injection_bijection">}})

## 定義

{{% thm "シュレーダー・ベルンシュタインの定理 (Schr&ouml;der-Bernstein theorem)" %}}
$X, Y$を集合とする。2つの単射$f: X \to Y, g: Y \to X$が存在すれば、$X$から$Y$への全単射が存在する。

{{% /thm %}}

## 注意

- この定理は単にBernsteinの定理とも呼ばれる。
- この定理から、$X$から$Y$へ全射と単射が存在すれば全単射が存在することもわかる。全射$f: X \to Y$があれば各$y \in Y$に対して$f^{-1}(\set{y})$を1つずつ選んで$Y$から$X$への単射を作れるからである。
- 同様に、2方向の全射から全単射を作ることもできる。
- $X$から$Y$、$Y$から$X$に双方向Borelな単射が存在すれば、$X$から$Y$へのBorel同型が存在することもSchr&ouml;der-Bernsteinの定理と呼ぶことがある。証明は単なる写像の場合とほぼ同様である。

## 参考文献
