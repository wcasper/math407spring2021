---
layout: post
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

### More examples of groups
#### Symmetries in geometry
To begin, let's think about the filled-in square $$\mathcal S = [-1,1]\times[-1,1]$$ centered at the origin.  A **(linear) symmetry** of $$\mathcal S$$ is a linear transformation $$T: \mathbb R^2\rightarrow\mathbb R^2$$ which maps $$\mathcal S$$ to itself.  For example, rotations are linear transformations and rotation by $$90$$ degrees preserves the square, so a $$90$$-degree clockwise rotation is a symmetry of $$\mathcal S$$.  This transformation can be represented as a function

$$T(x,y) = (y,-x)$$

or in terms of a $$2\times 2$$ matrix

$$\left(\begin{array}{cc}
0& 1\\
-1 & 0
\end{array}\right).$$

The set $$G$$ of all symmetries of $$\mathcal S$$ consists (in matrix notation) of
- identity

$$
\left(\begin{array}{cc}
1 & 0\\
0 & 1
\end{array}\right)
$$

- rotations

$$
\left(\begin{array}{cc}
0& 1\\
-1 & 0
\end{array}\right),\quad
\left(\begin{array}{cc}
-1& 0\\
 0&-1
\end{array}\right),\quad
\left(\begin{array}{cc}
0&-1\\
1 & 0
\end{array}\right)
$$

- reflections

$$
\left(\begin{array}{cc}
1 & 0\\
0 &-1
\end{array}\right),\quad
\left(\begin{array}{cc}
-1& 0\\
 0& 1
\end{array}\right),\quad
\left(\begin{array}{cc}
0 & 1\\
1 & 0
\end{array}\right),\quad
\left(\begin{array}{cc}
 0 & -1\\
-1 & 0
\end{array}\right).
$$

This collection of $$8$$ matrices forms a group, sometimes called the **dihedral group** $$D_4$$.  More generally, one can consider the group of symmetries of an $$n$$-gon on the plane, obtaining the dihedral group $$D_n$$.  In fact, we can extend this to higher dimensions and consider the symmetry groups of various polytopes, forming even more interesting groups.

#### Solutions of algebraic equations
Consider the set $$G$$ of complex-valued solutions of an algebraic equation $$z^n=1$$.  If $$z=a$$ is a solution (ie. $$a^n=1$$), and $$z=b$$ is also a solution, then $$(ab)^n = a^nb^n=1\cdot 1 = 1$$ and therefore $$z = ab$$ is also a solution.  Furthermore if $$a\in G$$ then $$(1/a)^n = 1/a^n = 1$$ and so $$z=1/a$$ is a solution.  In other words, if $$a,b\in G$$ then $$ab\in G$$ and if $$a\in G$$ then $$a^{-1}\in G$$.  Thus $$G$$ is a group.

More generally, we can think about the set of roots of any polynomial equation $$p(z) = 0$$.  Associated to any such equation is a very special group called the [Galois Group](https://en.wikipedia.org/wiki/Galois_group), which we will discuss later in this course.

#### Number theory
One of the foundations of number theory is a clockwork-style addition for numbers called **modular arithmetic**.  To begin, fix a positive integer $$n$$ and consider the set

$$\mathbb Z_n = \{0,1,2,3,\dots,n-1\}.$$

We define **modular addition** on $$\mathbb Z_n$$ by setting

$$a +_n b = \text{remainder after dividing $a+b$ by $n$}.$$

This makes $$\mathbb Z_n$$ into a group.  So for example

$$\begin{align*}
2 +_5 3 &= 0\\
8 +_2 5 &= 1\\
4 +_7 9 &= 6.
\end{align*}$$

Note: the notation we use here is consistent with Fraleigh's text, but is not the usual notation for this operation.  The latter is typically framed in terms of the notion of a **quotient group**, a topic of later discussion.

This kind of weird addition is actually very intuitive if we think about how hours work on a clock.  If it's currently 10:00 then in three hours it will be 1:00.  Fourteen hours after that, it will be 3:00.  Thus mathematically, we're discovring that clock-addition works just like addition modulo $$12$$:

$$\begin{align*}
10 +_{12} 3 = 1\\
1 +_{12} 14 = 3
\end{align*}$$

We can also define a continuous form of modular addition for real numbers.  Fix a positive real number $$r>0$$ and consider the set

$$\mathbb R_r = [0,r).$$

We define modular addition on $$\mathbb R_r$$ by setting

$$a+_rb = \left\lbrace\begin{array}{cc}
a+b, & \text{if $a+b<r$}\\
a+b-r, & \text{if $a+b\geq r$}
\end{array}\right.$$

Thus for example

$$\begin{align*}
\sqrt{2} +_3 2 &= \sqrt{2}-1\\
4.3 +_5 + 2.1 &= 1.4
\end{align*}$$

This defines a group, and we can look to the unit circle for intuition.  In the unit circle, if we have an angle of $$7\pi/4$$ radians and then we add $$\pi/2$$ radians, then we have gone one full circle ($$2\pi$$ radians), plus a bit extra, ending up at $$\pi/4$$ radians.  In other words, radians in the unit circle work like modular addition modulo $$2\pi$$.

$$7\pi/4 +_{2\pi} \pi/2 = \pi/4.$$

For this reason, we often identify $$\mathbb R_{2\pi}$$ with the unit circle.
