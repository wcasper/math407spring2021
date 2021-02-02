---
layout: page
title: Relations
---

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



