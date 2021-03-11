---
layout: page
title: Normalizers
---


## Normalizers and Prime Powers

In the non-abelian situation, subgroups of a group $$G$$ do not need to be normal.  In this case, it makes sense to consider the subset of elements of $$G$$ for which the group *does* behave like a normal subgroup. 

**Definition:**  The **normalizer** of a subgroup $$H$$ of $$G$$ is the set

$$N(H) = \{g\in G: gHg^{-1} = H\}.$$

The normalizer of $$H$$ in $$G$$ is the largest subgroup of $$G$$ containing $$H$$ in which $$H$$ is normal.

**Proposition:**  $$N(H)$$ is a subgroup of $$G$$ and $$H$$ is a normal subgroup of $$N(H)$$.

Of course, it's entirely possible that $$N(H)$$ is the same thing as $$H$$, which wouldn't be particularly interesting.  Luckily, under certain circumstances, we can prove that $$N(H)\neq H$$.  Here is one such example

**Lemma:** Let $$H$$ be a subgroup of a finite group $$G$$ and assume that the order of $$N$$ is a power of a prime $$p$$. Then

$$[N(H):H] = [G:H]\mod p.$$

To prove this lemma, we consider the action of the group $$H$$ on the set $$X = G/H$$ via multiplication.

Let $$x_1,\dots, x_n\in H$$ belong to the distinct nontrivial orbits of this group action.  We know that

$$\lvert X\rvert = \lvert X_H\rvert + \sum_{i} [H:H_{x_i}]$$

and since $$H$$ has order equal to a power of a prime, this implies $$[G:H] = \lvert X\rvert = \lvert X_H\rvert\mod p$$.

Furthermore, if $$haH = aH$$ for all $$h\in H$$ then $$a^{-1}ha\in H$$ for all $$h\in H$$, making $$a\in N(H)$$.  In this way $$N(H) = X_H$$ proving the Lemma.

As a consequence, we have the following

**Prop:** Let $$H$$ be a subgroup of a finite group $$G$$ and assume that the order of $$N$$ is a power of a prime $$p$$. If $$p$$ divides $$[G:H]$$ then $$N(H)\neq H$$.

This follows simply because the previous lemma implies $$[N(H):H] = 0\mod p$$ and therefore $$N(H)\neq H$$.


