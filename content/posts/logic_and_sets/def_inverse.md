---
title: 逆写像
date: 2024-10-20
categories:
  - 論理と集合
tags:
  - 定義
draft: false
---

逆写像について解説します。

<!--more-->

## 前提知識

- [写像]({{< ref "def_map">}})
- [全射・単射・全単射]({{< ref "def_inverse">}})
- [合成]({{< ref "def_composition">}})

## 定義

{{% def "逆写像 (inverse)" %}}
写像$f: X \to Y$に対し、
$$g \circ f = \mathrm{id}_X, f \circ g = \mathrm{id}_Y$$
満たす写像$g: Y \to X$があれば、それを$f$の**逆写像**とよび、$f^{-1}$とかく。

{{% /def %}}

## 注意

- 全単射な写像は必ず逆写像を持つ。

## 参考文献
