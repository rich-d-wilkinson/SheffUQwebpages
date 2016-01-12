---
layout: default
---

# GPy
In 2010 I started working on GPy. Based in part on Neil Lawrence's matlab code, I started to make a framework for Gaussian processes in python. The aim was to facilitate reproducible research, and to give myself a platform to build future work on, with things like automatic gradient-checking built in.

Now GPy has evolved into much more than that. With the contribution of other lab members, we began to build a platform that can be used for research and teaching.

Check out the code on [github](http://github.com/sheffieldml/gpy)

# GPclust
GPclust contains effiecient code for clustering time series using Gaussian processes. It's based on a modification to the VBEM algorithm that I wrote about [here](http://papers.nips.cc/paper/4766-fast-variational-inference-in-the-conjugate-exponential-family), and builds on GPy. There are [notebook tutorials](https://github.com/jameshensman/GPclust/blob/master/notebooks/index.ipynb) to go with the [open source code](https://github.com/jameshensman/GPclust/)



# Hierarchical GPs
It's possible to extend Gaussian processes into hierarchical structures to model groupings in data. The linear-Gaussian mature of the model means that the whole thing is still a Gaussian process: I wrote about this in [BMC Bioinformatics](http://www.biomedcentral.com/1471-2105/14/252). 
I've incorporated the code for this paper into GPy. I've created an IPython notebook to show how to [apply these ideas](https://github.com/SheffieldML/notebook/blob/master/compbio/Hierarchical.ipynb)

# Variational Inference
In 2012 I wrote about a method for doing [fast optimization in Variational Bayes problems](). It's a generally applicable method, so I've used the code for other models also. You can find the code on [github](githib.com/sheffieldml/colvb).

# RNA Transcript Quantification (BitSeq)
Variational inference is useful across so many domains: we've recently shown how it can be aplied to count molucues from high-throuput sequencing. The paper is [here](http://bioinformatics.oxfordjournals.org/content/early/2015/09/04/bioinformatics.btv483.full.pdf+html) and the code is now part of the BitSeq project, [here](https://www.bioconductor.org/packages/release/bioc/html/BitSeq.html).

