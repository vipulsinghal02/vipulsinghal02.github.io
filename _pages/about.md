---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a computational biologist at the Genome Institute of Singapore. I have been working on developing new algorithms for spatial multi-omics data analysis. I studied electrical engineering at Imperial for my undergrad.  During my [PhD](https://thesis.library.caltech.edu/11161/) studies at Caltech, my main focus was on Bayesian parameter inference for models of gene regulation.

### Research interests 
I am currently interested in developing graph deep learning enabled embedding methods for multi-omics data analysis. In some sense, this would generalize our recent neighbourhood augmented clustering method ([BANKSY](https://www.nature.com/articles/s41588-024-01664-3); Singhal, Chou, et al., *Nat. Genet.* 2024) to multi-omics, and enable the capture of complex patterns in the data via augmentation with embeddings learned using graph-based deep learning. 

In the longer term, I am broadly interested in developing and building new ML tools for analyzing data in genomics and medicine. The next set of breakthroughs in AI will come from a better understanding of how (artificial) reasoning can be achieved on structured representations of data or the environment. Tools with such capabilities could have profound implications for genomics and healthcare, by generating insights that respect the logical relationships in the data and literature. 

I am also interested in developing a description of parametric uncertainty in models of gene regulatory networks (and possibly deep neural networks) using ideas from nonlinear control. I suspect this will be the natural language for a theory of system composability in the presence of uncertainty in model parameters. To do this, I am working through Boothby's [excellent book](https://shop.elsevier.com/books/an-introduction-to-differentiable-manifolds-and-riemannian-geometry-revised/boothby/978-0-08-057475-2) on differential geometry, and [Isidori's book](https://link.springer.com/book/10.1007/978-1-84628-615-5), which develops relevant ideas like nonlinear observability.

### Recent Projects
We developed BANKSY, which is a clustering method for spatially arranged multi-omics data. It uses the omics features of cells, along with their relative spatial locations, to construct a graph in a custom embedding space, which is then clustered using community detection algorithms. The [paper](https://www.nature.com/articles/s41588-024-01664-3) was published recently, and you may find the [code](https://prabhakarlab.github.io/Banksy/) and [twitter thread](https://x.com/shyam_lab/status/1762648072360792479?s=20) helpful, along with a high level overview [here](/files/banksy-news.pdf). 

A [project](/files/Calibration_2024.pdf) that merges ideas from synthetic and systems biology involves developing parameter consistency conditions for composing dynamical models of systems. The application we have demonstrated it on is the reduction of batch variability in cell-free systems, which are used as prototyping platforms for genetic circuits. More generally, it should be possible prove analogous results for *system composability*, and will be a future direction of research. 

I have also worked on a [MATLAB toolbox](https://academic.oup.com/synbio/article/6/1/ysab007/6129121) for modeling and composing genetic circuits, and for performing consensus  parameter inference (multiple datasets / models informing a shared set of parameters) using MCMC. 


