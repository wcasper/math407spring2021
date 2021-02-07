---
layout: page
title: Subgroups
---

## Basic Definition and Examples

Let $$G$$ be a group with binary operation $$*$$ and identity $$e$$.

**Definition:** A **subgroup** $$H$$ of $$G$$ is a subset $$H\subseteq G$$ with the property that $$*$$ restricts to a binary operation on $$H$$ making $$H$$ a group.  A subgroup $$H$$ is called **proper** if $$H\neq G$$.

**Notation:** We write $$H<G$$ or $$H\leq G$$ to mean that $$H$$ is a subgroup of $$G$$ and $$H\lneq G$$ to mean that $$H$$ is a proper subgroup of $$G$$.

**Example:** The set $$\{e\}$$ is a subgroup of $$G$$.  This is called the
**trivial subgroup**.  If $$H\neq \{e\}$$ then $$H$$ is called **non-trivial**.

**Example:** The subset $$H = \{0,2,4,6\}$$ is a subgroup of $$\mathbb Z_8$$.

**Example:** The set $$H = \{z\in\mathbb C: z^n=1\}$$ of $$n$$'th roots of unity is a subset of $$\mathbb T = \{z\in\mathbb C: |z\ = 1\}.$$

**Example:** The set $$\text{SL}_n = \{A\in \text{GL}_n(\mathbb R): \det(A) = 1\}$$ is a subset of the group $$\text{GL}_n(\mathbb R)$$ of $$n\times n$$ real, invertible matrices. These groups are referred to as the **special linear group** and the **general linear group** respectively.

In general, to check if a subset $$H$$ of $$G$$ is a subgroup, we can check three very simple properties captured in the next theorem.

**Theorem:**  A subset $$H$$ of $$G$$ is a subgroup if and only if the following properties hold
* $$e\in H$$
* $$a*b\in H$$ for all $$a,b\in H$$ (ie. $$H$$ is closed under $$*$$)
* $$a^{-1}\in H$$ for all $$a\in H$$ (ie. $$H$$ is closed under inversion)

**Proof:** Since $$G$$ is a group, we know $$*$$ is associative.  Thus the second property implies $$H$$ is a semigroup.  The first property implies that $$H$$ is a monoid, and finally the last property implies that $$H$$ is a group.

In fact, we can reduce our check that a subset is a group to checking a single property.

**Theorem:** A nonempty subset $$H$$ is a group if and only if it satisfies the following property
* $$x*y^{-1}\in H$$ for all $$x,y\in H$$

**Proof:**  Let $$a\in H$$, which exists since $$H$$ is non-empty.  Then taking $$x=y=a$$, we see $$e = aa^{-1}\in H$$.  Now taking $$x=e,y=a$$ we see $$a^{-1} = e*a^{-1}\in H$$.  Thus $$H$$ contains the identity and is closed under inversion.  Lastly, if $$a,b\in H$$ then $$b^{-1}\in H$$ and therefore taking $$x = a$$ and $$y=b^{-1}$$ we have $$a*b = a*(b^{-1})^{-1}\in H$$.  Thus $$H$$ is closed under $$*$$ and is therefore a group.

In the case that $$H$$ is a finite set, we have an even easier job!

**Theorem:** If $$H$$ is a finite subset of $$G$$ then $$H$$ is a subgroup if
and only if $$H$$ is closed under $$*$$.

**Proof:** Exercise.

**Proposition:** If $$H\leq G$$ and $$K\leq G$$ then the intersection $$H\cap K$$ is a subgroup of $$G$$.
**Proof:** If $$a,b\in H\cap K$$ then $$a,b\in H$$ and $$a,b\in K$$.  Since $$H$$ and $$K$ are subgroups, $$ab^{-1}\in H$$ and $$ab^{-1}\in K$$.  Therefore $$ab^{-1}\in H\cap K$$.

By the same argument, one can show that the intersection of any number of subgroups of $$H\cap K$$ is also a subgroup.


