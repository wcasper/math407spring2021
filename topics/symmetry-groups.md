---
layout: page
title: Symmetry groups
---


### Symmetries in geometry
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

