# Exploring Genomics of Drug Sensitivity in Cancer (GDSC)

## Overview

This project explores the relationship between cancer genomic features and drug sensitivity using the Genomics of Drug Sensitivity in Cancer (GDSC) dataset.

Completed as part of the **HackBio internship**, the project applies Python-based data analysis to cancer pharmacogenomics, with a focus on understanding drug-response patterns across cancer cell lines and investigating how genomic, transcriptomic, and epigenomic features may relate to treatment response.

The project contributes to my developing skills in **Genomic Data Science, bioinformatics, and computational biology**, particularly in biological data handling, exploratory data analysis, and visualization.

## Project Objectives

- Explore and characterize the GDSC dataset.
- Identify key variables and assess data quality, including missing values and inconsistencies.
- Investigate patterns in drug sensitivity across cancer cell lines and cancer types.
- Compare drug-response measurements to explore differences in sensitivity and variability.
- Examine potential relationships between drug response and genomic features, including copy number alterations, gene expression, and methylation.
- Communicate exploratory findings through clear and informative visualizations.

## Dataset

The project uses the GDSC dataset provided through HackBio.

**Source:** [HackBio Public Datasets — GDSC.xlsx](https://github.com/HackBio-Internship/public_datasets/raw/refs/heads/main/GDSC.xlsx)

The dataset contains drug-response measurements alongside cancer cell line information, cancer classifications, and molecular features relevant to treatment sensitivity.

### Key Variables

| Variable | Description |
|---|---|
| `COSMIC_ID` | Unique identifier for a cell line in the Catalogue of Somatic Mutations in Cancer (COSMIC). |
| `CELL_LINE_NAME` | Name of the cancer cell line. |
| `TCGA_DESC` | Cancer-type classification using TCGA codes. |
| `DRUG_ID` / `DRUG_NAME` | Drug identifiers and names. |
| `LN_IC50` | Natural logarithm of the half-maximal inhibitory concentration (IC50). |
| `AUC` | Area under the dose-response curve. |
| `Z_SCORE` | Standardized drug-response measurement. |
| `CNA` | Copy number alteration information. |
| `Gene Expression` | Gene expression feature information. |
| `Methylation` | DNA methylation feature information. |
| `TARGET` | Genetic target associated with a drug. |
| `TARGET_PATHWAY` | Pathway associated with the drug target. |

Additional metadata describe tissue classifications, microsatellite instability, screening conditions, and cell growth properties.

## Tools and Technologies

- **Python** — programming and analysis.
- **Pandas** — data loading, manipulation, and cleaning.
- **NumPy** — numerical operations.
- **Matplotlib** — visualization and figure customization.
- **Seaborn** — statistical visualization.
- **Jupyter Notebook** — interactive analysis and documentation.
- **OpenPyXL** — reading Excel datasets with Pandas.

## Analytical Focus

### 1. Dataset Exploration and Quality Assessment

- Inspect the dataset's structure, dimensions, and data types.
- Examine variable definitions and identify relevant analytical features.
- Investigate missing values and potential inconsistencies.
- Prepare data for downstream exploratory analysis where necessary.

### 2. Drug Sensitivity Analysis

Explore drug-response measurements, including `LN_IC50`, `AUC`, and `Z_SCORE`, to investigate differences in sensitivity and response variability across drugs and cell lines.

Drug-response metrics require careful interpretation. For example, higher IC50 values generally indicate that more drug is required to inhibit growth, whereas lower IC50 values indicate greater potency under the assay conditions. AUC interpretation depends on the dose-response curve and the dataset's measurement conventions.

### 3. Cancer Cell Line Comparisons

Investigate how drug-response patterns vary across cancer types and cell lines, using the available cancer classifications and cell line metadata.

### 4. Molecular Features and Drug Response

Explore potential associations between drug sensitivity and molecular features, including copy number alterations, gene expression, and methylation, where the available data support the analysis.

These comparisons are exploratory and do not, by themselves, establish causation.

### 5. Data Visualization

Use statistical graphics to communicate patterns in the dataset, including distribution plots, box plots, scatter plots, and correlation analyses where appropriate.

## Skills Demonstrated

- Loading and inspecting biological datasets in Python.
- Data cleaning and preparation with Pandas.
- Exploratory analysis of cancer pharmacogenomics data.
- Interpreting drug-response metrics.
- Comparing measurements across cancer types, drugs, and cell lines.
- Visualizing biological data using Seaborn and Matplotlib.
- Formulating biological questions from structured datasets.
- Communicating analytical workflows and observations.

## Reproducing the Analysis

### Requirements

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn openpyxl jupyter
```

### Getting Started

1. Clone or download this repository.
2. Download the GDSC dataset from the source linked above.
3. Open the relevant Jupyter notebook in VS Code or Jupyter Notebook.
4. Ensure the dataset path in the notebook points to the downloaded Excel file.
5. Run the notebook cells in sequence.

The dataset can also be loaded directly from its source using Pandas:

Primary notebook: GDSC Code Task 2.ipynb

The notebook above contains the preferred solution to the GDSC coding task, including exploratory analysis and visualization of drug-sensitivity-related variables.

## Project Context

This project is part of my ongoing development in **Genomic Data Science** through the HackBio internship. It provides practical experience working with biological data and investigating questions at the intersection of cancer biology, pharmacogenomics, and computational analysis.

My broader interest is in applying computational methods and AI to biological research, including understanding disease mechanisms and exploring data-driven approaches to biomedical discovery.

---

*Part of my HackBio internship project.*