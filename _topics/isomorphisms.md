---
layout: page
title: Isomorphisms
---

### Basic definition

Suppose that $$(G,*)$$ and $$(G,\star)$$ are two sets with binary relations.  Sometimes, these sets will be basically the same in a certain sense.  For example, there is obviously very little difference between

$$G = \{0,1,2,3,\dots,11\}\quad \text{with the binary relation $+_{12}$}\}$$

and the set

$$H = \{x| \text{$x$ is an hour on a clock}\}\quad \text{with the binary relation of adding hours}$$

Mathematically, the way we express this kind of equivalence is through isomorphisms.

**Definition:**  An **isomorphism** from $$(G,*)$$ to $$(H,\star)$$ is a bijection $$f: G\rightarrow H$$ satisfying

$$f(a*b) = f(a)\star f(b)\quad\text{for all $a,b\in G$}.$$

In other words, it's a bijection which is compatible with the binary relations.

### The circle group

The unit circle in the complex plane $$\mathbb T$$ consists of all complex numbers $$z\in\mathbb C$$ whose norm is $$1$$

$$\mathbb T = \{z\in\mathbb C : |z| = 1\}.$$

The circle has a well-define binary relation given by the usual multiplication of complex numbers.

$$z*w = zw.$$

It turns out that this is isomorphic to

$$\mathbb R_{2\pi} = [0,2\pi)\quad\text{with the binary operator $+_{2\pi}$}.$$

To see this, consider the function

$$f: \mathbb R_{2\pi}\rightarrow \mathbb T,\quad\text{defined by}\ f(x) = e^{i x}.$$

We claim that this is an isomorphism!  To check this, we need to show that it is a bijection and that it respects the binary operators.

* **Injectivity:**

If $$f(x) = f(y)$$, then $$e^{i x} = e^{iy}$$ and therefore $$e^{i (x-y)} = 1$$ meaning that 

$$\cos(x-y) + i\sin(x-y) = 1.$$

Thus $$\sin(x-y)=0$$ meaning that $$x-y=k\pi$$ for some integer $$k$$ and since $$\cos(x-y) = 1$$ we see $$k$$ is even, ie. $$k=2j$$ for some $$j$$.  Since $$0\leq x,y < 2\pi$$, this means $$x-y=0$$ so that $$x=y$$.  This proves injectivity.

* **surjectivity:**

If $$z\in \mathbb T$$, then Euler's formula says $$z = e^{i\theta}$$ for some $$0\leq\theta < 2\pi$$ because $$|z|=1$$. Thus $$z = f(\theta)$$.  This proves surjectivity.

* **respects the binary operator:**

Since $$x+_{2\pi}y = x+y+2\pi j$$ for some integer $$j$$, we see

$$f(x+_{2\pi} y) = e^{i(x+_{2\pi}y)} = e^{i(x+y+2\pi j)} = e^{ix + iy + 2\pi i j} = e^{ix}e^{iy}\left(e^{2\pi i}\right)^j = e^{ix}e^{iy} 1^j = f(x)f(y).$$

Thus  $$f(x+_{2\pi}y) =f(x)f(y)$$ and the function $$f(x)$$ preserves the inner product.

### The dihedral group

Let $$n>2$$ be an integer and consider the set

$$D_n = \{0,1,2,\dots,n-1\}\times \{-1,1\}$$

We define a binary relation on $$D_n$$ by setting

$$(a,b)*(c,d) = (a*d +_n c, bd)$$

This binary relation makes $$D_n$$ into a group called the **dihedral group**.

**Example:** Let's look at the multiplication table for this binary relation for $$D_3$$

|    *   | (0, 1) | (1, 1) | (2, 1) | (0,-1) | (1,-1) | (2,-1) |
| (0, 1) | (0, 1) | (1, 1) | (2, 1) | (0,-1) | (1,-1) | (2,-1) |
| (1, 1) | (1, 1) | (2, 1) | (0, 1) | (2,-1) | (0,-1) | (1,-1) |
| (2, 1) | (2, 1) | (0, 1) | (1, 1) | (1,-1) | (2,-1) | (0,-1) |
| (0,-1) | (0,-1) | (1,-1) | (2,-1) | (0, 1) | (1, 1) | (2, 1) |
| (1,-1) | (1,-1) | (2,-1) | (0,-1) | (2, 1) | (0, 1) | (1, 1) |
| (2,-1) | (2,-1) | (0,-1) | (1,-1) | (1, 1) | (2, 1) | (0, 1) |

**Theorem:** The **dihedral group** $$D_n$$ is isomorphic to the group of symmetries of a regular $$n$$-sided polygon.

**Proof for the triangle:**

The set of symmetries $$\text{symm}(T)$$ of the triangle $$T$$ consists of
* clockwise rotation by $$0$$, $$120$$, and $$240$$ degrees: $$R_0$$, $$R_{2\pi/3}$$ and $$R_{4\pi/3}$$
* reflection across $$x=0$$, $$y=-\sqrt{3}x$, and $$y=\sqrt{3}x$$: $$S_0$$, $$S_{2\pi/3}$$, $$S_{4\pi/3}$$

Define a function $$f: D_n\rightarrow T$$ by

$$\begin{align*}
(0, 1) &\mapsto R_0\\
(1, 1) &\mapsto R_{2\pi/3}\\
(2, 1) &\mapsto R_{4\pi/3}\\
(0,-1) &\mapsto S_0\\
(1,-1) &\mapsto S_{2\pi/3}\\
(2,-1) &\mapsto S_{4\pi/3}
\end{align*}$$

This defines a bijection from $$D_n$$ to $$T$$.  For this to be an isomorphism, we need to make sure it respects the products. We can check this by looking at the image of the multipliication table under this map

|                | $$R_0$$        | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ |
| $$R_0$$        |  $$R_0$$       | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ |
| $$R_{2\pi/3}$$ | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$R_0$$        | $$S_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ |
| $$R_{4\pi/3}$$ | $$R_{4\pi/3}$$ | $$R_0$$        | $$R_{2\pi/3}$$ | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ | $$S_0$$        |
| $$S_0$$        | $$S_0$$        | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ | $$R_0$$        | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ |
| $$S_{2\pi/3}$$ | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ | $$S_0$$        | $$R_{4\pi/3}$$ | $$R_0$$        | $$R_{2\pi/3}$$ |
| $$S_{4\pi/3}$$ | $$S_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$R_0$$        |

This is identical to the multiplication table for the symmetry group of the triangle, so the previous map is an isomorphism!
