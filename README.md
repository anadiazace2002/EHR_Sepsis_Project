# EHR_Sepsis_Project
This repository contains an end-to-end analysis of severe sepsis patients using the MIMIC-III database. The project focuses on cohort selection, data extraction, cleaning, and exploratory and statistical analysis to compare clinical, laboratory, and treatment factors between survivors and non-survivors.

---

## Project Structure
ehr-sepsis-project/
│
├── data/ # Intermediate and processed datasets
│ ├── clinical.csv
│ ├── laboratory.csv
│ ├── treatment.csv
│ └── cleaned_data/ # Cleaned datasets (after preprocessing)
│ ├── clinical_clean.csv
│ ├── laboratory_clean.csv
│ └── treatment_clean.csv
│
├── notebooks/
│ ├── 01_cohort_selection/ # Cohort definition and extraction
│ │ └── cohort_extraction.ipynb
│ │
│ ├── 02_cleaning_preprocessing/# Missing data, outliers, transformations
│ │ └── data_cleaning.ipynb
│ │
│ └── 03_analysis_visualization/# Comparative analysis and models
│ └── final_analysis.ipynb
│
├── results/
│ ├── tables/ # Summary tables for the paper
│ └── figures/ # Final plots and visualizations
│
├── paper/
│ └── main.tex # LaTeX manuscript (or synced with Overleaf)
│ └── paper.pdf 
│
├── README.md
└── .gitignore


---

## Methodological Overview

1. **Cohort Selection**
   - Adult patients (>18 years)
   - Severe sepsis defined using ICD-9 codes
   - Clinically justified inclusion and exclusion criteria

2. **Data Preprocessing**
   - Identification and handling of missing values
   - Encoding of categorical variables
   - Outlier detection and transformation
   - Reproducible preprocessing pipeline

3. **Analysis**
   - Descriptive analysis of survivors vs. non-survivors
   - Visualization of clinical, laboratory, and treatment factors
   - Optional logistic regression models with clinically selected variables

4. **Reporting**
   - Results and figures integrated into a LaTeX manuscript
   - Limitations and clinical interpretation discussed

---

## Data Source

- MIMIC-III Clinical Database (v1.4)
- Access subject to credentialing and data use agreement

---

## Authors

- Víctor – Cohort selection and clinical analysis  
- Ana – Data preprocessing and cleaning  
- Person 3 – Statistical analysis and visualization

