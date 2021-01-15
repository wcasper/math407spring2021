---
layout: post
---

## Sets, Relations, and Functions

### Sets

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

### Relations

In mathematics, we are constantly trying to identify patterns and relationships, for example the relationship between $$x$$ and $$y$$-coordinates in a parabola $$y=x^2$$.  As such, it is imperative to have a formal way of describing various relationships.  One very slick way of accomplishing this is via the notion of a relation.

**Definition:** A **relation from a set $$A$$ to a set $$B$$** is a subset $$\mathscr R$$ of the cartesian product $$A\times B$$.  If $$A=B$$, then we say $$\mathscr R$$ is a **relation on $$A$$.$$$$**  Notation-wise, we write $$a\mathscr Rb$$ to mean that $$(a,b)\in\mathscr R$$.

Note that we don't have to use a fancy R to denote a relation.  You can often see relations denoted by $$\sim$$ or $$\equiv$$, or even a letter like $$f$$.  The choice of notation typically depends on the context or on the *kind* of relation we are dealing with.  The tremendous flexibility of the concept of a relation allows is immediately apparent via the very diverse roles they play.  Let's see some examples:

**Example:**  Let $$P$$ be the set of all living people in the world.  We define a relation $$\mathscr R$$ on $$P$$ by saying $$x\mathscr Ry$$ if $$x$$ and $$y$$ have a biological parent in common.  Thus for example (Venus Williams)$$\mathscr R$$(Serena Williams).

**Example:**  Let $$A=\{a,b,c,d\}$$ and $$B = \{1,2,3,4\}$$ and $$\mathscr R = \{(a,3),(b,2),(b,3)\}$$.  Then $$\mathscr R$$ is an equivalence relation from $$A$$ to $$B$$.  For example $$a\mathscr R3$$ and $$b\mathscr R2$$.

**Example:**  Let $$B$$ be the set of all published books.  Define a relation $$\mathscr R$$ from $$B$$ to $$\mathbb N$$ by saying $$x\mathscr R n$$ if and only if $$n$$ is the number of pages in book $$x$$.  

In the special case that $$\mathscr R$$ is an equivalence relation on $$A$$, we are typically interested in three specific properties.  

**Definition:**   We call $$\mathscr R$$ 

- **reflexive** if $$x\mathscr Rx$$ for all $$x\in A$$
- **symmetric** if $$x\mathscr R y$$ implies $$y\mathscr R x$$ for all $$x,y\in A$$
- **transitive** if $$x\mathscr R y$$ and $$y\mathscr R z$$ implies $$x\mathscr R z$$ for all $$x,y,z\in A$$

A relation $$\mathscr R$$ on $$A$$ which is reflexive, symmetric, and transitive is called an **equivalence relation**.  In this case, we define the **equivalence class** of an element $$a\in A$$ to be

$$
[a] = \{x\in A: a\mathscr Rx\}
$$

The set of equivalence classes forms a partition of $$A$$.  In fact, there is a natural one-to-one correspondence between partitions and equivalence classes.  Note that the first example above is actually an example of an equivalence relation.

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





