---
layout: post
title:  "Seminar"
date:   2017-10-11

categories: jekyll update events
---

[Ed Ryan](http://www.lancaster.ac.uk/lec/about-us/people/edmund-ryan) (Lancaster)
**Calibrating a global atmospheric chemistry transport model using a Gaussian process emulator and measurements of surface ozone and surface CO**
Hicks J11, 2-3pm


Atmospheric chemistry transport models (CTMs) simulate the production, loss and transport of hundreds of gases in the atmosphere.  They are used to make local, regional and global short-term forecasts of air quality.  They are also used for more long-term forecasts to understand how reducing, increasing or maintaining the emissions of greenhouse gases affects the atmsopheric chemistry composition.  To ensure that these models are accurate representations of reality we compare their predictions of gas concentrations with measurements.  A more formal statistical approach, called model calibration, involves using algoirthms like history matching or MCMC to find areas of the model's parameter space where the agreement between the model and measurements is acceptable.  For computationally expensive models, such as a CTM which typically takes 12 hours to simulate 1 year, we use a much faster running Gaussian process emulator as a surrogate of the CTM.  In this talk, I describe results of using MCMC to estimate the posterior distribution of parameters from a CTM called FRSGC/UCI, using measurements of surface ozone and surface CO from locations in North America and Europe. Using both synthetic and real measurements, I investigate how the posterior distribution of the parameters changes when: (1) varying the uncertainty and spatial coverage of the measurements; (2) using both surface ozone and surface CO as two different measurement constaints, instead of just one of them as a single constraint.