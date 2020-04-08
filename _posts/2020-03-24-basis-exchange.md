---
title: 'Basis Exchange'
date: 2099-03-25
permalink: /posts/2020/03/basis-exchange/
tags:
  - matroid
  - linear algebra
  - exterior algebra
mathjax: true
---

_Given a subset of a basis, can we choose a subset of another basis so that exchanging them doesn't violate the linear independence of both of them?_

### Prerequisites

- Basic notions in linear algrebra (vector space, basis, etc.)

### Recommended

- Matroid
- Exterior algebra

_**Problem**. Let \\(\mathcal{B}\\) and \\(\mathcal{B'}\\) be bases of a finite dimensional vector space \\(V\\).
Let \\(k\\) be an integer with \\(1\leq k\leq \dim(V)\\). Choose any \\(k\\)-element subset \\(X\\) of \\(\mathcal{B}\\).
Can we choose a \\(k\\)-element subset \\(Y\\) of \\(\mathcal{B'}\\) so that after exchanging \\(X\\) and \\(Y\\),
\\(\mathcal{B}\\) and \\(\mathcal{B'}\\) are still bases of \\(V\\)?_

This problem is formulated in terms of linear algebra, but tackling it is not as easy as basic linear algebra.
In fact, even restricting to a specific case \\(V=\mathbb{R}\\) does not make much difference.

There are at least two ways to approach. This post will present two solutions of the problem.

## Using matroid theory

Readers familiar with [matroids](https://en.wikipedia.org/wiki/Matroid) may notice that this is a generalization of the **basis exchange property**;
if \\(A\\) and \\(B\\) are distinct bases of a matroid \\(M\\) and \\(a\in A\setminus B\\), then there exists \\(b\in B\setminus A\\) such that
\\((A\setminus\left\lbrace a\right\rbrace\cup\left\lbrace b\right\rbrace)\\) is again a basis of \\(M\\).

In fact, there is a weaker generalization of the basis exchange property, called **strong basis exchange property**.

_**Theorem**. _
