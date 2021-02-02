---
layout: page
title: Complex number review
---

### Basic definitions

A **complex number** is a number of the form

$$z = x + iy,\quad\text{where $x$ and $y$ are real-valued}.$$

Here $$i$$ is a very special complex number, denoting the square root of a negative number $$i=\sqrt{-1}$$.  More generally, complex numbers of the form $$iy$$ for some $$y\in\mathbb R$$ are called **imaginary numbers**.  This is an absolutely horrible name, since it predisposes one to the notion that these numbers are unnatural or "made up".  In fact, imaginary numbers and more generally complex numbers are just as natural and "real" as their real counterparts.

Examples of complex numbers include $$2 + 3i$$ and $$\sqrt{2} + (-1)i$$.  The need for complex numbers arises naturally from the desire to find roots of polynomial equations.  An equation like $$z^2+1=0$$ has no solutions over the real numbers, but two solutions over the complex numbers, namely $$z=\pm i$$.  In fact, over the complex numbers the Fundamental Theorem of Algebra is true.

**Fundamental Theorem of Algebra**:  Allowing for complex roots, any polynomal with $$p(z)$$ of degree $$n$$ has exactly $$n$$ has precisely $$n$$ roots, counting multiplicities.
 
We can do all the usual operations with complex numbers
- addition:

$$(2 + 3i) + (5 + 7i) = 7 + 10i$$

- subtraction:

$$(2 + 3i) - (5 + 7i) = -2 - 4i$$

- multiplication

$$
\begin{align*}
(2 + 3i)\cdot (5 + 7i)
  & =  2\cdot 5 + 2\cdot 7i + 3i\cdot 5 + 3i\cdot 7i\\
  & =  10 + 14i + 15i + 21i^2\\
  & =  10 + 14i + 15i - 21\quad\text{(since $i^2=-1$)}\\
  & =  -11 + 29i
\end{align*}
$$

- division

$$
\begin{align*}
(2 + 3i) / (5 + 7i)
  & =  (2+3i)\cdot \frac{1}{5+7i}\\
  & =  (2+3i)\cdot \frac{1}{5+7i}\frac{5-7i}{5-7i}\\
  & =  (2+3i)\cdot \frac{5-7i}{(5+7i)(5-7i)}\\
  & =  (2+3i)\cdot \frac{5-7i}{74}\\
  & =  \frac{(2+3i)(5-7i)}{74}\\
  & =  \frac{31+i}{74}\\
  & =  \frac{31}{74} + \frac{1}{74}i
\end{align*}
$$

The **complex conjugate** of a complex number $$z = x + iy$$ is $$\overline z = x-iy$$.  Note that we multiplied and divided by the complex conjugate of $$5+7i$$ above in order to o simplify the denominator.  

### Geometric point of view

Just as the real numbers are geometrically arranged into the real line $$\mathbb R$$, the complex numbers naturally form a plane $$\mathbb C$$ called the **complex plane**.  All planes look the same, so we're really looking at something identical to the $$x,y$$-plane $$\mathbb R^2$$.  A complex number $$x+iy$$ corresponds to the point $$(x,y)$$ in $$\mathbb R^2$$.
The **norm of a complex number** is the distance of the point in the complex plane from the origin

$$|x + iy| = \sqrt{x^2 + y^2}.$$

The norm itself is very related to the complex conjugate via the relation
$$z\overline z = |z|^2\quad\text{or equivalently}\quad (x+iy)(x-iy) = x^2 + y^2.$$
In particular, a complex number times its complex conjugate is always a positive, real number.

Polar coordinates also translates naturally into the language of complex numbers.
Recall that a point $$(x,y)$$ in the complex plane can be rexpressed in polar coordinates as $$(r,\theta)$$ where here

$$\begin{align*}
x & = r\cos(\theta)\\
y & = r\sin(\theta)
\end{align*}$$

In this same way, we can write

$$x +iy = r\left[\cos(\theta) + i\sin(\theta)\right],\ \ r = |x+iy|$$

In particular **unimodular** complex numbers, complex numbers whose norms are equal to $$1$$, are all of the form $$\cos(\theta) + i\sin(\theta)$$ for some angle $$\theta$$.  The angle itself simply determines its position on the unit circle in the complex plane.

### Euler's Definition

One of the many great contributions Euler gave to modern mathematics is the following *definition*

$$e^{i\theta} = \cos(\theta) + i\sin(\theta).$$

This equation is called **Euler's Formula**.  The wonderful thing about this formula is that this definition is mathematically consistent in every way we could possibly expect!  For example, using trigonometric identities we can verify

$$(\cos(\theta)+i\sin(\theta))(\cos(\phi))+i\sin(\phi)) = \cos(\theta+\phi) + i\sin(\theta+\phi).$$

This is consistent with what we would expect from the exponential identities

$$e^{i\theta}e^{i\phi} = e^{i\theta + i\phi} = e^{i(\theta +\phi)}.$$

Of course, there's a reason why this definition works so well.  If we think about the exponential function as an absolutely convergent Taylor series

$$e^x = \sum_{n=0}^\infty \frac{x^n}{n!}$$

then by replacing $$x$$ with $$i\theta$$ and using the Taylor series for $$\sin(x)$$ and $$\cos(x)$$, we obtain

$$\begin{align*}
e^{i\theta}
  & = \sum_{n=0}^\infty \frac{(i\theta)^n}{n!}\\
  & = \sum_{n=0}^\infty \frac{(i\theta)^{2n}}{(2n)!} + \sum_{n=0}^\infty \frac{(i\theta)^{2n+1}}{(2n+1)!} \\
  & = \sum_{n=0}^\infty \frac{(-1)^n\theta^{2n}}{(2n)!} + i\sum_{n=0}^\infty \frac{(-1)^n\theta^{2n+1}}{(2n+1)!} \\
  & = \cos(\theta) + i\sin(\theta)
\end{align*}$$


