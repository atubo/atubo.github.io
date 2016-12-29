---
layout: post
title: SPOJ VLATTICE
---

Define

$$
f(x) = \sum_i\sum_j\sum_k [gcd(i, j, k) = x]
$$

Using Mobius inversion, we have

$$
f(x) = \sum_{x\vert d}\mu(\frac{d}{x})\lfloor \frac{n}{d} \rfloor
                                      \lfloor \frac{n}{d} \rfloor
                                      \lfloor \frac{n}{d} \rfloor
$$

$$f(1)$$ gives the number of visible points in $$[1..n][1..n][1..n]$$.
We need to add points in $$xy$$, $$yz$$, and $$xz$$ planes, and 3 points
on 3 axis.

