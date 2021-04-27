---
layout: page
title: Homework 8
permalink: /homework/hw8
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* submitted to David X. Cohen to be included inconspicuously in an upcoming episode of The Simpsons.

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:** 

For each of the following examples of rings, determine with explanation whether or not the ring is an integral domain.  If it is an integral domain, describe its field of fractions.

* (a) $$\mathbb Z$$
* (b) $$\mathbb Z\times\mathbb Z$$
* (c) $$\mathbb Z[x]$$
* (d) the set of $$2\times 2$$ matrices with coefficients in $$\mathbb C$$
* (e) $$\mathbb Q[x]/I$$ for $$I$$ the principal ideal $$I = \langle x^2-1\rangle$$

**Problem 2:**

Let $$R$$ be a commutative ring with identity.
An ideal $$I$$ in $$R$$ is called **prime** if it satisfies the property that

$$ab\in I\ \Longleftrightarrow\ a\in I\ \text{or}\ b\in I.$$

* (a) Show that if $$f(x)\in \mathbb Q[x]$$ is an irreducible polynomial, then the ideal $$I = \langle f(x)\rangle$$ of $$Q[x]$$ is a prime ideal.

* (b) Let $$I$$ be an ideal of a commutative ring with identity $$R$$.  Show that $$I$$ is a prime ideal if and only if $$R/I$$ is an integral domain.

**Problem 3:**

For each of the following field extensions of $$\mathbb Q$$, describe the field extension by finding a basis.

* (a) $$\mathbb Q[\sqrt{-5}]$$
* (b) $$\mathbb Q[\sqrt[3]{2}]$$
* (c) $$\mathbb Q[\sqrt{2} + i\sqrt{2}$$

**Problem 4:**
For many numbers it is difficult to determine whether or not the number is transcendental.

A **Liouville number** is an irrational number $$\alpha$$ satisfying the property that for every positive integer $$n>0$$, there are integers $$a$$ and $$b$$ with $$b>1$$ and

$$|\alpha - a/b| < 1/b^n.$$

In this problem, we will prove that Liouville numbers are transcendental.
The proof of this algebraic fact is particularly interesting, given its reliance on *analysis*.

Let $$\alpha$$ be an irrational number which is *not* transcendental, and in particular is a simple root of a nonzero polynomial $$f(x)\in \mathbb Z[x]$$ of degree $$d$$.  Choose $$r>0$$ such that $$\alpha$$ is the only root of $$f(x)$$ on $$[\alpha-r,\alpha+r]$$ is $$\alpha$$ and let $$M = \max\{|f'(x)|: |x-\alpha|\leq r\}.$$
By the Mean Value Theorem

$$|f(x)| = |f(x)-f(\alpha)|\leq |x-\alpha|M\quad\text{for all}\ |x-\alpha|\leq r.$$

* (a) Suppose that $$a,b$$ are integers with $$b>0$$ and $$|x-a/b|\leq r$$.  Show that $$1/b^d < |f(a/b)|$ and use the above inequality to prove

$$\frac{1}{b^dM} < |\alpha-a/b|.$$

* (b) Now choose $$n>0$$ such that $$2^n>\max(1/M,1/r)$$.  Note that this means $$b^n>\max(1/M,1/r)$$ for any integer $$b>1$$.  Use the result of part (a) to show that $$\alpha$$ cannot be a Liouville number.  Thus all Liouville numbers must be transcendental.

* (c) Use the result of (b) to prove that the number

$$\alpha = \sum_{k=0}^\infty \frac{1}{10^{k!}}$$

is transcendental.






