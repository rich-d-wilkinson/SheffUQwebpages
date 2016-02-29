---
layout: post
title:  "Seminar"
date:   2016-03-03

categories: jekyll update events
---

[Andrew Golightly](http://www.mas.ncl.ac.uk/~nag48/) (University of Newcastle)
**Building bridges: Improved bridge constructs for stochastic differential equations**
Hicks Lecture Theatre C, 2pm

We consider the task of generating discrete-time realisations of a non-linear multivariate 
diffusion process satisfying an Ito stochastic differential equation conditional 
on an observation taken at a fixed future time-point. Such realisations are typically termed 
diffusion bridges. Since, in general, no closed form expression exists for the transition 
densities of the process of interest, a widely adopted solution works with the Euler-Maruyama 
approximation, by replacing the intractable transition densities with Gaussian approximations. 
However, the density of the conditioned discrete-time process remains intractable, necessitating 
the use of computationally intensive methods such as Markov chain Monte Carlo. Designing an 
efficient proposal mechanism which can be applied to a noisy and partially observed system 
that exhibits non-linear dynamics is a particularly challenging problem, and is the focus of this talk. 
By partitioning the process into two parts, one that accounts for non-linear dynamics in 
a deterministic way, and another as a residual stochastic process, we develop a class of 
novel constructs that bridge the residual process via a linear approximation. As well as 
compare the performance of each new construct with a number of existing approaches, we 
illustrate the methodology in a real data application.