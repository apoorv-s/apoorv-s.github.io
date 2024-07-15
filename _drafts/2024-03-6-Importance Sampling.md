---
layout: posts
author: Apoorv Srivastava
date: 2022-01-20
title: Importance Sampling
tag: 2023
category: personal
ExcerptOut: True
Keywords: 
excerpt: 
---

We often want to estimate $\mathbb{E}_P[f(X)]$ for random variable $X$, however, the underlying probability distribution $P_X$ is inacessible. In such cases, we can use a simple trick to evaluate the expectation as
$$
\mathbb{E}_P[f(X)] = \int f(x)P_X(x)dx = \int f(x)\frac{P_X(x)}{Q_X(x)}Q_X(x)dx = \mathbb{E}_Q\Big[f(x)\frac{P_X(x)}{Q_X(x)}\Big]
$$
where $Q_X$ is called the importance density and can be easily evaluated.
