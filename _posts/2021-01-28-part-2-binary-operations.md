---
layout: post
---

## Binary Operators
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

### Multiplication Tables
When $$G$$ is a finite set, we can encode the binary operation of a set $$G$$ in terms of a **multiplication table**.
For example, if $$G = \{0,1,2,3,4\}$$ with binary operator $$a*b = a+_5b$$ then the multiplication table for $$G$$ is

|   | 0 | 1 | 2 | 3 | 4 |
| 0 | 0 | 1 | 2 | 3 | 4 |
| 1 | 1 | 2 | 3 | 4 | 0 |
| 2 | 2 | 3 | 4 | 0 | 1 |
| 3 | 3 | 4 | 0 | 1 | 2 |
| 4 | 4 | 0 | 1 | 2 | 3 |

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
