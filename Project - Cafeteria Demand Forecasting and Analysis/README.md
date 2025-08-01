# Cafeteria Demand Forecasting and Analysis  
**Business Analytics Final Project**  
Authors: Damla Uçar, Ahmet Sayan  
---

## Project Overview  
This project analyzes daily meal distribution data from Bilkent University’s main cafeteria over two years (December 2022 – December 2024). The main goals are to understand the factors affecting meal demand, including menus, academic periods, holidays, and special events, and to build predictive models for daily meal attendance to improve planning and reduce food waste.

---
## Dataset  
**Note:** The dataset has been removed from this repository to prevent any confidentiality issues related to institutional data.

---

## Notebooks  
- **Initial Analysis of Data.ipynb** contains the initial data analysis and trends, with most visualizations and exploratory analysis conducted here.  
- **Models.ipynb** includes the development of predictive models and their corresponding performance metrics.

---

## Full Report  
For more detailed information, analysis, and results, please refer to the [full project report](./Project - Cafeteria Demand Forecasting and Analysis/Cafeteria Project Report.pdf).

---

## Key Highlights  
- Data preprocessing included segmentation by academic semesters, holiday annotations, outlier removal (e.g., earthquake period), and consolidation of similar food items.  
- Explored multiple predictive models: Linear Regression, Lasso Regression, Random Forest, and LightGBM.  
- LightGBM was selected as the best-performing model based on R-squared, MSE, and MAE metrics.  
- Used SHAP values to interpret feature importance, identifying key demand drivers such as holidays, exam periods, Ramadan, day of the week, and menu components.  
- Model evaluation showed significant reduction in both food waste and shortages compared to a fixed meal preparation plan.

---

## Contents  
- Introduction and Data Description  
- Problem Statement and Initial Analysis  
- Implementation of Analytical Methods  
- Interpretation of Results  
- Appendices with figures and supplementary analyses  

---

## How to Use This Repository  
- Explore the Jupyter notebooks/scripts to see data cleaning, exploratory analysis, model training, and evaluation.  
- Review figures and tables illustrating demand patterns and model insights.  
- Refer to the appendix for detailed visualizations and SHAP interpretation.

---
