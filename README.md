# Unsupervised EM Initialization for Mixture Models: A Complex Network Driven Approach for Modeling Financial Time Series

by
Carlo Mari,
Cristiano Baldassari.

This repository contains the code to reproduce all the results reported in the paper Unsupervised EM Initialization for Mixture Models: A Complex Network Driven Approach for Modeling Financial Time Series.

## Abstract

The EM algorithm is an iterative algorithm very often used to estimate Mixture Models via maximum likelihood. Since the vector of the initial parameters is so critical for the convergence of the algorithm to the best local maximum of the likelihood function, an efficient initialization is required. Our solution to this problem is an unsupervised initialization based on network science. By mapping time series to complex networks using as adjacency matrix the Markov Transition Field associated to the time series, we can connect observed points and discover communities between them. In this way, (i) the number of communities found in the network structure can be matched to the number of the Mixture Model components; (ii) the vector of initial parameters can be directly obtained by the membership of the data points to the discovered communities. An experiment conducted on financial times series with very different characteristics shows that
our approach produces significantly better results if compared to conventional methods of initialization, as K-means and Random, thus demonstrating the effectiveness of the proposed method.

## Reproducing the results

The provided Python [notebook](https://github.com/cbaldassari/gmm_init/blob/main/workflow.ipynb) contains the code that implements the method of initialization we propose in the paper and covers all the steps of the workflow:

![Workflow](https://github.com/cbaldassari/gmm_init/blob/main/img/workflow.png)

## Getting the code
You can download a copy of all the files in this repository by cloning the
[git](https://github.com/cbaldassari/gmm_init) repository:
    git clone https://github.com/cbaldassari/gmm_init
or [download a zip archive](https://github.com/cbaldassari/gmm_init/archive/refs/heads/main.zip).
