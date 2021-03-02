---
layout: page
title: Simple Groups
---


## Simple Groups and Maximal Normal Subgroups

**Definition:** A group $$G$$ is **simple** if it has no nontrivial proper normal subgroups.

**Example:** The group $$Z_n$$ is simple if and only if $$n$$ is prime.

**Theorem:** The alternating group $$A_n$$ is simple for $$n\geq 5$$.

One of the biggest results in the last hundred years of algebra was the classification of all finite simple groups.  The classification took place in stages, aggregating the work of hundreds of mathematicians between 1950-1980.  The simple groups all turn out to be one of the following:
* cyclic groups of prime order
* alternating group $$A_n$$ for some $$n\geq 5$$
* groups of Lie type (associated with certain Lie groups)
* the Tit's group of order $$17971200$$
* one of $$26$$ other **sporadic groups**, including the **monster group** whose order is $$808017424794512875886459904961710757005754368000000000$$

To give an example of a simple group coming from Lie theory, think about the following example.

**Example:** The group $$G=\text{GL}_n(\mathbb Z_2)$$ is simple.

**Definition:** A normal subgroup $$H$$ Of $$G$$ is a **maximal normal subgroup** if $$H\neq G$$ and for any $$N$$ satisfying $$H\leq N\trianglelefteq G$$ we have $$N=H$$ or $$N=G$$.

**Theorem:** Let $$H\trianglelefteq G$$.  Then $$G/H$$ is simple if and only if $$H$$ is maximal.

**Example:** Since $$S_n/A_n\cong \mathbb Z_2$$ is simple, we know $$A_n$$ is a maximal normal subgroup of $$A_n$$.


