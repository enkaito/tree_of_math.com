---
title: 和集合
date: 2024-10-19
author: Enklht
avatar: img/avatars/enklht.webp
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

和集合について解説します。

<!--more-->

## 前提知識

- [集合]({{< ref "def_set">}})

## 定義

{{% def "和集合 (union)" %}}
$X, Y$を集合とする。$X$か$Y$のいずれかに属する元の集合を$X$と$Y$の**和集合**といい、$X \cup Y$とかく。つまり、
$$X \cup Y := \set{x; x \in X \vee x \in Y}$$

より一般に、集合族$\mathcal{F}$に対し、集合族の集合のいずれかに属する元の集合を和集合といい、$\bigcup \mathcal{F}$とかく。つまり、
$$\bigcup \mathcal{F} := \set{x; \exists X \in \mathcal{F}, x \in X}$$

集合族$\cal{F}$が$\mathcal{F} = \set{X_\lambda}_{\lambda \in \Lambda}$と添字付けられている場合、和集合を$\bigcup_{\lambda \in \Lambda} X_\lambda$とかく。つまり、
$$\bigcup_{\lambda \in \Lambda} X_\lambda := \set{x; \exists \lambda \in \Lambda, x \in X_\lambda}$$

{{% /def %}}

## 注意

- 和集合は合併、結びとも呼ばれる。
- 記号$\cup$はカップと読むことがある。

## 参考文献
