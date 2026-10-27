# Bacterial Fitness Data Visualization with Seaborn

## Overview

This project explores bacterial fitness data using Python's data visualization ecosystem, with a focus on identifying distributions, relationships, and differences across biological categories.

Completed as part of the **HackBio internship**, the exercise applies statistical visualization techniques to biological data, demonstrating how exploratory data analysis (EDA) can support the interpretation and communication of biological measurements.

The project contributes to my developing skill set in **Genomic Data Science**, particularly Python-based biological data analysis and visualization.

## Objectives

- Explore the distributions of bacterial fitness measurements.
- Investigate relationships between different fitness-related variables.
- Compare measurements across phenotypes, labels, and isolation origins.
- Visualize patterns and correlations among numerical fitness measurements.
- Practice selecting appropriate visualizations for different analytical questions.

## Dataset

The exercise uses the `bacteria_data` dataset provided by HackBio.

**Source:** [HackBio — bacteria.csv](https://raw.githubusercontent.com/HackBio-Internship/2025_project_collection/refs/heads/main/bacteria.csv)

The dataset contains bacterial fitness measurements and categorical variables used to explore differences and relationships across biological groups.

## Tools and Libraries

- **Python** — data analysis and programming.
- **Pandas** — data manipulation and preparation.
- **Seaborn** — statistical data visualization.
- **Matplotlib** — plot customization, labels, titles, and figure presentation.

## Analyses and Visualizations

### 1. Distribution Analysis
- Histogram of `carb_fit`.
- Kernel density estimate (KDE) plot of `cipro_fit`.
- Distribution plots grouped by phenotype.

### 2. Relationships Between Fitness Measurements
- Scatter plots comparing `carb_fit` and `pip_fit`.
- Line plots comparing `kan_fit` and `genta_fit`.
- Color-based grouping to explore patterns across labels, phenotypes, and isolation origins.

### 3. Categorical Comparisons
- Bar plots grouped by labels.
- Box plots grouped by phenotype.
- Violin plots grouped by isolation origin.
- Strip or swarm plots displaying individual observations.

### 4. Fitness Heatmap
A heatmap of numerical fitness measurements, with annotated cell values, to facilitate visual comparison across measurements.

### 5. Faceted Categorical Visualization
A faceted box plot using Seaborn's `catplot()` to explore expression measurements across genes and experimental conditions, where the required variables are available in the dataset.

## Skills Demonstrated

- Exploratory data analysis of biological datasets.
- Statistical visualization with Seaborn and Matplotlib.
- Mapping categorical variables to visual properties such as color and facets.
- Comparing numerical measurements across biological groups.
- Visual communication through plot titles, axis labels, legends, and annotations.
- Writing structured, readable Python analysis code.

## Reproducing the Analysis

1. Clone or download this repository.
2. Ensure Python and Jupyter Notebook are installed.
3. Install the required libraries:

   ```bash
   pip install pandas seaborn matplotlib jupyter
   ```

4. Download the dataset from the source linked above.
5. Open the notebook in Jupyter Notebook or VS Code.
6. Update the dataset path if necessary and run the notebook cells.

## Context

This exercise is part of my ongoing development in computational approaches to biological research. It builds practical foundations in data handling and visualization that are relevant to broader work in Genomic Data Science, bioinformatics, and computational biology.

---

*Part of my HackBio internship project portfolio.*