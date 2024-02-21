---
title: "DUBStepR is a scalable correlation-based feature selection method for accurately clustering single-cell data"
collection: publications
permalink: /publication/2021-dubstepper-natcom
excerpt: "DUBStepR is a feature selection method for spatial transcriptomics data, relying on the intuition of finding the most informative features, given the set of features already identified.<br/><img src='/images/‎dubsteppr_fig1.png' height='690' width='600'>"
date: 2021-10-06
venue: 'Nature Communications'
code: 'https://github.com/prabhakarlab/DUBStepR'
paperurl: 'https://doi.org/10.1038/s41467-021-26085-2'
citation: 'Ranjan, B. et al. &quot;DUBStepR is a scalable correlation-based feature selection method for accurately clustering single-cell data.&quot; <i>Nat. Commun.</i>. 12, 5849 (2021).'
---

**Abstract:**
Feature selection (marker gene selection) is widely believed to improve clustering accuracy, and is thus a key component of single cell clustering pipelines. Existing feature selection methods perform inconsistently across datasets, occasionally even resulting in poorer clustering accuracy than without feature selection. Moreover, existing methods ignore information contained in gene-gene correlations. Here, we introduce DUBStepR (Determining the Underlying Basis using Stepwise Regression), a feature selection algorithm that leverages gene-gene correlations with a novel measure of inhomogeneity in feature space, termed the Density Index (DI). Despite selecting a relatively small number of genes, DUBStepR substantially outperformed existing single-cell feature selection methods across diverse clustering benchmarks. Additionally, DUBStepR was the only method to robustly deconvolve T and NK heterogeneity by identifying disease-associated common and rare cell types and subtypes in PBMCs from rheumatoid arthritis patients. DUBStepR is scalable to over a million cells, and can be straightforwardly applied to other data types such as single-cell ATAC-seq. We propose DUBStepR as a general-purpose feature selection solution for accurately clustering single-cell data.

![](/images/dubsteppr_fig1.png)
