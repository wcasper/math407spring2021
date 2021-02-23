---
layout: page
title: Normal Subgroups
---

## Basic Definition and Examples

**Definition:** Let $$G$$ be a group and $$H$$ a subgroup.  We say that $$H$$ is a **normal subgroup** if $$aH = Ha$$ for all $$a\in G$$.  In this case we write $$H\trianglelefteq G$$.

**Example:** If $$G$$ is abelian, then every subgroup is normal.

**Example:** Consider the group $$G$$ of symmetries of the square, which consists of the four rotations $$R_0$$, $$R_{\pi/4}$$, $$R_{\pi/2}$$, $$R_{3\pi/4}$$ and the four reflections $$S_0$$, $$S_{\pi/4}$$, $$S_{pi/2}$$, $$S_{3\pi/4}$$.  The subgroup $$H = \{R_0,R_{\pi/4},R_{\pi/2},R_{3\pi/4}\}$$ is a normal subgroup.  The subgroup $$K=\{R_0,S_0\}$$ is not a normal subgroup.

**Theorem:**  Let $$\phi: G\rightarrow H$$ be a group homomorphism.  Then the kernel $$\ker(\phi)$$ is a normal subgroup of $$G$$.

We will show later that every normal subgroup of $$G$$ arises in this fashion.

**Example:** The determinant defines a group homomorphism

$$\det: \text{GL}_n(\mathbb C)\rightarrow \bbc^\times,\quad A\mapsto \det(A).$$

The kernel of this homomorphism is the special linear group

$$\text{SL}_n(\mathbb C) = \{A\in M_n(\bbc): \det(A) = 1\}.$$

Thus the special linear group is a normal subgroup of the general linear group.

**Theorem:** Let $$H\leq G$$.  Then the following are equivalent.
* $$H$$ is a normal subgroup of $$G$$
* $$ghg^{-1}\in H$$ for all $$h\in H$$ and $$g\in G$$
* every right coset of $$H$$ in $$G$$ is also a left coset

