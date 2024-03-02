---
title: "BANKSY unifies cell typing and tissue domain segmentation for scalable spatial omics data analysis"
collection: publications
permalink: /publication/2024-banksy-ng
excerpt: "BANKSY is an algorithm with R and Python implementations that identifies both cell types and tissue domains from spatially-resolved -omics data by incorporating spatial kernels capturing microenvironmental information, applicable to a range of spatially-resolved technologies, and scalable to millions of cells.<br/><img src='/images/banksy_fig1.png' height='628' width='495'>"
date: 2024-02-27
venue: 'Nature Genetics'
code: 'https://prabhakarlab.github.io/Banksy/'
paperurl: 'https://www.nature.com/articles/s41588-024-01664-3'
citation: 'Singhal, V., Chou, N., Lee, J. et al. (2024). &quot;BANKSY unifies cell typing and tissue domain segmentation for scalable spatial omics data analysis.&quot; <i>Nat Genet</i>.'
---

Spatial omics data involve measurements of both the molecular profiles (such as RNA or protein counts) and the spatial locations of cells. This allows us to measure the arrangement of individual cell types in stereotypical spatial patterns, which is a fundamental property of solid tissues. 

The data resulting from these technologoes are clustered to define both cell types and tissue domains. BANKSY is an algorithm that unifies these two spatial clustering problems by utilizing a biologically motivated feature augmentation strategy. Cells are embedded in a product space of their own and the local neighborhood transcriptome, representing cell state and microenvironment respectively.

The neighbourhood is encoded using the local mean transcriptome, and local neighbourhood gradients computed using the azimuthal Gabor filter (AGF), weighted by a mixing parameter, lambda. The AGF is like the traditional plane wave Gabor filter used to quantify texture in image processing, but computed in the azumuthal (polar) coordinates around each cell, and modulated with a Gaussian waveform.

![](/images/banksy_fig1.png)

Cell typing I: When reference data is not available, BANKSY can provide an accurate unsupervised alternative to reference-based deconvolution methods like RCTD for labeling Slide-seq data, which tends to have measurement noise due to contamination between adjacent spots: 

![](/images/banksy-image4.png)

The idea behind this ‘denoising’ effect is that lifting cells to BANKSY’s higher-dimensional neighour-augmented space can be used to disambiguate cell identities. This is because similar cells tend to have similar microenvironments, and so the separation along the neighborhood axis helps separate the cells better:

![](/images/banksy-image10.png)

Cell typing II: BANKSY can also be used to identify niche dependent cell subtypes. Cell types residing in distinct microenvironments can can have subtly distinct transcriptomes. BANKSY stratified mature oligodendrocytes in mouse hypothalamus MERFISH data into white matter (anterior commissure) and grey matter (general hypothalamic area) subpopulations, which were corroborated in matching scRNA-seq data (panel e)

![](/images/banksy-image5.png)

Cell typing III: In a MERSCOPE neoplastic human colon tumor dataset, BANKSY resolved intermingled mesenchymal and immune cell types, and identified cycling epithelial cells that could not be identified using nonspatial clustering (blue cells in h).

![](/images/banksy-inage12.png)

Domain Segmentation: Performs domain segmentation when neighbourhood expression is upweighted: on the CODEX spatial proteomics data of human intestine, it identifies a CD66+ mature epithelial community and an α-smooth muscle actin-expressing community not found by non-spatial clustering, verified by marker expression:

![](/images/banksy-inage6.png)

Importantly, it is substantially faster and more scalable than existing methods, enabling the processing of million-cell datasets. 

![](/images/banksy-inage9.png)

Generality: can even be used for spatial batch correction, and outperforms other methods, including another method’s batch correction strategy https://bit.ly/48w9dX2 

![](/images/banksy-inage8.png)

Robustness: works at default param settings across diverse data types. Also: robust to random number seed. 
![](/images/banksy-inage1.png)

Salas et al. (https://bit.ly/4bRYfxR) and Ren et al. (https://bit.ly/3wDsubK) independently benchmarked and recommended BANKSY, and Shamir et al. (https://bit.ly/3wuRjH5) showed it works even on brain MRI data. 

![](/images/banksy-image2.png)

All in all, BANKSY provides an accurate, biologically motivated, scalable and versatile framework for analyzing spatially resolved omics data. The image below gives a high level overview of the feature augmentation strategy taken by BANKSY. 