# Single-Cell RNA-seq Analysis of Pancreatic Ductal Adenocarcinoma (PDAC)

## Overview

This project reproduces key components of a published single-cell RNA sequencing (scRNA-seq) study investigating the tumor microenvironment (TME) of pancreatic ductal adenocarcinoma (PDAC) before and after chemotherapy.

The primary objective is to characterize cellular heterogeneity, identify distinct cell populations, and investigate transcriptional differences between untreated and chemotherapy-treated tumor samples.

## Dataset

- **Source:** Publicly available scRNA-seq data from a published PDAC chemotherapy study.
- **Samples analyzed:** 4 patient samples (2 untreated, 2 chemotherapy-treated).
- **Framework:** R and Seurat.

## Analysis Pipeline

1. **Quality Control:** Filtering low-quality cells using gene counts, UMI counts, mitochondrial expression, and erythroid contamination.
2. **Doublet Detection:** Identification and removal of potential doublets using `scDblFinder`.
3. **Normalization:** Library-size normalization followed by log transformation.
4. **Data Integration:** Integration of patient samples using Seurat's anchor-based approach.
5. **Dimensionality Reduction:** Principal Component Analysis (PCA) and UMAP visualization.
6. **Clustering:** Graph-based clustering using the Leiden algorithm.
7. **Cell Type Annotation:** Identification of major cell populations using established marker genes and cluster-specific differential expression.

## Analysis and Visualization

- UMAP visualization of cellular populations.
- Identification of cluster-specific marker genes.
- Feature plots, dot plots, and expression heatmaps.
- Comparison of cellular composition between untreated and treated samples.

## Future Directions

- Differential gene expression analysis between treatment groups.
- Copy number variation inference using `inferCNV` to investigate malignant cell populations.
- Characterization of chemotherapy-associated changes in the tumor microenvironment.

## Tools and Technologies

**R | Seurat | scDblFinder | ggplot2 | Single-Cell RNA Sequencing**

## Acknowledgment

This project is an independent reproduction of a published scRNA-seq analysis for educational and computational research purposes. The original study and its authors are acknowledged for providing the publicly available data and methodology.
