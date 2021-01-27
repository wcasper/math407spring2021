---
layout: page
title: Functions
---

### Functions

Functions are very familiar to us from our exploration in previous math courses.  The true, formal definition of functions is in terms of relations with special properties.

**Definition:** A relation $$f$$ from $$A$$ to $$B$$ is a **function** if it satisfies the property that for every $$a\in A$$ there exists a unique $$b\in B$$ satisfying $$afb$$.  In this case, we usually use a specialized notation $$f: A\rightarrow B$$ to mean $$f$$ is a function from $$A$$ to $$B$$ and write $$f(a)=b$$ in place of $$afb$$.

**Example:**  The relation $$\mathscr R$$ from $$\mathbb Z$$ to $$[0,\infty)$$ defined by saying $$n\mathscr Rx$$ if and only if $$n=x^2$$ is *not* a function.  This is because there is no $$x$$ such that $$-1\mathscr R x$$

**Example:**  The relation $$\mathscr R$$ from $$\mathbb N$$ to $$\mathbb R$$ defined by saying $$n\mathscr Rx$$ if and only if $$n=x^2$$ is *not* a function because there is more than one value of $$x$$ satisfying $$1\mathscr Rx$$, namely $$x=1$$ and $$x=-1$$.

**Example:**  The relation $$\mathscr R$$ from $$\mathbb N$$ to $$[0,\infty)$$ defined by saying $$n\mathscr Rx$$ if and only if $$n=x^2$$ is a function because every $$n$$ has a unique $$x$$ satisfying $$n\mathscr Rx$$.  In this case, we could also have defined the relation in functional notation $$f: \mathbb N\rightarrow [0,\infty]$$ by defining $$f(n)=\sqrt{n}$$.

As we know, we are often interested in various properties of the function, such as injectivity, surjectivity, or bijectivity.

**Definition:** A function $$f: A\rightarrow B$$ is called

- **injective** or **one-to-one** if for all $$a_1,a_2\in A$$ with $$a_1\neq a_2$$ we have $$f(a_1)\neq f(a_2)$$.  In other words, $$f$$ never maps different elements to the same place
- **surjective** or **onto** if for all $$b\in B$$ there exists $$a\in A$$ with $$f(a)=b$$
- **bijective** if it is both injective and surjective





