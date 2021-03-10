---
layout: page
title: Quotient Group Examples in the x,y-plane
---

## Quotients of $$\mathbb R^2$$

The real plane $$\mathbb R^2$$ is a group $$G$$ under the binary operation defined by vector addition.  We will explore three examples of quotient subgroups of $$\mathbb R^2$$,relating them to geometric constructions we are already familiar with.

**Example 1:** Let $$G=\mathbb R^2$$ and let $$H$$ be the subgroup

$$H = \{(x,0): x\in \mathbb R\}.$$

Then $$(a,b)+H = (c,d) +H$$ if and only if $$(a-c,b-d)\in H$$, which is true if and only if $$b=d$$.  Thus the unique cosets are given by

$$G/H = \{(0,y) + H: y\in \mathbb R\}.$$

The quotient map $$G\mapsto G/H$$ sends $$(x,y)\mapsto (x,y) + H = (0,y) + H$$.  In this way, we can identify the quotient map with projection onto the $$y$$-axis.

**Example 2:** Let $$G=\mathbb R^2$$ and let $$H$$ be the subgroup

$$H = \{(x,x): x\in \mathbb R\}.$$

Then $$(a,b)+H = (c,d) +H$$ if and only if $$(a-c,b-d)\in H$$, which is true if and only if $$a-c,b-d$$.  In particular $$(x,y) + H = ((x-y)/2,(y-x)/2) +H$$, so that the unique cosets are given by

$$G/H = \{(0,y) + H: y\in \mathbb R\}.$$

The quotient map $$G\mapsto G/H$$ sends $$(x,y)\mapsto (x,y) + H = (0,y-x) + H$$.  In this way, we can identify the quotient map with projection onto the line $$y=-x$$.

**Example 3:** Let $$G=\mathbb R&2$$ and let $$H$$ be the subgroup

$$H = \mathbb Z \times\mathbb Z = \{(m,n): m,n\in \mathbb Z\}.$$

Then $$(a,b) + H = (c,d) + H$$ if and only if $$a-b\in \mathbb Z$$ and $$c-d\in\mathbb Z$$.  Thus the cosets are

$$G/H = \{(a,b) + H: 0\leq a,b < 1\}.$$

Geometrically, this is the same as taking the closed square $$[0,1]\times[0,1]$$ and gluing together points lying across from each other on the edges producing a torus!
