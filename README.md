[English](README.md) | [Français](README.fr.md)

---

# Survival Data Analysis - Haberman's Survival Dataset

**Project instructions available in [PROJET_TND_7d393c181caebd340aefb61df17429e8.pdf](PROJET_TND_7d393c181caebd340aefb61df17429e8.pdf) (written in French).**

## Project Description

This project performs a comprehensive statistical analysis of Haberman's Survival dataset, which contains information about the survival of patients who underwent surgery for breast cancer between 1958 and 1970 at the University of Chicago's Billings Hospital.

## Objectives

The main objective is to analyze the factors influencing patient survival at 5 years post-operation, using data analysis and classification techniques.

## Dataset Content

The dataset includes **306 observations** with the following variables:

- **Patient Age**: Age at the time of operation
- **Year of Operation**: Year - 1900
- **Number of Positive Axillary Nodes Detected**: Indicator of cancer spread
- **Survival Status**: 
  - 1 = survived 5 years or longer
  - 2 = died within 5 years

## Analyses Performed

### 1. Data Preprocessing
- Loading and structuring the dataset
- Checking for missing values
- Variable type verification
- Outlier detection

### 2. Univariate Analysis
- Patient age distribution
- Distribution of detected lymph nodes
- Survival status distribution

### 3. Bivariate Analysis
- Relationship between age and survival
- Impact of lymph node count on survival rate
- Visualizations using ggplot2

### 4. Hierarchical Classification
- Variable standardization
- Euclidean distance matrix calculation
- Clustering with Ward's method
- Dendrogram visualization

## Technologies Used

- **Language**: R
- **Libraries**:
  - `ggplot2`: Advanced visualizations
  - `FactoMineR`: Multivariate analysis
  - `cluster`: Clustering methods
  - `MASS`: Statistical functions

## Project Structure

```
Projet-TND/
├── Code/
│   └── Code.R           # Main analysis script
├── Data/
│   └── Binome3/
│       ├── haberman.data      # Raw data
│       └── haberman.names     # Dataset description
└── README.md
```

## Usage

1. Ensure R is installed on your machine
2. Install required packages:
   ```r
   install.packages(c("ggplot2", "FactoMineR", "cluster", "MASS"))
   ```
3. Run the main script:
   ```r
   source("Code/Code.R")
   ```

## Expected Results

The analysis allows to:
- Identify at-risk patient groups
- Understand the influence of lymph node count on survival
- Visualize patterns in the data
- Propose a patient classification

**For detailed results and visualizations, please refer to the [full report](Rapport.pdf) (written in French).**

## Author

[@thmsgo18](https://github.com/thmsgo18)
[@Yvngval](https://github.com/Yvngval)

## Data Source

Haberman, S. J. (1976). Generalized Residuals for Log-Linear Models.  
Dataset available via the UCI Machine Learning Repository.
