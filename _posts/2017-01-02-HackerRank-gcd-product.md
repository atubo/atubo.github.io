---
layout: post
title: HackerRank "GCD Product"
---

$\text{ans}=\prod\limits_{i=1,j=1}^{i=n,j=m} \gcd(i,j)$

Therefore

$$
\begin{align*}
\log(\text{ans})&=\log (\prod_{i,j}\gcd(i,j)) \\
&=\sum_{i,j}\log (\gcd(i, j)) \\
&=\sum_{i,j}\sum_{t}\log(t) [\gcd(i,j)=t] \\
&=\sum_{t=1}^{n}\log(t)\sum_{t\vert d} \mu(\frac{d}{t}) \lfloor \frac {n}{d} \rfloor \lfloor \frac{m}{d} \rfloor \\
\end{align*}
$$

Let $d=kt$, then

$$
\begin{align*}
\log(\text{ans})&=\sum_{t=1}^{n}\log(t)\sum_{k}\mu(k) \lfloor \frac{n}{kt} \rfloor \lfloor \frac{m}{kt} \rfloor \\
&=\sum_{t=1}^{n} \log(t) \sum_{k=1}^{n'} \mu(k) \lfloor \frac{n'}{k} \rfloor \lfloor \frac{m'}{k} \rfloor
\end{align*}
$$

where $n'=\frac{n}{t}$, thus

$$
\text{ans}=\prod_{t=1}^{n} t^{\sum\limits_{k=1}^{n'} \mu(k) \lfloor \frac{n'}{k} \rfloor \lfloor \frac{m'}{k} \rfloor}
$$

