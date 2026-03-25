# BioPath Perturbation Analysis using GEO Dataset (GSE15852)

## Overview

This project focuses on analyzing biological pathway perturbations using real gene expression data from the GEO database (GSE15852). The aim is to identify key differences between cancer and normal samples and understand how these differences affect biological pathways.

This work combines machine learning and statistical analysis to extract meaningful biological insights from high-dimensional genomic data and serves as a foundation for pathway-level analysis using frameworks such as Reactome and MP-BioPath.

---

## Objectives

* Analyze gene expression patterns in cancer vs normal samples
* Identify differentially expressed genes (DEGs)
* Perform dimensionality reduction and clustering
* Apply statistical methods for gene significance
* Visualize patterns using advanced plots
* Interpret biological relevance of findings
* Establish a foundation for pathway-level perturbation analysis

---

## Dataset

* Source: NCBI GEO
* Accession: GSE15852
* Type: Microarray gene expression dataset
* Samples: Breast cancer vs normal tissues
* Genes: ~22,000

This is a research-grade dataset widely used in bioinformatics studies.

---

## Methodology

### Data Preprocessing

* Removed metadata and missing values
* Converted gene expression values into numeric format
* Prepared dataset for machine learning analysis

### Dimensionality Reduction (PCA)

* Reduced high-dimensional gene data into 2D space
* Enabled visualization of separation between cancer and normal samples

### Clustering (K-Means)

* Grouped samples into clusters
* Verified biological grouping patterns

### Differential Expression Analysis

* Applied statistical t-test
* Computed fold change for each gene
* Ranked genes based on significance and expression difference

### Pathway-Level Perspective

Significant genes identified in this analysis can be mapped to biological pathways using databases such as Reactome. This provides a basis for integrating with tools like MP-BioPath to study pathway perturbations at a systems level.

---

## Visualizations

The project includes multiple visualization techniques for better understanding:

* PCA plot → shows separation between sample groups
* Clustering plot → shows grouping structure
* Heatmap → highlights gene expression variation
* Volcano plot → shows significance vs fold change
* Correlation heatmap → reveals gene relationships
* Fold change distribution → overall gene variation
* Top gene plot → highlights most important genes

---

## Results

* Clear separation between cancer and normal samples observed
* Large number of significantly different genes identified
* High fold-change genes indicate potential biomarkers
* Correlation patterns suggest possible pathway-level interactions

---

## Output Files

### Data Files

* significant_genes.csv → filtered important genes
* all_genes_results.csv → complete gene analysis

### Text Output

* analysis_summary.txt → biological interpretation

### Visualization Files

* pca_plot.png
* clustering_plot.png
* Top_50_variable_genes.png
* volcano_plot.png
* Gene_Correlation_Heatmap.png
* Fold_Change_Distribution.png
* top_genes_plot.png

---

## Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* SciPy
* Matplotlib, Seaborn

---

## How to Run

pip install -r requirements.txt

Run the notebook:
notebooks/BioPath_Analysis.ipynb

---

## Key Insights

* Gene expression patterns clearly distinguish cancer from normal samples
* Differential analysis identifies genes driving disease progression
* High fold-change genes may serve as biomarkers
* Combined machine learning and statistical analysis improves interpretability

---

## Limitations

* Normal vs cancer grouping is assumed based on dataset structure
* No pathway enrichment analysis included
* Analysis is limited to transcript-level data

---

## Future Work

* Pathway enrichment analysis (KEGG / Reactome)
* Integration with MP-BioPath for pathway perturbation modeling
* Network-based pathway modeling
* Integration with mutation and PTM datasets
* Advanced deep learning approaches

---

## Author

Susanth Mohan Kamala – GSoC Applicant

---

## Acknowledgement

Dataset obtained from NCBI GEO (GSE15852)
