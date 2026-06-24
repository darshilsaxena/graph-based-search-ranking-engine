# Graph-Based Search Ranking Engine

A C++ implementation of Google's PageRank-inspired ranking algorithm for directed graphs.

## Overview

This project computes node importance scores in large directed graphs using iterative probability propagation. The ranking process is based on the PageRank algorithm, where nodes distribute their current score across outgoing edges until convergence.

## Features

* Directed graph processing
* PageRank computation using iterative updates
* Configurable damping factor
* Dangling node handling
* Convergence-based stopping criterion
* Efficient adjacency-list graph representation

## Algorithm

Each node distributes its rank equally among its outgoing neighbors. During each iteration:

1. Incoming rank contributions are collected.
2. Dangling-node rank is redistributed.
3. Random-jump probability is applied through a damping factor.
4. Iterations continue until convergence.

## Technologies

* C++
* STL
* Graph Algorithms
* Probability-Based Ranking

## Future Improvements

* Document indexing
* Search query support
* Top-K page retrieval
* Visualization of graph rankings
