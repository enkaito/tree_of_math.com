---
title: 2-connectedなグラフの任意の2つの辺を含むcycleの存在
date: 2025-04-27T21:35:02+12:00
categories:
  - グラフ理論
tags:
  - 命題
draft: false
---

2-connectedなグラフにおいて、任意の2本の辺を含むcycleが存在することを、Mengerの定理を用いて証明する方法を紹介します。

<!--more-->

## 前提知識

{{% def "誘導される部分グラフ" %}}
グラフ$G = (V, E)$と頂点集合$V$の部分集合$U \subset V$について、
グラフ$(U, \set{\set{x, y}; x, y \in U})$を$U$の誘導する部分グラフといい、
$G[U]$とかく。
{{% /def %}}

{{% def "$k$-connected" %}}
グラフ$G$の頂点集合からどの$k-1$頂点を取り除いても誘導されるグラフが連結なとき、$G$は$k$-connectedであるという。
{{% /def %}}

{{% def path %}}
グラフ$G$の相異なる頂点の列$v_1, v_2, ..., v_n$で、
$i = 1, 2, ..., n-1$について$\set{v_i, v_i+1} \in E(G)$を満たすものを$v_1$から$v_n$へのpathという。
{{% /def %}}

{{% def cycle %}}
グラフ$G$の相異なる頂点の列$v_1, v_2, ..., v_n$で、
$i = 1, 2, ..., n-1$について$\set{v_i, v_i+1} \in E(G)$を満た し、更に$\set{v_n, v_1} \in E(G)$を満たすものをcycleという。
{{% /def %}}

{{% def independence %}}
2つの$x$から$y$へのpath$x, v_1, ..., v_n, y$と$x, u_1, ..., u_m, y$について、
$v_1, ..., v_n$と$u_1, ..., u_m$の間に共通元がないとき、
2つのpathはindependentであるという。
{{% /def %}}

{{% thm Mengerの定理 %}}
$k$-connectedなグラフの任意の2頂点の間には、$k$本のindependentなpathが存在する
{{% /thm %}}

{{% thm "ear decomposition" %}}
グラフ$G$について、以下は同値

- $G$は2-connected
- グラフの列$G_0, G_1, ..., G_n$であって、以下を満たすものが存在する。
  - $G_0$はcycle
  - $G_n = G$
  - 各$i = 1, 2, ..., n-1$について、
  $G_{i+1}$は$G_i$にpathを付け加えることで得られる。

すなわち、cycleにpathをいくつか付け加えたものは2-connectedであり、
逆に2-connectedなグラフは必ずそのようにして得られる。
{{% /thm %}}

## 主張

{{% prop %}}
$G$を2-connectedなグラフとし、$e, f$をその異なる2辺とすると、
$G$は$e, f$をともに含むcycleを持つ。
{{% /prop %}}

## 証明

$e = \set{x, y}, f = \set{z, w}$とし、$s, t$を$V(G)$に現れない元とする。

$G$に頂点$s, t$と辺$\set{s, x}, \set{s, y}, \set{z, t}, \set{w, t}$を付け加えて得られるグラフ$G'$を考える。
$G'$は$G$に2つのpathを加えてできるグラフなので2-connectedである。
よってMengerの定理より、$s$から$t$への2つのindependent pathsが存在する。
したがって、以下のどちらかが成立する。

- $x$から$z$, $y$から$w$への交わらないpathsが存在する
- $x$から$w$, $y$から$z$への交わらないpathsが存在する

どちらの場合でも、得られたpathsと$e, f$はcycleをなす。

## 系

{{% cor %}}
グラフ$G$の異なる辺$e, f$について、以下は同値

- $e, f$を含むcycleが存在する
- $e, f$を含むblock（極大2-connected部分グラフまたはbridgeとそのendverticesからなる部分グラフ）が存在する
{{% /cor %}}

## 参考文献
