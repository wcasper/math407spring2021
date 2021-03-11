---
layout: page
title: Group Action
---


## G-sets and the Orbit Stabilizer Theorem

**Def:** A **group action** of $$G$$ on a set $$X$$ is a function $$G\times X\rightarrow X$$ defined by $$(g,x)\mapsto g\cdot x$$ with
* $$g\cdot(h\cdot x) = (gh)\cdot x$$ for all $$g,h\in G$$ and $$x\in X$$
* $$e\cdot x = x$$ for all $$x\in X$$

In this case the set $$X$$ is called a $$G$$-set.

**Def:** The **orbit** of an element $$x\in X$$ is 
$$\text{orb}(x) = \{g\cdot x: g\in G\}$$


**Prop:** The relation $$x\sim y$$ if and only if $$x\in \text{orb}(y)$$ defines an equivalence relation on $$X$$. Thus the orbits form a partition of $$G$$.

**Def:** The **isotropy subgroup** or **stabilizer subgroup** of a subset $$S\in X$$ is the subgroup

$$G_S = \{g\in G: g\cdot x= x\ \forall x\in S\}.$$

In the special case $$S = \{x\}$$, we write $$G_x$$ in place of $$G_S$$.

**Orbit-Stabilizer Theorem:**  Let $$G$$ be a group.  Then

$$\lvert G\rvert = \lvert G_x\rvert\cdot\lvert\text{orb}(x)\rvert.$$

More generally, we can use $$X/G$$ to denote the distinct orbits of elements of $$X$$ under $$G$$.

$$\lvert X\rvert = \sum_{[x]\in X/G} \lvert \text{orb}(x) \rvert = \sum_{[x]\in X/G} [G: G_x]$$

We can simplify this by factoring out the subset on which $$G$$ acts trivially

$$X_G = \{x\in X: g\cdot x= x\}.$$

Then we can write

$$\lvert X\rvert = |X_G| + \sum_{[x]\in X/G,\ \lvert \text{orb}(x)\rvert >1 } [G: G_x]$$


## Applications

**Prop:** Suppose that $$G$$ is a group of order $$p^n$$ for some prime $$p$$.  Then $$G$$ has a nontrivial center.

**Corollary:** If $$G$$ has order $$p^2$$ then $$G$$ is abelian.

