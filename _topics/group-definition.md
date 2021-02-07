---
layout: page
title: Group
---

## Groups

As we have mentioned and explored thorough various examples, any
group $$G$$ can be thought of as a set of transformations satisfying
* the set is closed under composition
* the identity transformation is in $$G$$
* the inverse of any transformation in $$G$$ is also in $$G$$

To create the formal definition of a group, we abstract these three properties.
The set $$G$$ of transformations is replaced with an arbitrary set and
composition of transformations is replaced by an associative binary operation.
Note that the operation must be associative, since composition is!

The identity transformation corresponds to an element in $$G$$ called an identity element.

**Definition** Let $$G$$ be a set with a binary relation $$*$$.  An **identity
element** of $$G$$ is an  element $$e$$ satisfying $$a*e = e*a = a$$.

Not all binary relations will have identity elements.  Moreover, if it does,
then it has at most one.  This makes since intuitively, since there is only one
identity function also!

**Prop:** Let $$G$$ be a set with a binary relation $$*$$.  If $$e$$ and $$e'$$
are two identity elements of $$G$$, then  $$e=e'$$.

**Proof:** Since $$e$$ is an identity, $$ee' = e'$$.  Also, since $$e'$$ is an
identity, $$ee' = e$$.  Thus $$e=e'$$.


Inverse transformations are now able to be defined in terms of this unique inverse.

**Definition:** Let $$G$$ be a set with a binary relation $$*$$ which has an
identity $$e$$.  An **inverse** of an element $$a\in G$$ is an element $$b\in
G$$ satisfying $$a*b = b*a = e$$.

Just like the identity, inverses are also unique!

**Prop:** Let $$G$$ be a set with a binary relation $$*$$ which as an identity
$$e$$.  If $$b$$ and $$b'$$ are two inverses of $$a\in G$$ then $$b=b'$$.

**Proof:** By definition $$b' = e*b' = b*a*b' = b*e = b$$.

We now have all the tools required to formally define a group!

**Definition** A group is a set $$G$$ with a binary operation $$*$$ satisfying the following properties
* the binary operation is **associative**: $$(a*b)*c = a*(b*c)$$ for all $$a,b\in G$$
* there is an **identity element**: there exists $$e\in G$$ such that $$e*a=a*e = a$$ for all $$a\in G$$
* there are **inverses**: for each $$a\in G$$ there exists $$b\in G$$ with $$a*b = b*a = e$$

**Example:** The set of $$n\times n$$ invertible matrices with binary operation
given by matrix multiplication is a group.  This group is called the **general
linear group of degree $$n$$**.

**Example:** The set $$S_n$$ of permutations of $$\{1,2,\dots,n\}$$ with the
binary operation given by composition is a group.  This group is called the
**symmetric group**.

**Example:** The set of integers $$\{0,1,2,\dots, n-1\}$$ with binary operation $$+_n$$ is a group.

We say that a group $$G$$ is **abelian** if it has the additional property
* the binary operation $$*$$ is commutative: $$a*b = b*a$$ for all $$a,b\in G$$

**Example:** The set $$\mathbb Q$$ of rational numbers with binary operation $$+$$ is an abelian group.

**Example:** The set $$\mathbb Q^\times$$ of nonzero rational numbers with binary operation $$\cdot$$ is an abelian group.



## Almost Groups

Sometimes we end up with objects that are almost, but not quite a group.

**Definition:** A **semigroup** is a set $$G$$ with a binary relation $$*$$ which is associative.

**Definition:** A **monoid** is a semigroup $$G$$ with an identity element $$e$$.

Thus a group is simply a monoid with inverses!

**Example:** The set of $$n\times n$$ matrices with binary operation given by matrix multiplication is a monoid, but not a group.

**Example:** The set of strings of letters in the alphabet with binary operation given by concatenation is a semigroup but not a group.  It is a monoid if and only if we allow the "empty string" to be included.


