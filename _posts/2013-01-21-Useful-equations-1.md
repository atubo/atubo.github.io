---
layout: post
title: Useful equations - 1
use_math: true
---
$$\sum\limits_{k=0}^n k (\frac 1 2)^k=2-\frac{n+2}{2^n}$$


#Proof

Note that

$$
\begin{align*}
(\frac 1 2)^x &= -2\Delta((\frac 1 2)^x)\\
\sum\limits_{k=0}^n (\frac 1 2)^k&= 2 - (\frac 1 2)^n
\end{align*}
$$

Therefore,

$$
\begin{align*}
\sum\limits_{k=0}^n k (\frac 1 2)^k 
&=\sum\limits_{k=0}^{n+1} x (\frac 1 2)^x \delta x\\
&=-2\sum\limits_{k=0}^{n+1} x \Delta((\frac 1 2)^x)\\
&=-2\left[\left.x(\frac 1 2)^x\right|_0^{n+1}-\sum\limits_{k=0}^{n+1}(\frac 1 2)^{x+1}\delta x\right]\\
&=-2\left[(n+1)\left(\frac 1 2\right)^{n+1}-\left(\frac 1 2\right)\left(2-(\frac 1 2)^n\right)\right]\\
&=2-\frac{n+2}{2^n}\qquad\Box
\end{align*}
$$

