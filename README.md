# Inferential Statistical Analysis of Stroke Risk Factors

## Overview
This repository contains the implementation for the **21AIC401T Inferential Statistics and Predictive Analytics Case Study** focused on **stroke risk factors** using the Kaggle Healthcare Stroke Dataset.  

The analysis includes three statistical tests:
- **One-sample t-test** → average glucose level vs. 100 mg/dL  
- **Two-sample t-test** → BMI between stroke and non-stroke groups  
- **One-way ANOVA with Tukey HSD post-hoc** → age across smoking status  

The project is implemented in **Python (Google Colab)**, with outputs compatible for Excel and SPSS, meeting the requirements for the **September 23, 2025 viva**.

**Author:** Prejan Raja S  
**Course:** 21AIC401T Inferential Statistics and Predictive Analytics  
**Date:** September 22, 2025  

---

## Dataset
- **Source:** [Kaggle Healthcare Stroke Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset) (5,110 records)  
- **Variables:** Age, average glucose level, BMI, hypertension, smoking status, stroke (binary)  
- **Cleaning:**  
  - Missing BMI imputed with **median = 28.7**  
  - Excluded `'Unknown'` smoking status for ANOVA  
- **Access:** Loaded directly via GitHub raw URL:  
[https://raw.githubusercontent.com/rupakroy/healthcare-dataset-stroke-data/master/healthcare-dataset-stroke-data.csv](https://raw.githubusercontent.com/rupakroy/healthcare-dataset-stroke-data/master/healthcare-dataset-stroke-data.csv)

---

## Repository Structure
PrejanRajaS_stroke_analysis/
├── PrejanRajaS_analysis.ipynb   # Google Colab notebook with full implementation
├── PrejanRajaS_CaseStudy.xlsx   # Cleaned dataset + README sheet
├── PrejanRajaS_results.txt      # Statistical results for report/SPSS
├── stroke_analysis_plots.png    # Visualizations (BMI and age boxplots)
└── README.md                    # Project documentation



---

## Setup Instructions
1. Open [Google Colab](https://colab.research.google.com) and create a new notebook named **PrejanRajaS_analysis.ipynb**.  
2. Copy the Python code from this repo into the notebook.  
3. Run the cells in sequence — no manual dataset upload needed (auto-loads via GitHub URL).  
4. Dependencies (`pandas`, `numpy`, `scipy`, `statsmodels`, `matplotlib`, `seaborn`) are pre-installed in Colab.  
5. The notebook auto-generates:  
   - **PrejanRajaS_CaseStudy.xlsx** → cleaned data + variable descriptions  
   - **PrejanRajaS_results.txt** → test results (t-stats, p-values, CI)  
   - **stroke_analysis_plots.png** → boxplots for BMI and age  

---

## Implementation Details
- **Language:** Python 3 (Google Colab)  
- **Tests Performed:**  
  - One-sample t-test → mean glucose vs. 100 mg/dL (normal threshold)  
  - Two-sample t-test → BMI between stroke and non-stroke (Welch’s test)  
  - One-way ANOVA + Tukey HSD → age across smoking groups  

- **Visualizations:**  
  - BMI boxplot by stroke  
  - Age boxplot by smoking status  

- **Outputs:**  
  - Excel file with cleaned dataset  
  - Text file with inferential results  
  - PNG plots for report inclusion  

---

## Usage
### Running the Notebook
1. Open **PrejanRajaS_analysis.ipynb** in Colab.  
2. Execute cells in order.  
3. No dataset upload needed — loads directly from GitHub.  


