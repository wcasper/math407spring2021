---
layout: page
title: Permutation Groups
---

## The Symmetric Group

**Definition:** Let $$A$$ be a set.  A **permutation** of $$A$$ is bijection $$\sigma: A\rightarrow A$$.  The **symmetric group on $$A$$** is the set

$$S_A = \{\sigma: \sigma\ \text{is a permutation of $A$}\}.$$

In the special case that $$A = \{1,2,\dots,n\}$$, we write $$S_n$$ in place of $$S_A$$.

**Proposition:**  The set $$S_A$$ is a group with
* product $$\sigma*\tau = \sigma\circ\tau$$ given by composition
* identity $$e=id_A: a\mapsto a,\ \forall a\in A$$
* inverses given by *inverse functions* $$\sigma^{-1}: a\mapsto b$$ for $$\sigma(b) = a$$

**Notation:** For brevity, we write $$\sigma\tau$$ in place of $$\sigma\circ\tau$$.  We can represent an element $$\sigma\in S_n$$ as

$$\left(\begin{array}{ccccc}
1 & 2 & 3 & \dots & n\\
\sigma(1) & \sigma(2) & \sigma(3) & \dots & \sigma(n)
\end{array}\right)$$

Thus for example in $$S_4$$

$$\left(\begin{array}{cccc}
1 & 2 & 3 & 4\\
2 & 3 & 1 & 4
\end{array}\right)$$

represents the permutation which sends $$1\mapsto 2$$, $$2\maspto 3$$, and so on.

An alternative, extremely useful notation is in terms of cycles

**Definition:** A **k-cycle** in $$S_n$$ is a special permutation which for some subset $$\{a_1,\dots, a_k\}$$ of $$A=\{1,\dots, n\}$$ maps

$$\begin{align}
a_1&\mapsto a_2\\
a_2&\mapsto a_3\\
a_3&\mapsto a_4\\
&\dots\\
a_{k-1}&\mapsto a_k\\
a_k &\mapsto a_1
\end{align}$$

and fixes all the remaining elements of $$A$$.  Notationally, we express this permutation using **cycle notation** $$(a_1\ a_2\ \dots\ a_k)$$.

**Example:**  The $$3$$-cycle $$(1\ 4\ 2)$$ in $$S_4$$ is the same as the permutation

$$\left(\begin{array}{cccc}
1 & 2 & 3 & 4\\
4 & 1 & 3 & 2
\end{array}\right)$$

**Definition:**  Two cycles $$(a_1\ \dots\ a_j)$$ and $$(b_1\ \dots\ b_k)$$ are called **disjoint** if $$a_m\neq b_n$$ for any $$m,n$$.

**Proposition:** If $$\sigma$$ an $$\tau$$ are two disjoint cycles, then $$\sigma\tau = \tau\sigma$$.

**Proposition:**  Every permutation in $$S_n$$ may be expressed as a product of disjoint cycles.  This product is unique up to the order of the cycles.

**Definition:**  A **transposition** is a $$2$$-cycle.

**Proposition:**  Let $$n\geq 2$$.  Any $$k$$-cycle in $$S_n$$  may be written as a product of $$2$$-cycles.  Thus any permutation in $$S_n$$ may be written as a product of two cycles.

The $$2$$-cycle decomposition of a permutation is not unique.  However, the parity is preserved.

**Proposition:** No $$k$$-cycle may be expressed as a product of an even number of $$2$$-cycles and an odd number of $$2$$-cycles.

**Definition:** A permutation is called **even** if it can be written as a product of an even number of $$2$$-cycles.  Otherwise it is called **odd**.  The **sign** of a permutation is given by

$$\sgn(a) = \left\lbrace\begin{array}{cc}
 1 & a\ \text{is even}\\
-1 & a\ \text{is odd}\\
\end{array}\right.$$

**Proposition:** The subset of $$S_n$$ consisting of permutations with even parity is a subgroup, called the **alternating group** and denoted $$A_n$$.
