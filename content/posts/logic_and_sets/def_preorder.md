---
title: 前順序
date: 2024-10-21
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

前順序の定義を解説します。

<!--more-->

## 前提知識

- [二項関係]({{< ref "def_binary_relation">}})

## 定義

{{% def "前順序 (preorder)" %}}
$\preceq$を集合$X$上の[二項関係]({{< ref "def_binary_relation">}})とする。
$\preceq$が以下を満たすとき、$X$上の**前順序**という。

1. $\forall x \in X, x \preceq x$
2. $\forall x, y, z \in X, x \preceq y \; かつ  \; y \preceq z \implies x \preceq z$

{{% /def %}}

## 注意

- 1の性質を**反射律**、2の性質を**推移律**という。

## 参考文献
