
## Overview
This project implements an end-to-end bulk RNA-seq workflow using GEO dataset GSE183947 (Tumor vs Adjacent Normal breast tissue).

## Methods
- Metadata harmonization
- Log2 transformation of FPKM values
- PCA-based quality control
- Differential expression analysis using limma-trend
- FDR correction
- GO enrichment analysis
- Reproducible Quarto reporting

## Key Findings
- 5735 significantly differentially expressed genes (FDR < 0.05)
- Upregulation of MKI67 and KRT19 in tumor samples
- Downregulation of ESR1 in tumor tissue
- Enrichment of proliferation-associated pathways

## Tools
R, tidyverse, limma, pheatmap, clusterProfiler, GEOquery, Quarto

## Data
Data downloaded from:
https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE183947

## How to Run
1. Install required R packages
2. Download GEO supplementary file
3. Render `GSE183947.qmd`