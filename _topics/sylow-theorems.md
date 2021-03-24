---
layout: page
title: Sylow Theorems
---


## Subgroups of a given order

Let $$G$$ be a finite group.  We know from Lagrange's theorem that if $$H$$ is a subgroup of $$G$$ then the order of $$H$$ divides the order of $$G$$.  Thus subgroups of $$G$$ must have orders determined by the divisors of $$n = \lvert G\rvert$$.  In the abelian case, we actually know much more!  We know that if $$m$$ divides $$n$$ then $$G$$ has a subgroup of order $$m$$.

**Theorem:** If $$G$$ is a finite abelian group of order $$n$$, and $$m$$ divides $$n$$, then $$G$$ has a subgroup of order $$m$$.

This is not true however in the nonabelian case!

**Ex:** The alternating group $$A_n$$ has order $$n!/2$$, but has no subgroup of order $$n!/4$$ for $$n\geq 5$$.  Such a subgroup would have index $$2$$ and therefore be normal, but we know $$A_n$$ is a simple group (ie. has no normal subgroups).

Still we can show that some subgroups of various orders must exist.  For example, we have Cauchy's theorem.

**Cauchy's Theorem:**  Let $$G$$ be a finite group and let $$p$$ be a prime number dividing the order of $$G$$.  Then $$G$$ has a subgroup of order $$p$$.

Sylow Theory extends Cauchy's result to prove the existence of subgroups of order $$p^k$$.  Moreover, it relates these subgroups in terms of containment and conjugation.

## Sylow subgroups

**Def:**  Let $$p$$ be a prime number.  A **$$p$$-subgroup** $$H$$ of $$G$$ is a proper subgroup of order $$p^k$$ for some integer $$k>0$$

**Def:**  A $$p$$-subgroup $$H$$ of $$G$$ is a **Sylow $$p$$-subgroup** if $$H$$ is not properly contained in any other $$p$$ subgroup of $$G$$.  In other words, Sylow $$p$$-subgroups are maximal among the chains of subgroups.  

