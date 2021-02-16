---
layout: page
title: Homework 3
permalink: /homework/hw3
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* inscribed on the wing of a B-52 based at Area 51 in Roswell, New Mexico

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:**  Find all subgroups of the given group

* $$\mathbb Z_8$$
* $$\mathbb Z_{12}$$
* $$\mathbb Z_{17}$$

**Problem 2:**  An **automorphism** of a group $$G$$ is an isomorphism from $$G$$ to itself.  Find all automorphisms of each of the following groups

* $$\mathbb Z_8$$
* $$\mathbb Z_{84}$$
* $$\mathbb Z$$


**Problem 3:**  Let $$G$$ be a group and let $$S\subseteq G$$.  Show that

$$H_S = \{x\in G: xa = ax\ \text{for all $a\in S$}\}$$

is a subgroup.  Show that in the special case $$S=G$$ that $$H_S=H_G$$ is abelian.  The subgroup $$H_G$$ is called the **center** of $$G$$.

**Problem 4: (Bonus -- very tricky)**  Suppose that $$G\subseteq\mathbb R^3$$ is a group with binary operation $$*$$ satisfying the following property
* if $$a\times b\neq 0$$, then $$a*b = a\times b$$ (where the latter denotes the cross product)

Prove that $$a\times b=0$$ for all $$a,b\in G$$.

You can prove this via contradiction.  Start by assuming that there are $$a,b\in G$$ with $$a\times b\neq 0$$.  Then use the following steps.

1.  Show that $$G$$ must contain an orthogonal basis for $$\mathbb R^3$$.  Without loss of generality, we may take $$a$$, $$b$$, and $$c=a\times b$$ to be an orthogonal basis.
2.  By considering the product $$a*a*b$$, show that $$a*a$$ must be parallel to $$b$$.  Similarly, show it is parallel to $$c$$ and hence $$a*a=0$$.
3.  Use the same strategy to show that $$b*b=0$$ and $$c*c=0$$.
4.  By considering the product $$e*a$$, show that $$e$$ must be parallel to $$a$$.  Similarly, show that $$e$$ is parallel to $$b$$ also, forcing $$e=0$$.
5.  Show that $$b*a*b*a=e$$ and that $$a*a*b*b=e$$.  Conclude that $$a*b=b*a$$.
6.  Use the fact that $$a\times b = -b\times a$$ to conclude that $$c = a*b= 0$$, contradicting the assumption $$a\times b\neq 0$$.

**Problem 5:**  Recall that the **dihedral group** $$D_n$$ is

$$D_n = \{(a,j): a\in \mathbb Z_n\quad\text{and}\ j=\pm 1\}$$

with the binary operation $$(a,j)*(b,k) = (ak+_nb,jk)$$.

Draw the Cayley graph for the dihedral group $$D_6$$ with generating set $$S = \{(1,1),(0,-1)\}$$.

**Problem 6:**  Let $$G = \mathbb C^\times$$ be the group  of nonzero complex numbers with binary operation given by multiplication and let $$H$$ be a finite subgroup of $$G$$.

1. Show that if $$z\in H$$, then $$z^k = 1$$ for some $$k$$.
2. Let $$H = \{z_0,z_1,\dots, z_r\}$$ and for each $$j$$ choose $$m_j>0$$ with $$z_j^{m_j}=1$$ (which exist by Part 1).  Show that $$m=m_1m_2\dots m_r$$ satisfies $$z_j^m=1$$ for all $$j$$.  Thus $$H\leq \{z\in\mathbb C : z^m = 1\}.$$

3. Suppose that $$w\in\mathbb C$$ and $$w^m=1$$ for some $$m>0$$.  Show that $$\langle w\rangle = \{z\in\mathbb C: z^n = 1\}$$, where here $$n$$ is the smallest positive integer satisfying $$w^n=1$$.

4. Use Part 3 and the fact that $$\{z\in\mathbb C : z^m = 1\}$$ is cyclic, and that subgroups of cyclic groups are cyclic, to prove that there exists an $$n>0$$ satisfying

$$H = \{z\in\mathbb C: z^n = 1\}$$






