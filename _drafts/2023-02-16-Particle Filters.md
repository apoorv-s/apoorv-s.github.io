---
layout: posts
author: Apoorv Srivastava
date: 2022-01-20
title: Particle Filters
tag: 2023
category: personal
ExcerptOut: True
Keywords: 
excerpt: 
---
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.css" integrity="sha384-zB1R0rpPzHqg7Kpt0Aljp8JPLqbXI3bhnPWROx27a9N0Ll6ZP/+DiW/UqRcLbRjq" crossorigin="anonymous">

Filtering, also known as data-assimilation, refers to the process of sequentially refining the state (and/or parameters) from noisy observations of a dynamic system. The mathematical tools that aid this endeavour are called filters. Popular example of filters include Kalman filter and emsemble kalman filter.

For a dynamic system described by 
$$
\tag{1}
\mathbf{x}_k = M(\mathbf{x}_{k-1}) + \mathbf{v}_k \\
\mathbf{y}_k = H(\mathbf{x}_k) + \mathbf{w}_k
$$
With $\mathbf{x}_k$ and $\mathbf{y}_k$ representing the state and the observations at time $t_k$. Term $\mathbf{v}_k$ and $\mathbf{w}_k$ denote the forward model error and observation error respectively. Also, let $\mathbf{X_k} = \{\mathbf{x}_i|i = 0, \dots, k\}$ and $\mathbf{Y}_k = \{\mathbf{y}_i|i = 0, \dots, k\}$ signify the sequence of states of time from $t = 0$ to $t = k$. Filtering problem, in the bayesian context, can then be defined as the process of estimating $f_{X_k | Y_k}$ given $f_{X_{k-1} | Y_{k-1}}$. Using Bayes theorem
$$
\tag{2}
f_{X_k|Y_k} = \frac{f_{Y_k | X_k} f_{X_k}}{f_{Y_k}} = 
$$