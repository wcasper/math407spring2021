---
layout: page
title: Finitely Generated Abelian Groups
---

## Structure Theorem

One of the great results of elementary group theory is the classification of finitely generated abelian groups.  We'll state the classification first, followed by some examples and some theorems used to prove it.

The structure theorem has two verions, both very useful depending on the circumstances.

**Theorem (Fundamental Theorem of Finitely Generated Abelian Groups -- Prime Divisor Version):**
If $$G$$ is a finitely generated abelian group, then $$G$$ is isomorphiic to

$$G\cong Z_{p_1^{r_1}}\times Z_{p_2^{r_2}}\times\dots\times Z_{(p_n)^{r_n}}\times Z^s$$

where here $$p_1,\dots, p_n$$ are primes (not necessarily distinct) and $$r_1,\dots, r_n,s$$ are nonnegative integers.
Furthermore, the direct product is unique, up to rearrangement of the factors.

**Example:** Any finitely generated abelian groups of order $$24$$ must be isomorphic to one of the following
* $$\mathbb Z_{2^3}\times\mathbb Z_3$$
* $$\mathbb Z_{2^2}\times \mathbb Z_2\times\mathbb Z_3$$
* $$\mathbb Z_2\times\mathbb Z_2\times \mathbb Z_2\times\mathbb Z_3$$

**Theorem (Fundamental Theorem of Finitely Generated Abelian Groups -- Invariant Factor Version):**
If $$G$$ is a finitely generated abelian group, then $$G$$ is isomorphiic to

$$G\cong Z_{a_1}\times Z_{a_2}\times\dots\times Z_{a_m}\times Z^s$$

where $$a_j\geq 2$$ is an integer for all $j$$ and $$a_j$$ divides $$a_{j+1}$$ for $$1\leq j\leq m-1$$.  Furthermore, the representation is unique.

**Example:** Any finitely generated abelian groups of order $$24$$ must be isomorphic to one of the following
* $$\mathbb Z_{24}$$
* $$\mathbb Z_{2}\times \mathbb Z_{12}$$
* $$\mathbb Z_2\times\mathbb Z_2\times \mathbb Z_6$$

## Direct Sum of Cyclic Groups

From the above, we see that in particular a direct sum of cyclic groups can be put into a **canonical form**, either prime divisor form or invariant factor form.

For example, the group $$\mathbb Z_6\times \mathbb Z_9$$ has
* prime divisor form $$\mathbb Z_2\times\mathbb Z_3\times\mathbb Z_9$$
* invariant factor form $$\mathbb Z_3\times \mathbb Z_{18}$$

The theorem we use to go between forms is the following

**Theorem:**
The groups $$\mathbb Z_m\times\mathbb Z_n$$ and $$\mathbb Z_{mn}$$ are isomorphic if and only if $$m$$ and $$n$$ are relatively prime.

Using this, we find

$$\begin{align*}
\mathbb Z_6\times\mathbb Z_9
  & \cong \mathbb Z_2\times\mathbb Z_3\times\mathbb Z_9\\
  & \cong \mathbb Z_3\times\mathbb Z_2\times\mathbb Z_9\\
  & \cong \mathbb Z_3\times\mathbb Z_{18}
\end{align*}$$
