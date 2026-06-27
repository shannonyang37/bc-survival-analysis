## **Analysis of Clinical Determinants of Mortality in Breast Cancer**

### Project Overview
This project aims to investigate the clinical determinants of mortality in breast cancer patients. Utilizing Pandas, Seaborn, and Matplotlib, a custom statistical pipeline was engineered to conduct univariate exploratory data analysis across 13 clinical factors. By coupling visual distributions with rigorous mathematical validation (including Chi-Square, ANOVA, Welch's T-Test, and Multivariate Log-Rank tests), this analysis identifies the statistically significant prognostic drivers of patient survival.

---
### Project Workflow
The project is broken down into three Jupyter Notebooks:
1. **Data Cleaning and Preprocessing (`1_data_cleaning.ipynb`):** Cleaned and preprocessed the SEER Breast Cancer Dataset.
2. **Defining Analysis Tools (`2_analysis_tools.ipynb`):** Serves as a backend graphical and statistical engine, designed functions to automate the exploratory data analysis. 
3. **Exploratory Data Analysis (`3_exploratory_analysis.ipynb`):** Deployed the analysis tools in Notebook 2 to perform univariate exploratory data analysis to analyse the 13 clinical factors of mortality in breast cancer patients. 

---
### Key Results
The univariate exploratory data analysis revealed a crucial clinical distinction between the likelihood of mortality and the velocity of mortality among the 13 clinical factors evaluated.

- **Universal Prognostic Significance:** Every clinical factor analyzed—spanning demographic, anatomical, and biological variables—proved to be a highly statistically significant determinant of overall survival probability. Factors such as advanced T Stage, higher Tumor Grade, and negative hormone receptor status all drastically increased a patient's absolute risk of mortality.
- **Selective Acceleration of Terminal Decline:** While all 13 factors strongly influenced whether a patient would survive, only a specific subset of biological and systemic factors mathematically accelerated the timeline to death once the disease became terminal. Factors indicating systemic metastasis, specifically N Stage (lymphatic spread), A Stage (distant metastasis), and negative Estrogen or Progesterone receptor status, significantly shortened the median survival time of the deceased cohort.
---
### Limitations and Future Work
The primary limitation of this project is the absence of multivariate analysis. While exploring factors in isolation successfully reveals individual statistical associations with patient survival, it does not account for potential confounding variables or multi-collinearity. Furthermore, because the clinical factors were evaluated individually, it is impossible to rank their prognostic strength or determine which factor is the single most powerful driver of mortality. 

In the future, we could introduce multivariate analysis such as Cox Proportional Hazards model for the simultaneous evaluation of all 13 clinical factors. We could also utilize machine learning techniques to rank the features to explicitly isolate the most dominant clinical determinants of breast cancer mortality.

---
### Installation
Clone the repository:
```
git clone https://github.com/shannonyang37/bc-survival-analysis.git
cd bc-survival-analysis
```

Set up a virtual environment:
```
python -m venv venv
venv\Scripts\activate
```

Install dependencies:
```
pip install -r requirements.txt
```

Launch Jupyter Notebook:
```
jupyter notebook
```

Run the notebooks in sequential order to replicate the study:
* 1_data_cleaning.ipynb
* 2_analysis_tools.ipynb
* 3_exploratory_analysis.ipynb

---
### Author
Shannon Yang

Learning Project: Analysis of Clinical Determinants of Mortality in Breast Cancer
