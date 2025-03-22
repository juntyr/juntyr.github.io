---
title: "Communication-free and Parallel Simulation of Neutral Biodiversity Models"
collection: publications
category: theses
permalink: /publication/2021-06-14-necsim-rust
excerpt: 'necsim-rust implements a novel communication-free algorithm for individual-based probabilistic neutral biodiversity simulations.'
date: 2021-06-14
venue: 'Imperial College London'
paperurl: 'https://arxiv.org/abs/2108.05815'
citation: '<b>Tyree, J.</b> (2021) <i>Communication-free and Parallel Simulation of Neutral Biodiversity Models</i>. Master’s Thesis. Available from: <a href="https://doi.org/10.48550/arXiv.2108.05815">doi:10.48550/arXiv.2108.05815</a>.'
---

* Supervisors:
  * Dr Anthony Field, Imperial College London
  * Dr James Rosindell, Imperial College London
  * Prof. Ryan A. Chisholm, National University of Singapore

## Abstract

We present a novel communication-free algorithm for individual-based probabilistic neutral biodiversity simulations. The algorithm transforms a neutral Moran ecosystem model into an embarrassingly parallel problem by trading off inter-process communication at the cost of some redundant computation.

Specifically, by careful design of the random number generator that drives the simulation, we arrange for evolutionary parent-child interactions to be modelled without requiring knowledge of the interaction, its participants, or which processor is performing the computation. Critically, this means that every individual can be simulated entirely independently. The simulation is thus fully reproducible irrespective of the number of processors it is distributed over. With our novel algorithm, a simulation can be (1) split up into independent batch jobs and (2) simulated across any number of heterogeneous machines - all without affecting the simulation result.

We use the Rust programming language to build the extensible and statically checked simulation package `necsim-rust`. We evaluate our parallelisation approach by comparing three traditional simulation algorithms against a CPU and GPU implementation of our Independent algorithm. These experiments show that as long as some local state is maintained to cull redundant individuals, our Independent algorithm is as efficient as existing sequential solutions. The GPU implementation further outperforms all algorithms on the CPU by a factor ranging from ∼2 to ∼80, depending on the model parameterisation and the analysis that is performed. Amongst the parallel algorithms we have investigated, our Independent algorithm provides the only non-approximate parallelisation strategy that can scale to large simulation domains.
