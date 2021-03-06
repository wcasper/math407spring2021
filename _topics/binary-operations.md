---
layout: page
title: Binary operations
---

### Basic Definition and Examples
As we mentioned previously, a group is a set where you have some notion of a "product" (eg. multiplication or addition) and where that operation is sufficiently nice.  Mathematically, various products are described by special functions called binary operations.  This language is much nicer, since calling something like addition a product would be very confusing!

**Definition:** Let $$G$$ be a set.  A **binary operation** $$*$$ on $$G$$ is a function $$G\times G\rightarrow G$$ sending a pair of elements $$(a,b)$$ to their **product** $$a*b$$.

**Example:** Let $$G=\mathbb R$$.  Then $$a*b = a+b$$ defines a binary operation on $$G$$.

**Example:** Let $$G=\mathbb R$$.  Then $$a*b = ab$$ defines a binary operation on $$G$$.

**Example:** Let $$G=\mathbb R$$.  Then $$a*b = a-b$$ defines a binary operation on $$G$$.

**Example:** Let $$G$$ be the set of $$5\times 5$$ matrices.  Then setting $$A*B$$ to be the matrix product of the matrices $$A$$ and $$B$$ defines a binary operation on $$G$$.

We do need to be a little careful when we are defining a binary operation $$*$$ on a set $$G$$.  We need to make sure that it is **well defined**, meaning that for any $$a,b\in G$$ the expression $$a*b$$ is defined and unique.  We also need to be sure that $$G$$ is **closed under $$*$$**, meaning that the value of $$a*b$$ also needs to always be in $$G$$.

**Example:** Let $$G=\mathbb R$$.  Then $$a*b = a/b$$ does not define a binary operation on $$G$$, because $$a*0$$ is not defined.  In particular, $$*$$ is not well-defined.

**Example:** Let $$G=\mathbb N$$.  Then $$a*b = a-b$$ does not define a binary operation on $$G$$, because $$2*3=-1$$ is not in $$\mathbb N$$.  In particular, $$G$$ is not closed under $$*$$.

### Properties of Binary Operations
**Definition** A binary operation $$*$$ on a group $$G$$ is called
- **associative** if $$(a*b)*c = a*(b*c)$$ for all $$a,b,c\in G$$
- **commutative** if $$a*b = b*a$$ for all $$a,b\in G$$

For example, $$a*b=a+b$$ and $$a*'b = a-b$$ are two different binary operation on $$\mathbb R$$.  The operation $$*$$ is both associative and commutative, but $$*'$$ is neither associative nor commutative.  In particular

$$\begin{align*}
(1*'1)*'1 &= (1-1)*'1 = 0*'1 = 0-1 = -1\\
1*'(1*'1) &= 1*'(1-1) = 1*'0 = 1-0 = 1.
\end{align*}$$

which shows that $$(1*'1)*'1 \neq 1*'(1*'1)$$.
