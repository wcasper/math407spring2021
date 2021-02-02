---
layout: page
title: Intuitive notion of a group
---

## Examples of Groups

### Intuition

Fundamentally, a group can be thought of as an abstract way of capturing mathematically a collection of ways that we can "transform" a particular object.  To help make sense of this, think for a second about a deck of playing cards.  We can transform the deck by rearranging the cards.  For example, we can "cut the deck" by switching the top 26 and bottom 26 cards.  Alternatively, to transform the deck we could take all the cards and sort them into their various suits in increasing order, and then stack them back together again.
We put all of these different transformations into a set

$$G = \{g| g\ \text{is a way of rearranging a deck of $52$ cards}\}$$

and this set is what we will call a group.  Formally, what we mean by rearrangments is bijections from the set of $$52$$ playing cards to itself.  The group we just described is a very nice example, called a permutation group.  By studying properties of this group, we can answer very interesting questions such as [how many shuffles does it take to randomize a deck of cards](https://www.ams.org/publicoutreach/feature-column/fcarc-shuffle).

Of course, not every rickety assortment of transformations can be awarded the distinction of being a group.  We have standards after all!  The notion of what should distinguish a group from other sets of transformations arose simultaneously from three different areas of mathematics: symmetries in geometry, solutions of algebraic equations, and number theory.  Thus groups are defined so as to link together shared properties of the objects coming from these diverse subjects.  Informally, we should think of a group $$G$$ as a set of transformations $$G$$ which satisfies the following properties
- the composition of two transformations in $$G$$ (ie. doing one transformation and then another) is in $$G$$
- composition is associative
- every transformation in $$G$$ is reversible by another transformation in $$G$$
In the general setting, we can even drop the idea of the group elements being transformations.  We simply replace the notion of composition with some multiplicative or additive operation.  Later on, we'll describe this as a **binary operation**

Below, we will explore some examples of groups representative of their historical origins.  In the first example, we again deal with a collection of transformations.  In the latter two examples, we think about the more general notion of a group as a set with a way of either multiplying or adding which is sufficiently nice.

