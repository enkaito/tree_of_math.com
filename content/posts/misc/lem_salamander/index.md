---
title: サラマンダーの補題
date: 2025-03-11T20:28:43+13:00
categories:
  - 
tags:
  - 補題 
draft: true
---

サラマンダーの補題とその証明について解説します。

<!--more-->

$$
\gdef\im{\operatorname{im}}
\gdef\rcp#1{{}^\square \! #1}
\gdef\don#1{#1_\square}
$$

## 記号の定義

{{% def %}}
二重複体の中の加群$A$に対して、以下のように記号を定義する。

<iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNyxbMSwxLCJBIl0sWzAsMSwiXFxidWxsZXQiXSxbMSwwLCJcXGJ1bGxldCJdLFswLDAsIlxcYnVsbGV0Il0sWzIsMSwiXFxidWxsZXQiXSxbMSwyLCJcXGJ1bGxldCJdLFsyLDIsIlxcYnVsbGV0Il0sWzEsMCwiYiIsMV0sWzIsMCwiYSIsMV0sWzMsMCwicCIsMV0sWzAsNCwiYyIsMV0sWzAsNSwiZCIsMV0sWzAsNiwicSIsMV1d&embed" width="432" height="432" style="border-radius: 8px; border: none;"></iframe>

- $A_= := \ker c / \im b$: $A$の水平ホモロジー
- $A_\| := \ker d / \im a$: $A$の垂直ホモロジー
- $\rcp A := (\ker c \cap \ker d) / \im p$: $A$でのreceptor
- $\don A := \ker q / (\im a + \im b)$: $A$でのdonor

{{% /def %}}

## 補題

{{% lem "The Intramural Maps" %}}
恒等写像$1_A: A \to A$は以下の可換図式を誘導する。

<iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwxLCJBX3tcXHx9Il0sWzEsMCwiXlxcc3F1YXJlIEEiXSxbMiwxLCJBXz0iXSxbMSwyLCJBX1xcc3F1YXJlIl0sWzEsMF0sWzEsMl0sWzIsM10sWzAsM11d&embed" width="432" height="432" style="border-radius: 8px; border: none;"></iframe>

可換図式に現れる4つの射を、$A$に関するintramural mapsという。
{{% /lem %}}

{{% lem "The Extramural Maps" %}}
二重複体に現れる射$f: A \to B$は射$\don A \to \rcp B$を誘導する。
この射を、$f$に関するextramural mapという。
{{% /lem %}}

## サラマンダーの補題

{{% lem "Salamander Lemma" %}}
二重複体において、水平射$A \to B$があり、$A$の上に$C$が、$B$の下に$D$があるとする。

{{< img src="salamander_assumption.svg" >}}

このとき、以下の列は完全。
ただし、両端の射はそれぞれ$\rcp A, \don B$を経由するようなintra/extramural map の合成。
$$\don{C} \xrightarrow{\rcp A} A_\| \to \don{A} \to \rcp{B} \to B_\| \xrightarrow{\don B} \rcp{D}$$

また、垂直射$A \to B$があり、$A$の左に$C$が、$B$の右に$D$がある時、以下の列は完全となる。
$$\don{C} \xrightarrow{\rcp A} A_= \to \don{A} \to \rcp{B} \to B_= \xrightarrow{\don B} \rcp{D}$$

{{% /lem %}}

## 名前について

得られる完全列を図に表すと以下のようになる。
矢印がサラマンダーに見えることが名前の由来と思われる。

{{< img src="salamander_hol.svg" >}}
{{< img src="salamander_vert.svg" >}}

## 参考文献
