# Explainable-AI
Explainable AI framework for Parkinson's Disease biomarker discovery using multicohort transcriptomic integration, machine learning, SHAP interpretability, and pathway enrichment analysis of substantia nigra gene expression datasets.


# Explainable AI-Driven Multicohort Transcriptomic Profiling of the Substantia Nigra Reveals Biomarkers for Parkinson's Disease

## Project Overview

Parkinson's Disease (PD) is the second most common neurodegenerative disorder worldwide, characterized by progressive loss of dopaminergic neurons in the substantia nigra pars compacta (SNpc). Early diagnosis remains challenging due to the absence of reliable molecular biomarkers.

This project presents a comprehensive bioinformatics and machine learning framework that integrates multiple transcriptomic datasets from the substantia nigra region to identify biologically meaningful biomarkers associated with Parkinson's Disease.

By combining multicohort transcriptomic integration, machine learning, explainable artificial intelligence (XAI), SHAP-based interpretation, and pathway enrichment analysis, this study aims to discover robust biomarkers while maintaining biological interpretability.

---

## Objectives

The major objectives of this project are:

- Integrate multiple GEO transcriptomic datasets from substantia nigra tissue.
- Build a harmonized gene expression matrix for Parkinson's Disease research.
- Develop machine learning models for disease classification.
- Apply Explainable AI techniques to interpret model predictions.
- Identify biologically relevant biomarkers.
- Investigate molecular pathways involved in Parkinson's Disease progression.
- Improve reproducibility and reliability of transcriptomic biomarker discovery.

---

## Background

Traditional biomarker studies often suffer from:

- Small sample sizes
- Platform-specific biases
- Poor reproducibility
- Lack of biological interpretability

To overcome these limitations, this project integrates multiple independent transcriptomic cohorts and employs Explainable AI to reveal the biological significance behind machine learning predictions.

---

## Datasets Used

Publicly available datasets were obtained from the NCBI Gene Expression Omnibus (GEO).

| GEO Dataset | Platform |
|------------|----------|
| GSE7621 | GPL570 |
| GSE20141 | GPL570 |
| GSE43490 | GPL6480 |
| GSE20163 | GPL96 |
| GSE20292 | GPL96 |
| GSE20164 | GPL96 |
| GSE24378 | GPL570 |

### Cohort Summary

- Parkinson's Disease Samples: 67
- Healthy Controls: 63
- Total Samples: 130

### Tissue Source

- Substantia Nigra (SNpc)

---

## Methodology

### Step 1: Data Collection

- Retrieval of transcriptomic datasets from GEO
- Metadata extraction
- Quality assessment

### Step 2: Data Preprocessing

- Probe annotation
- Gene symbol conversion
- Missing value handling
- Cross-platform harmonization
- Common gene intersection

### Step 3: Normalization

Min-Max normalization was applied to reduce batch effects and improve dataset compatibility.

### Step 4: Exploratory Data Analysis

Quality control visualizations:

- Heatmaps
- Boxplots
- Histograms
- Density plots
- Volcano plots

### Step 5: Machine Learning Modeling

Four machine learning models were trained and evaluated:

1. Logistic Regression
2. Random Forest
3. Support Vector Machine (SVM)
4. XGBoost

### Step 6: Explainable AI Analysis

SHAP (SHapley Additive Explanations) was used to:

- Interpret model decisions
- Rank gene importance
- Identify disease-associated biomarkers

### Step 7: Functional Enrichment Analysis

KEGG pathway enrichment analysis was performed on SHAP-prioritized genes.

### Step 8: Literature Validation

Biological validation was conducted using PubMed literature evidence.

---

## Workflow

```text
GEO Dataset Retrieval
          │
          ▼
 Data Cleaning & Annotation
          │
          ▼
 Common Gene Identification
          │
          ▼
 Data Harmonization
          │
          ▼
 Min-Max Normalization
          │
          ▼
 Exploratory Data Analysis
          │
          ▼
 Machine Learning Models
          │
          ▼
 SHAP Explainability
          │
          ▼
 Biomarker Discovery
          │
          ▼
 KEGG Pathway Analysis
          │
          ▼
 Literature Validation
