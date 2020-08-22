---
title: 'Dinic''s Algorithm and Dynamic Trees'
date: 2099-01-30
permalink: /posts/2020/01/dinic-algorithm/
tags:
  - algorithm
  - flow network
  - maximum flow
mathjax: true
---

[Dinic's algorithm](https://en.wikipedia.org/wiki/Dinic%27s_algorithm) is a well-known algorithm
for solving [maximum flow problem](https://en.wikipedia.org/wiki/Maximum_flow_problem).
It is also relatively simple and easy to implement, so it is also widely used in competitive programming.

Dinic's algorithm consists of the following steps. (Detailed definitions are not described in this post.
Please refer to the Wikipedia article for them.)

1. Construct the level graph of the residual graph.
1. If the sink node \(t\) is unreachable, return.
1. Find a blocking flow 
