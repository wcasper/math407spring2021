---
layout: page
title: Cosets
---

## Basic Definition and Examples

Let $$G$$ be a group and $$H$$ be subgroup of $$G$$.

**Definition:** Let $$a\in G$$.  The **left coset of $$H$$ containing $$a$$** is the set

$$aH = \{ah: h\in H\}.$$

The **right coset of $$H$$ containing $$a$$** is the set

$$Ha = \{ha: h\in H\}.$$

**Proposition:** If $$G$$ is abelian, then $$aH = Ha$$ for all $$a\in G$$.

**Notation:** If $$G$$ is abelian with binary relation $$+$$, then we write $$a+H$$ in place of $$aH$$.

**Proposition:** The relations $$\sim_L$$ and $$\sim_R$$ defined by

$$a\sim_L b\quad\text{if and only if}\quad a^{-1}b\in H$$
$$a\sim_R b\quad\text{if and only if}\quad ba^{-1}\in H$$

are both equivalence relations on $$G$$.  The equivalence classes with respect to $$\sim_L$$ are the left cosets of $$H$$ and the equivalence classes with respect to $$\sim_R$$ are the right cosets of $$H$$.


**Example:** Consider the group $$G$$ of symmetries of the square, which consists of the four rotations $$R_0$$, $$R_{\pi/4}$$, $$R_{\pi/2}$$, $$R_{3\pi/4}$$ and the four reflections $$S_0$$, $$S_{\pi/4}$$, $$S_{pi/2}$$, $$S_{3\pi/4}$$.

The left cosets of the subgroup $$H = \{R_0,S_0\}$$ are 
* $$R_0H        = \{R_0,S_0\}$$
* $$R_{\pi/4}H  = \{R_{\pi/4},R_{3\pi/4}\}$$
* $$R_{\pi/2}H  = \{R_{\pi/2},S_{\pi/2}\}$$
* $$R_{3\pi/4}H = \{R_{3\pi/4},S_{\pi/4}\}$$

The right cosets are
* $$HR_0        = \{R_0,S_0\}$$
* $$HR_{\pi/4}  = \{R_{\pi/4},S_{\pi/4}\}$$
* $$HR_{\pi/2}  = \{R_{\pi/2},S_{\pi/2}\}$$
* $$HR_{3\pi/4} = \{R_{3\pi/4},S_{3\pi/4}\}$$

**Example:** Consider the group $$\mathbb Z$$ with the subgroup $$H = 5\mathbb Z$$.  The cosets are
* $$    5\mathbb{Z} = \{\dots,-10,-5,0,5,10,\dots\}$$
* $$1 + 5\mathbb{Z} = \{\dots, -9,-4,1,6,11,\dots\}$$
* $$2 + 5\mathbb{Z} = \{\dots, -8,-3,2,7,12,\dots\}$$
* $$3 + 5\mathbb{Z} = \{\dots, -7,-2,3,8,13,\dots\}$$
* $$4 + 5\mathbb{Z} = \{\dots, -6,-1,4,9,14,\dots\}$$

**Proposition:** For any $$a\in G$$ the cardinality of $$aH$$ and $$Ha$$ is the same as $$H$$

**Lagrange's Theorem:** Let $$H$$ be a subgroup of a finite group $$G$$.  Then the order of $$H$$ divides the order of $$G$$.

**Proof:**  Let $$g_1H,\dots,g_rH$$ be the distinct cosets of $$H$$ in $$G$$.  Then these form a partition of $$G$$ so
$$\lvert G\rvert = \lvert g_1H\rvert + \dots + \lvert g_rH\rvert = r\lvert H\rvert.$$

**Definition:** The **index** $$[G:H]$$ of $$H$$ in $$G$$ is $$\lvert G\rvert / \lvert H\rvert.$$

**Corollary:** Every group of prime order is cyclic.

**Corollary:** The order of any element in a finite group $$G$$ divides the order of $$G$$.


**Theorem:** Suppose that $$K\leq H\leq G$$.  Then

$$[G:K] = [G:H][H:K]$$


