---
layout: page
title: Quotient Groups
---

## Quotients and Normal Subgroups

One of the most useful operations in mathematics is the **quotient**.  Quotients can be found throughout algebra, from rings and modules, to groups and fields.  Here we will focus on the case of groups.

### Products of subsets

If $$X,Y\subseteq G$$ are subsets of a group $$G$$ (not necessarily subgroups), we define

$$XY = \{xy: x\in X,\ y\in Y\}.$$

with this in mind, we have the following characterization of normal subgroups.

**Proposition:** Let $$G$$ be a group and let $$H$$ be a subgroup of $$G$$.  Then $$H$$ is normal if and only if

$$(aH)(bH) = abH,\quad\forall a,b\in G.$$

Thus in this case $$H$$ is a normal subgroup $$(aH)(bH) = abH$$ is a well-define binary relation on the set $$G/H$$ of left cosets of $$H$$ in $$g$$.  In fact, this makes $$G/H$$ into a group with
* binary operation $$aHbH = abH$$
* identity element $$eH$$
* inverse of $$gH$$ given by $$g^{-1}H$$ for $$g\in G$$

**Definition:** Let $$H$$ be a normal subgroup of $$G$$.  The group $$G/H$$ of cosets of $$G$$ called a **quotient group** or **factor group**, and referred to specifically as the **quotient of $$G$$ by $$H$$**.

**Example:**  The group $$\langle n\rangle = n\mathbb Z$$ is a normal subgroup of $$\mathbb Z$$.  The quotient $$\mathbb Z/n\mathbb Z$$ is isomorphic to $$\mathbb Z_n$$.

**Example:**  Let $$V$$ be a vector space over $$\mathbb R$$ with binary operation $$+$$ and let $$W$$ be a subspace of $$V$$.  The quotient group $$V/W$$ is also a vector space, called a **quotient space**.

**Example:**  Let $$A_n$$ be the alternating subgroup of $$S_n$$.  Then $$A_n$$ is a normal subgroup and $$S_n/A_n$$ is isomorphic to $$\mathbb Z_2$$.

If $$H$$ is a normal subgroup of a group $$G$$, then there is a natural group epimorphism

$$G\rightarrow G/H,\quad g\mapsto gH.$$

**Definition:** The above homomorphism is called the **quotient map**.

Via the quotient map, we see that normal subgroups are exactly kernels of group homomorphisms.

**Theorem:**  Let $$H$$ be a subgroup of $$G$$.  Then $$H$$ is a normal subgroup if and only if $$H=\ker(\varphi)$$ for some group homomorphism $$\varphi: G\rightarrow G'$$.

Moreover, the associated quotient group is isomorphic to the image of the group homomorphism.
**Theorem:**  Let $$\varphi: G\rightarrow G'$$ be a group homomorphism.  Then $$\varphi$$ induces an isomorphism

$$\widetilde\varphi: G/\ker(\varphi)\rightarrow \img(\varphi).$$


