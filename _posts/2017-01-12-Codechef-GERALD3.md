---
layout: post
title: Codechef GERALD3
tags:
    - Mo's algorithm
    - Suffix array
---
[Problem link](https://www.codechef.com/problems/GERALD3)

Use Mo's algorithm + suffix array

Denote $s(x)$ as the suffix starting at position $x$.  When we add a position $x$, suppose its rank in the suffix array is $k$, we look for its neighbors that have been added and calculate the maximum of the two LCPs between itself and the two neighbors.  Then the current answer is increased by $N-x-LCP$.
