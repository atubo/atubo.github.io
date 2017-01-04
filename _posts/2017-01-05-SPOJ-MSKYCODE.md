---
layout: post
title: SPOJ MSKYCODE
tags:
    - Mobius inversion
---

Denote $$\gcd(S)$$ as the gcd of a subset $$S$$, we have $$\text{ans}=\sum\limits_{S}[\gcd(S)=1]$$.

Define $$f(n)=\sum\limits_{S}[\gcd(S)=n]$$ and $$g(n) = \sum\limits_{d} f(n\cdot d)$$.

Therefore

$$f(x) = \sum\limits_{x\vert d}\mu(\frac {d}{x}) g(d)$$

and

$$\text{ans} = f(1) = \sum\limits_{d}\mu(d)g(d)$$

We also have $$g(d) = {C(d) \choose 4}$$ where $$C(d)$$ is the number of IDs that are divisible by
$$d$$.
