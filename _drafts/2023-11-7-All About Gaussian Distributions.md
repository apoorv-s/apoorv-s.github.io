---
layout: posts
author: Apoorv Srivastava
date: 2022-01-20
title: All About Gaussian Distributions
tag: 2023
category: personal
ExcerptOut: True
Keywords: 
excerpt: 
---
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.css" integrity="sha384-zB1R0rpPzHqg7Kpt0Aljp8JPLqbXI3bhnPWROx27a9N0Ll6ZP/+DiW/UqRcLbRjq" crossorigin="anonymous">

## Gaussian Distribution

A random variable (RV) $\mathbf{X} \in \mathbb{R}^n$ is said to be a Gaussian RV if its probability distribution function (PDF) is described by
$$
p(\mathbf{X}) = \frac{1}{\sqrt{(2\pi)^n|\Sigma|}}e^{-(\mathbf{X} - \mathbf{\mu})^\top \Sigma^{-1}(\mathbf{X} - \mathbf{\mu})},
$$

where

### Property 1

Linear transformation is gaussian

Proof.
