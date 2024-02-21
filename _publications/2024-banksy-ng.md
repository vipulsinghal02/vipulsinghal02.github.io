---
title: "BANKSY unifies cell typing and tissue domain segmentation for scalable spatial omics data analysis"
collection: publications
permalink: /publication/2024-banksy-ng
excerpt: "BANKSY is an algorithm with R and Python implementations that identifies both cell types and tissue domains from spatially-resolved -omics data by incorporating spatial kernels capturing microenvironmental information, applicable to a range of spatially-resolved technologies, and scalable to millions of cells.<br/><img src='/images/banksy_fig1.png' height='628' width='495'>"
date: 2022-04-15
venue: 'biorxiv (to appear, Nature Genetics)'
code: 'https://prabhakarlab.github.io/Banksy/'
paperurl: 'https://www.biorxiv.org/content/10.1101/2022.04.14.488259v1.full'
citation: 'Singhal and Chou et al. (2022). &quot;BANKSY: A Spatial Omics Algorithm that Unifies Cell Type Clustering and Tissue Domain Segmentation.&quot; <i>bioarxiv</i>. 1(1).'
---

Spatial omics data involve measurements of both the molecular profiles (such as RNA or protein counts) and the spatial locations of cells. This allows us to measure the arrangement of individual cell types in stereotypical spatial patterns, which is a fundamental property of solid tissues. 

The data resulting from these technologoes are clustered to define both cell types and tissue domains. We present BANKSY, an algorithm that unifies these two spatial clustering problems by embedding cells in a product space of their own and the local neighborhood transcriptome, representing cell state and microenvironment, respectively. 

BANKSY’s spatial feature augmentation strategy improves performance on both tasks, and has been tested on diverse RNA and protein datasets. In particular, BANKSY revealed unexpected niche-dependent cell states in the mouse brain, and outperformed competing methods on domain segmentation and cell typing benchmarks. BANKSY can also be used for quality control of spatial transcriptomics data and for spatially aware batch effect correction. 

Importantly, it is substantially faster and more scalable than existing methods, enabling the processing of million-cell datasets. 

All in all, BANKSY provides an accurate, biologically motivated, scalable and versatile framework for analyzing spatially resolved omics data. The image below gives a high level overview of the feature augmentation strategy taken by BANKSY. 

![](/images/banksy_fig1.png)

BANKSY augments cells' transcriptome information with a measure of the transcriptome of their microenvironment. This helps improve both cell type clustering and domain segmentation. 


<!-- You can download a preliminary proof copy of the paper [here](/files/41588_2024_1664_Author.pdf), with [Supplementary information](/files/41588_2024_1664_MOESM1_ESM.pdf), and [peer review](/files/41588_2024_1664_MOESM3_ESM.pdf) information. You can also access the Github pages for the [R version](https://prabhakarlab.github.io/Banksy/) and [Python version](https://github.com/prabhakarlab/Banksy_py) of the package, along with [data and scripts](https://zenodo.org/records/10258795) related to the manuscript.  -->

