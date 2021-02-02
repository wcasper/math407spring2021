---
layout: page
title: Multiplication table
---

When $$G$$ is a finite set, we can encode the binary operation of a set $$G$$ in terms of a **multiplication table**.
For example, if $$G = \{0,1,2,3,4\}$$ with binary operator $$a*b = a+_5b$$ then the multiplication table for $$G$$ is

|   | 0 | 1 | 2 | 3 | 4 |
| 0 | 0 | 1 | 2 | 3 | 4 |
| 1 | 1 | 2 | 3 | 4 | 0 |
| 2 | 2 | 3 | 4 | 0 | 1 |
| 3 | 3 | 4 | 0 | 1 | 2 |
| 4 | 4 | 0 | 1 | 2 | 3 |

The entry in the $$i$$'th row and $$j$$'th column represents the product $$a*b$$ of the left-most entry $$a$$ in the $$i$$'th row with the upper-most entry $$b$$ in the $$j$$'th column.  Note that this multiplication order is important when the group is **non-abelian**, meaning that the binary operation $$*$$ is not commutative.

As another example, consider the symmetry group of an isosceles triangle.  In terms of $$2\times 2$$ matrices, it consists of
* three rotation matrices

$$
R_0        = \left(\begin{array}{cc}1&0\\0&1\end{array}\right),\quad 
R_{2\pi/3} = \left(\begin{array}{cc}\frac{1}{2}&-\frac{\sqrt{3}}{2} \\ \frac{\sqrt{3}}{2}&\frac{1}{2}\end{array}\right),\quad
R_{4\pi/3} = \left(\begin{array}{cc}\frac{1}{2}& \frac{\sqrt{3}}{2} \\-\frac{\sqrt{3}}{2}&\frac{1}{2}\end{array}\right)
$$

* three reflection-rotation matrices

$$
S_0        = \left(\begin{array}{cc}-1&0\\0&1\end{array}\right),\quad 
S_{2\pi/3} = \left(\begin{array}{cc}-\frac{1}{2}&\frac{\sqrt{3}}{2} \\ \frac{\sqrt{3}}{2}&\frac{1}{2}\end{array}\right),\quad
S_{4\pi/3} = \left(\begin{array}{cc}-\frac{1}{2}&-\frac{\sqrt{3}}{2} \\-\frac{\sqrt{3}}{2}&\frac{1}{2}\end{array}\right)
$$

The multiplication table for this group is

|                | $$R_0$$        | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ |
| $$R_0$$        |  $$R_0$$       | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ |
| $$R_{2\pi/3}$$ | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$R_0$$        | $$S_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ |
| $$R_{4\pi/3}$$ | $$R_{4\pi/3}$$ | $$R_0$$        | $$R_{2\pi/3}$$ | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ | $$S_0$$        |
| $$S_0$$        | $$S_0$$        | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ | $$R_0$$        | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ |
| $$S_{2\pi/3}$$ | $$S_{2\pi/3}$$ | $$S_{4\pi/3}$$ | $$S_0$$        | $$R_{4\pi/3}$$ | $$R_0$$        | $$R_{2\pi/3}$$ |
| $$S_{4\pi/3}$$ | $$S_{4\pi/3}$$ | $$S_0$$        | $$S_{2\pi/3}$$ | $$R_{2\pi/3}$$ | $$R_{4\pi/3}$$ | $$R_0$$        |

The fact that this group is not abelian is reflected in the structure of the multiplication table above.  In particular it is not symmetric.

