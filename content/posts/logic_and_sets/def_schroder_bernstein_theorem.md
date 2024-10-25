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
$X, Y$を集合とする。２つの単射$f: X \to Y, g: Y \to X$が存在すれば、$X$から$Y$への全単射が存在する。

{{% /thm %}}

## 注意

- $X$から$Y$、$Y$から$X$に双方向Borelな単射が存在すれば、$X$から$Y$へのBorel同型が存在することもSchr&ouml;der-Bernsteinの定理と呼ぶことがある。証明は単なる写像の場合とほぼ同様となる。

## 参考文献
