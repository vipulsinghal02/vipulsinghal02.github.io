---
title: "A MATLAB toolbox for modeling genetic circuits in cell-free systems"
collection: publications
permalink: /publication/2021-txtlsim-oupsb
excerpt: "Txtlsim is a toolbox for simulating cell free reactions using mass action kinetics I this paper, we show how models of subsystems of a circuit can be individually characterized, and composed into the full system, whose behavior can be accurately predicted.<br/><img src='/images/‎txtlsim_summary.png' height='690' width='600'>"
date: 2021-02-05
venue: 'OUP Synthetic Biology'
code: 'https://github.com/vipulsinghal02/txtlsim_buildacell'
paperurl: 'https://doi.org/10.1093/synbio/ysab007'
citation: 'Singhal et al. (2022). &quot;A MATLAB toolbox for modeling genetic circuits in cell-free systems.&quot; <i>Synthetic Biology</i>. Volume 6, Issue 1, 2021, ysab007.'
---

**Abstract:**

We introduce a MATLAB-based simulation toolbox, called txtlsim, for an Escherichia coli-based Transcription–Translation (TX–TL) system. This toolbox accounts for several cell-free-related phenomena, such as resource loading, consumption and degradation, and in doing so, models the dynamics of TX–TL reactions for the entire duration of solution phase batch-mode experiments. We use a Bayesian parameter inference approach to characterize the reaction rate parameters associated with the core transcription, translation and mRNA degradation mechanics of the toolbox, allowing it to reproduce constitutive mRNA and protein-expression trajectories. We demonstrate the use of this characterized toolbox in a circuit behavior prediction case study for an incoherent feed-forward loop.

![](/images/txtlsim_summary.png)
Part characterization and parameter fitting for the incoherent feed-forward loop, followed by prediction of the full system behavior. The txtlsim toolbox can achieve system composability despite parametric undertainty. 
