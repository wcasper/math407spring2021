---
layout: page
title: Homework 3
permalink: /homework/hw3
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* inscribed in animal bone and pitched into a Scottish bog to be preserved for future generations

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**  

Find the kernel of each of the following morphisms.
* $$\phi: \mathbb Z\rightarrow\mathbb Z_8$$ defined by $$\phi(1)=6$$
* $$\phi: \mathbb Z\times\mathbb Z\rightarrow\mathbb Z$$ defined by $$\phi(m,n) = 3m-5n$$
* $$\phi: \mathbb Z\times\mathbb Z\rightarrow\mathbb Z\times\mathbb Z$$ defined by $$\phi(m,n) = (2m-3n,5m+2n)$$

**Problem 2:**

Let $$A$$ be a finite set and $$\sigma\in S_A$$.  Define a relation $$\mathscr R_\sigma$$ on $$A$$ by saying $$a\mathscr R_\sigma b$$ if and only if $$b\in\text{orb}_\sigma (a)$$.
* Show that $$\mathscr R_\sigma$$ is an equivalence relation on $$A$$
* Show that the equivalence class of $$a\in A$$ under $$\mathscr R_\sigma$$ is exactly $$\orb_\sigma(a)$$.  Since the equivalence classes of an equivalence relation form a partition, this shows that the orbits of $$\sigma$$ form a partition of $$A$$
* Choose $$a_1,a_2,\dots,a_r\in A$$ so that $$\{\text{orb}_\sigma(a_j): 1\leq j\leq r\}$$ is a partition of $$A$$.  For each $$j$$, let $$m_j = |\text{orb}_\sigma(a_j)$$ and $$a_{jk} = \sigma^k(a_j)$$ for $$1\leq k\leq m_j$$.  Prove that

$$\sigma = (a_{11}\ a_{12}\ \dots\ a_{1m_1})(a_{21}\ a_{22}\ \dots\ a_{2m_2})\dots(a_{r1)\ a_{r2}\ \dots\ a_{rm_r}).$$

In particular, this shows that $$\sigma$$ can be expressed as a product of **disjoint cycles**.

**Problem 3:**

Let $$A$$ be a set and let $$a_1,a_2,\dots,a_n\in A$$ be $$n$$ distinct elements of $$A$$.

* Show that for any $$2\leq k\leq n-1$$

$$(a_k\ a_{k+1}\ \dots\ a_n)(a_{k-1}\ a_n) = (a_{k-1}\ a_k\ a_{k+1}\ \dots\ a_n)$$

* Show that the $$n$$-cycle

$$\sigma = (a_1\ a_2\ a_3\ \dots\ a_n)$$

can be expressed as a product of transpositions (ie. $$2$$-cycles).

**Problem 4:**

For each of the following permutations, find all the orbits.  Then express the given permutation as a product of disjoint cycles.  Finally, express the permutation as a product of transpositions and determine the parity of the permutation
* $$\binom{1\ 2\ 3\ 4\ 5\ 6}{5\ 1\ 3\ 6\ 2\ 4}$$ in $$S_6$$
* $$\binom{1\ 2\ 3\ 4\ 5\ 6\ 7\ 8}{2\ 3\ 5\ 1\ 4\ 6\ 8\ 7}$$ in $$S_8$$

**Problem 5:**

Suppose that $$H$$ is a subgroup of $$S_n$$ for $$n>1$$.  Show that either all the permutations in $$H$$ are even, or else exactly half of them are even.



