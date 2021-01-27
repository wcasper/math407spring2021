---
layout: post
title: Modular arithmetic
---

One of the foundations of number theory is a clockwork-style addition for numbers called **modular arithmetic**.  To begin, fix a positive integer $$n$$ and consider the set

$$\mathbb Z_n = \{0,1,2,3,\dots,n-1\}.$$

We define **modular addition** on $$\mathbb Z_n$$ by setting

$$a +_n b = \text{remainder after dividing $a+b$ by $n$}.$$

This makes $$\mathbb Z_n$$ into a group.  So for example

$$\begin{align*}
2 +_5 3 &= 0\\
8 +_2 5 &= 1\\
4 +_7 9 &= 6.
\end{align*}$$

Note: the notation we use here is consistent with Fraleigh's text, but is not the usual notation for this operation.  The latter is typically framed in terms of the notion of a **quotient group**, a topic of later discussion.

This kind of weird addition is actually very intuitive if we think about how hours work on a clock.  If it's currently 10:00 then in three hours it will be 1:00.  Fourteen hours after that, it will be 3:00.  Thus mathematically, we're discovring that clock-addition works just like addition modulo $$12$$:

$$\begin{align*}
10 +_{12} 3 = 1\\
1 +_{12} 14 = 3
\end{align*}$$

We can also define a continuous form of modular addition for real numbers.  Fix a positive real number $$r>0$$ and consider the set

$$\mathbb R_r = [0,r).$$

We define modular addition on $$\mathbb R_r$$ by setting

$$a+_rb = \left\lbrace\begin{array}{cc}
a+b, & \text{if $a+b<r$}\\
a+b-r, & \text{if $a+b\geq r$}
\end{array}\right.$$

Thus for example

$$\begin{align*}
\sqrt{2} +_3 2 &= \sqrt{2}-1\\
4.3 +_5 + 2.1 &= 1.4
\end{align*}$$

This defines a group, and we can look to the unit circle for intuition.  In the unit circle, if we have an angle of $$7\pi/4$$ radians and then we add $$\pi/2$$ radians, then we have gone one full circle ($$2\pi$$ radians), plus a bit extra, ending up at $$\pi/4$$ radians.  In other words, radians in the unit circle work like modular addition modulo $$2\pi$$.

$$7\pi/4 +_{2\pi} \pi/2 = \pi/4.$$

For this reason, we often identify $$\mathbb R_{2\pi}$$ with the unit circle.
