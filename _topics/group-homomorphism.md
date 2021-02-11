---
layout: page
title: Group Homomorphisms
---

## What is a group homomorphism

**Definition:** Let $$G$$ and $$H$$ be groups.  A function $$f: G\rightarrow H$$ is called a **group homomorphism** if

$$f(gh) = f(g)f(h)$$

for all $$g,h\in G$$.

**Example:**

The function

$$f: \mathbb Z_3\rightarrow\mathbb Z_6,\ \ f(n) = 2n$$

is a group homomorphism.

**Example:**

The function

$$f: \mathbb Z_n\rightarrow\mathbb T,\ \ f(k) = e^{2\pi ik/n}$$

is a group homomorphism.


**Definition:** Let $$f:X\rightarrow Y$$ be a function from $$X$$ to $$Y$$, and suppose that $$A\subseteq X$$ and $$B\subseteq Y$$.  The **image** of $$A$$ is the set

$$f(A) = \{y\in Y: \exists\ x\in A\ \text{with}\ y = f(x)\}.$$

In the special case $$A=X$$, we call $$f(X)$$ the **image of $$f$$**, denoted $$\img(f)$$.  The **inverse image** or **preimage** of $$B$$ is the set

$$f^{-1}(B) = \{x\in X: f(x)\in B\}

**Definition:**  Let $$f: G\rightarrow H$$ be a group homomorphism.  The **kernel** of $$f$$ is the inverse image of the identity of $$H$$

$$\ker(f) = f^{-1}(\{e\}) = \{g\in G: f(g)=e\}.$$

**Proposition:**  Let $$f: G\rightarrow H$$ be a group homomorphism.  Then $$\ker(f)$$ is a subgroup of $$G$$ and $$\img(f)$$ is a subgroup of $$H$$.

**Example:**

The function

$$f: \mathbb Z_6\rightarrow\mathbb Z_3,\ \ f(n) = n$$

is a group homomorphism.  The kernel of this group homomorphism is

$$\ker(f) = \{0,3\}.$$

**Proposition:** A group homomorphism $$f: G\rightarrow H$$ is injective if and only if $$\ker(f)=\{e\}$$.

**Definition:** A group homomorphism which is injective is called a **monomorphism**.  One that is surjective is called a **epimorphism**.  If it's bijective, it is an **isomorphism**.

Notice that if $$f: G\rightarrow H$$ is a group monomorphism, then $$f$$ defines an isomorphism from $$G$$ to the subgroup $$\img(f)$$ of $$H$$.


## Cayley's Theorem

**Definition:** A group is called a **group of permutations** if it is a subgroup of $$S_A$$ for some set $$A$$.

**Theorem:** (Cayley's Theorem)  Every group is isomorphic to a group of permutations.

**Proof:**  Let $$G$$ be a group and $$A=G$$ and consider the symmetric group $$S_A$$ of permutations on $$A$$.  For $$g\in G$$, define a function

$$\sigma_g: a\mapsto ga\ \forall\ a\in A.$$

We can check that $$\sigma_g\circ\sigma_{g^{-1}}$$ and $$\sigma_{g^{-1}}\circ\sigma_g$$ are both the identity, so $$\sigma_g$$ is a permutation of $$A$$ with inverse $$\sigma_{g^{-1}}$$.

The function

$$f: G\rightarrow S_A,\ \ f(g) = \sigma_g$$

is a group monomorphism, and thus defines an isomorphism from $$G$$ to a subgroup of $$S_A$$.


