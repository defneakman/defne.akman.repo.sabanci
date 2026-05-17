# DSA210 Project - The Impact of the Academic Calendar and Physical Activity on Personal Biochemistry

## Project Motivation
This project investigates whether physical activity levels and academic stress periods are associated with changes in personal blood biomarkers.

## Data Sources
- Personal blood test results collected from e-Nabız
- Daily step count data exported from Apple Health
- Sabancı University academic calendar data from 2022 to 2026

## Repository Structure
- `data/raw/`: raw source files
- `data/processed/`: cleaned datasets
- `src/`: preprocessing scripts
- `notebooks/`: main analysis notebook
- `outputs/`: generated figures

## Methods
- Data cleaning and preprocessing
- Academic period labeling
- Exploratory Data Analysis
- Hypothesis testing
- Correlation analysis

## How to Run
1. Install dependencies from `requirements.txt`
2. Run preprocessing scripts in `src/`
3. Open the notebook in `notebooks/`

## Limitations
- Small sample size
- Irregular blood test timing
- Personal observational dataset
- Finals-period blood measurements are limited
## Machine Learning Methods

For the 5 May milestone, machine learning methods were applied to the processed blood test and physical activity dataset. Since the available dataset contains only 9 blood test observations, the goal was exploratory pattern discovery rather than building a high-accuracy predictive model.

The ML analysis included:

- PCA to reduce the biomarker and step-count feature space into two principal components.
- K-Means clustering to identify unsupervised biochemical/activity profile groups.
- Logistic Regression and Decision Tree classifiers evaluated with Leave-One-Out Cross Validation.
- Random Forest feature importance analysis to identify the most informative variables.
- Time-lag analysis using 14-day and 28-day average step count features.

13 features were used: 12 blood biomarkers (LDL, HDL, Total Cholesterol, Triglycerides, Glucose, CRP, TSH, Ferritin, WBC, Hemoglobin, Creatinine, Uric Acid) plus 14-day average step count. Features were z-score standardised; missing values imputed with column medians. The revised final notebook is at: notebooks/DSA210_FinalML_defneakman_1.ipynb

## AI Usage Disclosure (Detailed)
This project utilizes AI assistance (Claude/Gemini) as permitted by the course guidelines. Below is the documentation of the AI interaction:
**Prompt Used:**
> "this is my project guideline. 'The Impact of the Academic Calendar and Physical Activity on Personal Biochemistry...' guide me through what you can do"
**My contributions:**
The core and idea of this project is entirely mine. I designed the research question from personal curiosity about my own health patterns over four years of university. I collected all data myself — retrieving blood test records from e-Nabız across 12 sessions spanning 2022–2025, exporting my Apple Health data, and manually cross-referencing the Sabancı University academic calendar. I defined the stress labelling system (0–3) based on my own lived academic experience, including failed courses, repeated semesters, and internship overlap — context that no external tool could know. I verified every biological interpretation against my personal health history and made all decisions about which findings were meaningful.
**AI assistance:**
Claude helped with the technical implementation: parsing the Apple Health XML, structuring the dataset, writing analysis and ML code, and formatting the report. All data values, stress labels, research framing, and interpretations are my own.

**The updated notebook for the 18 May ML milestone is available here: notebooks/DSA210_FinalML_defneakman_1.ipynb**
