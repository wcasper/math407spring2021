---
layout: page
title: Sets
---

The notion of a **set** is the foundation of all of formal mathematics.  Intuitively, a set is a collection of objects (called elements), like the set of all positive real numbers, or the set of all letters in the English alphabet.  However, we cannot explicitly define what a set is, due to introduction of various paradoxes that inevitably result such as [Russell's paradox](https://en.wikipedia.org/wiki/Russell%27s_paradox).  Instead, we pull a very clever run-around by forgoing any definition of what a set is and instead simply describing how it behaves.  These behaviors are encoded in terms of a set of rules called **axioms**.  In this course, we will adopt the ZFC-axomatic system for sets, which includes the axiom of choice.  Furthermore, by and large the intuitive definition of a set will be sufficiently rigorous for the purposes of our presentation.

We assume that students have some familiarity with sets from previous math courses.  Still we present a very brief review of some of the basic notation and ideas.

Examples of sets include

$$
\begin{align*}
A &= \{1,2,3,a,b,c\}\\
B &= \{x: \text{$x$ is a real number and}\ 0\leq x \leq 2\}
\end{align*}
$$

The first set is in list **notation**, where the elements of the set are simply listed out.  The second set is in **set builder notation**, where the elements are determined by a specified condition.  A very important special example of a set is the **empty set** $$\varnothing$$ , which is the set not containing any elements.

We use the notation $$x\in A$$ to mean that $$x$$ is an element of the set $$A$$.  The notation $$A\subseteq B$$ means that $$A$$ is a **subset** of $$B$$, ie that every element of $$A$$ is also an element of $$B$$.

There are several ways of building new sets from old ones by means of various set-theoretic operations.  Important examples include

- **union**

  $$
  A\cup B = \{x:x\in A\ \text{or}\ x\in B\}
  $$

- **intersection**

  $$
  A\cap B = \{x:x\in A\ \text{and}\ x\in B\}
  $$



- **cartesian product**

  $$
  A\times B = \{(x,y): x\in A\ \text{and}\ y\in B\}
  $$

- **power set**

  $$
  \mathcal P(A) = \{C: \text{$C$ is a subset of $A$}\}
  $$



A **partition** of a set $$A$$ is a collection of subsets of $$A$$ whose union forms all of $$A$$.





