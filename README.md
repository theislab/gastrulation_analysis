# Gastrulation analysis

This repository contains all analysis files for the reproducibility of the single-cell RNAsequencing data analysis results presented in Scheibner et al., "Epithelial cell plasticity drives endoderm formation during gastrulation" (2021) - please consider citing this paper, if you find this collection of notebooks useful.

Raw counts matrices and velocyto loom files are available on GEO with accession code GSE162534. We organized the analysis in jupyter notebooks:

* 1_preprocessing.ipynb presents the quality control with cell and gene filtering, normalization and batch effect correction.
* 2_clustering_annotation.ipynb shows the annotation of the data based on louvain clustering and marker genes. 
* 3_differential_expression_pEpi.ipynb determines differentially expressed genes in the posterior epiblast with respect to epiblast and endoderm lineage, resp.
* 4_pseudotime.ipynb shows the gene dynamics of selected genes towards the mesoderm and endoderm lineage.
* 5_RNAvelocity.ipynb computes the dynamic RNA velocity model (with separate data pre-processing).
* 6_cellrank.ipynb computes cell fate probabilities based on the RNA velocity information
* 7_final_visualisation.ipynb contains a summary of final plots for publication.

A short guide to the figures displayed in the manuscript:

Figures:
* 1h - fate probability pie charts on UMAP (6_cellrank)
* 1i - lineage drivers (6_cellrank)
* 1j - stacked violin plot tissue markers (7_final_visualisation)

* 3a - heatmap Wnt signalling mesoderm - pEpi - TP - ADE (7_final_visualisation)
* 3b - lineplot (4_pseudotime)

* 4a - heatmap delamination (7_final_visualisation)
* 4b - lineplot (4_pseudotime)

Extended Data Figures:
* 2b - UMAP tissues (2_clustering_annotation)
* 2c - dotplot marker genes (7_final_visualisation)
* 2d - stream plot Foxa2 mRNA + FVF sorting (6_ellrank)
* 2e - scVelo metastable states (6_cellrank)
* 2f - barplots fate probability (6_cellrank)
* 2g - UMAP gene expression (Cdh1, Cdh2, Snail1, T, Foxa2) (7_final_visualisation)

* 8g - UMAP with Foxa2+/- pEpi (3_differential_expression_pEpi)
* 8h - stacked violin for pEpi and Epi (7_final_visualisation)
* 8i - stacked violin for Foxa2+/- pEpi (7_final_visualisation)

