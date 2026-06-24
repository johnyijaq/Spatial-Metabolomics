# Spatial Metabolomics Analysis Using Scanpy and Python

## Overview

This repository demonstrates an end-to-end spatial metabolomics analysis workflow using Python, Scanpy, Squidpy, and AnnData. The project analyzes MALDI mass spectrometry imaging (MALDI-MSI) data to identify spatially organized metabolic programs, characterize metabolically distinct tissue regions, and explore tissue heterogeneity through unsupervised and spatially aware analyses.

The workflow is designed as a reproducible and portfolio-ready notebook covering data preprocessing, quality control, dimensionality reduction, clustering, spatial statistics, differential analysis, metabolite visualization, and biological interpretation.

---

## Dataset

The analysis was performed using MALDI spatial metabolomics datasets:

* Sample 32 (`sample_data_32.h5ad`)
* Sample 59 (`sample_data_59.h5ad`)

Both datasets were merged into a single AnnData object for integrated analysis.

### Dataset Summary

| Metric              | Value             |
| ------------------- | ----------------- |
| Samples             | 2                 |
| Tissue Pixels       | 723               |
| Metabolite Features | 1326              |
| Platform            | MALDI-MSI         |
| Data Format         | AnnData (`.h5ad`) |

---

## Analysis Workflow

### Data Processing

* Data loading and AnnData inspection
* Dataset compatibility assessment
* Background pixel identification and removal
* Quality control (QC)
* Feature filtering
* TIC normalization
* Log transformation

### Exploratory Analysis

* Principal Component Analysis (PCA)
* Neighborhood graph construction
* UMAP visualization
* Leiden clustering

### Spatial Analysis

* Spatial cluster visualization
* Spatially variable metabolite analysis (Moran's I)
* ROI-level differential analysis
* Sample-level differential analysis

### Biological Interpretation

* Cluster marker metabolite identification
* Metabolite correlation network analysis
* Spatial metabolite visualization
* Metabolite annotation assessment
* Biological interpretation of spatial metabolic patterns

---

## Key Results

### Spatial Organization of Metabolism

The analysis identified multiple metabolically distinct clusters exhibiting spatially coherent tissue distributions.

### Spatially Variable Metabolites

Moran's I analysis revealed metabolites with strong spatial autocorrelation, indicating localized metabolic programs within the tissue.

### Differential Metabolite Abundance

Differential analyses identified metabolites associated with:

* Specific Leiden clusters
* Tissue ROIs
* Sample-specific metabolic differences

### Network-Level Relationships

Correlation network analysis highlighted coordinated metabolite abundance patterns and potential metabolic modules.

---

## Technologies Used

### Programming Languages

* Python

### Core Libraries

* Scanpy
* Squidpy
* AnnData
* NumPy
* Pandas
* SciPy
* Matplotlib
* Seaborn
* NetworkX

### Data Structure

* AnnData (`.h5ad`)

---


## Reproducibility

Install required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Lab:

```bash
jupyter lab
```

Open:

```text
Spatial_Metabolomics_End_to_End.ipynb
```

and execute the notebook sequentially.

---


## Author

Johny Ijaq

Bioinformatics Scientist | Spatial Omics | Multi-Omics Data Analysis | Machine Learning for Healthcare
