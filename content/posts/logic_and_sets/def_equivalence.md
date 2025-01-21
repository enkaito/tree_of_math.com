---
title: 同値関係
date: 2024-08-27T14:25:47+09:00
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

同値関係の定義を説明します。

<!--more-->

## 定義

{{% def "同値関係 (equivalence relation)" %}}
集合$X$上の二項関係 $R \subset X \times X$ が以下の三条件を満たすとき、 $R$ は $X$ 上の**同値関係**であるという。

1. $\forall x \in X, xRx$
2. $\forall x, y \in X, xRy \implies yRx$
3. $\forall x, y, z \in X, xRy \land yRz \implies xRz$
{{% /def %}}

## 注意

- 1.を**反射律**と呼ぶ。
- 2.を**対称律**と呼ぶ。
- 3.を**推移律**と呼ぶ。

## 参考文献
