---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a computational biologist at the Genome Institute of Singapore in Dr [Kok Hao Chen's](https://khchenlab.github.io/) lab, where I work on developing new algorithms for spatial multi-omics data analysis. I did my PhD on [system ID](https://thesis.library.caltech.edu/11161/) for models of gene regulation in Professor [Richard Murray's](https://murray.cds.caltech.edu/Main_Page) lab in the Computation and Neural Systems option at Caltech. I did my undergrad in electrical engineering at Imperial. You can find my CV [here](https://vipulsinghal02.github.io/files/vipul_cv.pdf). 

### Recent Projects
We recently developed BANKSY, which is a clustering method for spatially arranged multi-omics data. It uses the omics features of cells, along with their relative spatial locations, to construct a graph in a custom embedding space, which is then clustered using community detection algorithms. The paper will appear in Nature Genetics shortly, and in the meantime, you can read the biorxiv post from a couple of years ago [here](https://www.biorxiv.org/content/10.1101/2022.04.14.488259v1.full), and play with the code [here](https://prabhakarlab.github.io/Banksy/). 

A slightly more theory-based project involves developing parameter consistency conditions for composing dynamical models of systems. The application we have demonstrated it on is the reduction of batch variability in cell free systems, but much more generally, it should be possible prove analogous results for *system composability*. You can read more about this work in the current draft of the [manuscript](/files/Calibration_2024.pdf).

I have also worked on a MATLAB toolbox for modeling and composing genetic circuits, and for performing consensus  parameter inference (multiple datasets / models informing a shared set of parameters) using MCMC. You can read the paper [here](https://academic.oup.com/synbio/article/6/1/ysab007/6129121). 

### Academic interests 
I am currently interested in developing graph deep learning enabled embedding methods for multi-omics data. In some sense, this would generalize BANKSY to multi-omics, and enable the capture of complex patterns in the data. 

I am also interested in developing a description of parameteric uncertainty in models of gene regulatory networks using the theory of differentiable manifolds. I suspect this will enable better composition of subsystems into larger systems, in a way that is robust to parametric uncertainty. To do this, I am working through [Boothby's book](https://shop.elsevier.com/books/an-introduction-to-differentiable-manifolds-and-riemannian-geometry-revised/boothby/978-0-08-057475-2) on differential geometry, and also [Isidori's book](https://link.springer.com/book/10.1007/978-1-84628-615-5), which develops relevant ideas like nonlinear observability. If you are interested in this sort of thing, please feel free to reach out to me via email (on the left). 

In the long run, I am broadly interested in developing and building new AI paradigms for analyzing data in biology and medicine. In particular, I am curious about how high level planning and reasoning is achieved by biological brains using a model of the world, whether this can be built in-silico, and what implication this might have in healthcare and genomics. 