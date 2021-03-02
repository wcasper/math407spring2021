---
layout: page
title: Quotient Group Examples
---

## Quotients Group Examples

For many of these examples, we will use the following result.

**Proposition:** Let $$H\leq G$$.  Then $$ghH=gH$$ for all $$h\in H$$.


**Example:** Let $$G=\mathbb Z_4\times\mathbb Z_6$$ and $$H=\langle(2,3)\rangle$$.  The quotient group $$G/H$$ is an abelian group of order $$24/2=12$$.  From the structure theorem, we know that $$G/H$$ should be isomorphic to either $$\mathbb Z_{12}$$ or else $$\mathbb Z_2\oplus\mathbb Z_6$$.

Which is it?  Notice that if $$G/H\cong \mathbb Z_2\oplus\mathbb Z_6$$, then $$6G/H = \{(0,0)+H\}$$.  However we see

$$6((1,1) + H) = (6,6) + H = (2,0) + H \neq (0,0) + H$$

Therefore $$G/H\cong \mathbb Z_{12}$$.  In particular it is cyclic!  In fact, one can check that $$(1,1)+H$$ is a generator for $$G/H$$.

To get a specific isomorphism from $$G/H$$ to $$\mathbb Z_{12}$$ we can consider the homomorphism

$$\varphi: G/H\rightarrow\mathbb Z_{12},\ \ \varphi(m,n) = 3m-2n.$$

This is surjective with  kernel $$H$$, so $$\varphi$$ defines an isomorphism $$G\rightarrow G/H$$.

**Example:** Let $$G=\mathbb Z\oplus \mathbb Z\oplus \mathbb Z$$ and $$H=\langle(1,1,1)\rangle$$.  Then $$H$$ is the kernel of the group epimorphism

$$\varphi: \mathbb Z\oplus\mathbb Z\oplus\mathbb Z\rightarrow\mathbb Z\oplus\mathbb Z, (a,b,c)\mapsto (a-b,b-c).$$

Consequently $$G/H\cong \mathbb Z\oplus\mathbb Z$$.

**Example:** Let $$G=\mathbb Z_4\oplus\mathbb Z_4\oplus\mathbb Z_8$$ and $$H=\langle(1,2,4)\rangle$$.  Then

$$(a,b,c) + H = (a,b,c) - a(1,2,4) + H = (0,b-2a,c-4a) + H$$

in other words in $$G/H$$ we can ``get rid" of the first entry.  In this way, it looks like $$G/H$$ will be isomorphic to $$\mathbb Z_4\oplus\mathbb Z_8$$.  In fact we can show this via the epimorphism

$$\varphi: G\rightarrow \mathbb Z_{4}\oplus\mathbb Z_8,\ \ (a,b,c)\mapsto (b-2a,c-4a)$$

The kernel of this map is $$H$$ so it defines an isomorphism between $$G$$ and $$\mathbb Z_4\oplus\mathbb Z_8$$.

