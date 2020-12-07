# Gastrulation analysis

This repository contains all analysis files for the reproducibility of the single-cell RNAsequencing data analysis results presented in Scheibner et al.

Raw counts matrices and velocyto loom files are available on GEO with accession code GSE162534. We organized the analysis in jupyter notebooks:

* 1_preprocessing.ipynb presents the quality control with cell and gene filtering, normalization and batch effect correction.
* 2_clustering_annotation.ipynb shows the annotation of the data based on louvain clustering and marker genes. 
* 3_differential_expression_pEpi.ipynb determines differentially expressed genes in the posterior epiblast with respect to epiblast and endoderm lineage, resp.
* 4_pseudotime.ipynb shows the gene dynamics of selected genes towards the mesoderm and endoderm lineage.
