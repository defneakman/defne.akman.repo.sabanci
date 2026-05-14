**Milestones:** 
April 14, 2026 — Data Collection, EDA & Hypothesis Testing  
May 5, 2026 — Machine Learning Methods
**Updated for:**
18 May, 22:00: Final report and code submission

## Machine Learning Methods

For the final submission, ML methods were applied using 13 features:
12 blood biomarkers (LDL, HDL, Total Cholesterol, Triglycerides, Glucose,
CRP, TSH, Ferritin, WBC, Hemoglobin, Creatinine, Uric Acid) + 14-day avg step count.
Features were z-score standardised; missing values imputed with column medians.

Methods applied:
- PCA (dimensionality reduction + feature loading analysis)
- K-Means clustering (k=3, evaluated with ARI and silhouette score)
- Logistic Regression + Decision Tree (binary classification, LOO-CV)
- Time-lag Spearman correlation (steps -> biomarkers at 7/14/21/28 day lags)

Main notebook: [notebooks/DSA210_FinalML_defneakman_1.ipynb](notebooks/DSA210_FinalML_defneakman_1.ipynb)
