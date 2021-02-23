---
layout: page
title: Homework 5
permalink: /homework/hw5
---

### Directions
Solve the following problems and type up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* printed in barely-legible script using a gourmet custom t-shirt maker from Etsy in true hipster fashion

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

**Problem 1:** Find, up to isomorphism, all abelian groups of order $$1089$$

**Problem 2:** Find all cosets of the subgroup $$\langle 18\rangle$$ in the gropu $$\mathbb Z_{36}$$

**Problem 3:** Give an example of a group $$G$$ whose order is not prime and which is not isomorphic to any direct product of its nontrivial proper subgroups.

**Problem 4:** Let $$G$$ be a finite abelian group.  Show that if $$G$$ is not cyclic, then $$G$$ contains a subgroup isomorphic to $$\mathbb Z_p\times \mathbb Z_p$$ for some prime number $$p>1$$.

**Problem 5:** Show that if $$G$$, $$H$$ and $$K$ are groups and $$G\times K\cong H\times K$$, then $$G\cong H$$

**Problem 6:** For each of the following, give an example or explain why no example exists.
* A subgroup $$H$$ of an infinite group $$G$$ where $$H$$ has finitely many left cosets
* A subgroup of a group of order $$6$$, which has $$6$$ left cosets
* A subgroup of a group of order $$6$$, which has $$12$$ left cosets
* A subgroup of a group of order $$6$$, which has $$4$$ left cosets

**Problem 7:**  

Suppose that $$G$$ is a group (possibly infinite) and that $$H$$ is a subgroup of $$G$$.  Show that the cardinality of the set of left cosets of $$G$$ is the same as the cardinality of the set of right cosets.

**Problem 8:**

The **center of a group $$G$$** is the set

$$Z(G) = \{x\in G: ax=xa\ \forall a\in G\}.$$

Fill in the gaps in the proof of the following theorem by proving each claim.

**Theorem:** Suppose that $$G$$ is a group of order $$pq$$ with $$p$$ and $$q$$ prime.  Then either $$G$$ is abelian or $$Z(G) = \{e\}$$.

**Proof:**
Assume that $$G$$ is not a cyclic group and that $$Z(G) \neq \{e\}$$.  Choose $$x\in Z(G)$$ with $$x\neq e$$.  Note that since $$G$$ is not cyclic, we know $$G\neq \langle x\rangle$$.  Choose an element $$y\in G\backslash \langle x\rangle$$.

**Claim:** The orders of $$\langle x\rangle$$ and $$\langle y\rangle$$ are both prime.  

**Claim:** $$\langle x\rangle\cap \langle y\rangle = \{e\}$$

Thus without loss of generality, we may take the order of $$\langle x\rangle$$ to be $$p$$ and the order of $$\langle y\rangle$$ to be $$q$$.  Now consider the function

$$\varphi: \mathbb Z_p\times\mathbb Z_q\rightarrow G,\quad \varphi(j,k)\mapsto x^jy^k$$

**Claim:** The function $$\varphi$$ is an isomorphism.

Since $$G$$ is isomorphic to $$\mathbb Z_p\times\mathbb Z_q$$, this shows that $$G$$ is abelian.

