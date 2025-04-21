# Psychometric-Scale-Construction-with-EFA-CFA-and-Item-Analysis
This repository contains a full R-based workflow for developing and validating a psychological scale. It walks through the process from raw item responses to a theoretically sound and statistically valid factor structure.
---
## 🎯 Objectives
- To screen and analyze individual items
- To explore the underlying factor structure using Exploratory Factor Analysis (EFA)
- To confirm the structure with Confirmatory Factor Analysis (CFA)
- To ensure the scale’s psychometric soundness via reliability and model fit indices

## 🧠 Contents
The procedure follows a classical test theory approach:

### Part 1: Item Analysis & EFA
1. **Data Preparation**  
   Import and clean raw data; focus on items X1 to X28.
2. **Normality Check**  
   Evaluate skewness and kurtosis to confirm item-level normality.
3. **Score Construction**  
   Compute total and average scores across items.
4. **Group Splitting**  
   Split participants into high/low score groups.
5. **Independent Sample t-tests**  
   Evaluate item discrimination between groups.
6. **Missing Values & Descriptive Statistics**  
   Report item-level means and check scale range.
7. **Suitability for Factor Analysis**  
   Use KMO and Bartlett’s test to check assumptions.
8. **Exploratory Factor Analysis (EFA)**  
   Run parallel analysis, determine factor count, remove problematic items.
9. **Internal Consistency**  
   Calculate Cronbach’s alpha for each factor.

### Part 2: Confirmatory Factor Analysis (CFA)
1. **Model Comparison**  
   Iteratively test models (Model 1–Model 6) using fit indices: CFI, RMSEA, SRMR, Chi-square.
2. **Final Model Selection**  
   Present the best-fitting CFA model.
3. **Path Diagram Visualization**  
   Plot the final CFA model structure.

## 🧪 Key Methods
- `shapiro.test`, `describe`, `sapply` for item screening  
- `t.test`, `var.test` for discrimination  
- `psych::fa`, `lavaan::cfa` for EFA and CFA  
- `semPlot` for visualizing CFA model  

## 📦 Dependencies
- `psych`
- `lavaan`
- `semPlot`

## 📌 Notes
This project follows best practices in psychometric scale construction and can serve as a template for thesis work or applied research in education, psychology, or social sciences.

## 🧑‍🎓 Author
Created by Alice Cheng — Master's student in Educational Psychology, passionate about psychometrics and data science.
