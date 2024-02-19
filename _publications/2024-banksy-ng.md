---
title: "BANKSY unifies cell typing and tissue domain segmentation for scalable spatial omics data analysis"
collection: publications
permalink: /publication/2024-banksy-ng
excerpt: "BANKSY is an algorithm with R and Python implementations that identifies both cell types and tissue domains from spatially-resolved -omics data by incorporating spatial kernels capturing microenvironmental information, applicable to a range of spatially-resolved technologies, and scalable to millions of cells.<br/><img src='/images/banksy_fig1.png' height='290' width='270'>"
date: 2022-04-15
venue: 'biorxiv (accepted, Nature Genetics)'
code: 'https://prabhakarlab.github.io/Banksy/'
paperurl: 'https://www.biorxiv.org/content/10.1101/2022.04.14.488259v1.full'
citation: 'Singhal and Chou et al. (2022). &quot;BANKSY: A Spatial Omics Algorithm that Unifies Cell Type Clustering and Tissue Domain Segmentation.&quot; <i>bioarxiv</i>. 1(1).'
---

**Abstract:**

Spatial omics data are clustered to define both cell types and tissue domains. We present Building Aggregates with a Neighborhood Kernel and Spatial Yardstick (BANKSY), an algorithm that unifies these two spatial clustering problems by embedding cells in a product space of their own and the local neighborhood transcriptome, representing cell state and microenvironment, respectively. BANKSY’s spatial feature augmentation strategy improved performance on both tasks when tested on diverse RNA (imaging, sequencing) and protein (imaging) datasets. BANKSY revealed unexpected niche-dependent cell states in the mouse brain and outperformed competing methods on domain segmentation and cell typing benchmarks. BANKSY can also be used for quality control of spatial transcriptomics data and for spatially aware batch effect correction. Importantly, it is substantially faster and more scalable than existing methods, enabling the processing of millions of cell datasets. In summary, BANKSY provides an accurate, biologically motivated, scalable and versatile framework for analyzing spatially resolved omics data.

[](/images/banksy_schematic_1.png)
BANKSY augments cells' transcriptome information with a measure of the transcriptome of their microenvironment. This helps improve both cell type clustering and domain segmentation. See the paper (linked below) for details. 

You can download a preliminary proof copy of the paper [here](/files/41588_2024_1664_Author.pdf), with [Supplementary information](/files/41588_2024_1664_MOESM1_ESM.pdf), and [peer review](/files/41588_2024_1664_MOESM3_ESM.pdf) information. You can also access the Github pages for the [R version](https://prabhakarlab.github.io/Banksy/) and [Python version](https://github.com/prabhakarlab/Banksy_py) of the package, along with [data and scripts](https://zenodo.org/records/10258795) related to the manuscript. 

