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

## AI Usage Disclosure (Detailed)
This project utilizes AI assistance (Claude/Gemini) as permitted by the course guidelines. Below is the documentation of the AI interaction:

**Prompt Used:**
> "this is my project guideline. 'The Impact of the Academic Calendar and Physical Activity on Personal Biochemistry...' [Your full prompt here] ... guide me through what you can do"

**AI Contributions:**
- **Code Structuring:** Assisted in writing the Mann-Whitney U test loops and Pearson correlation logic.
- **Data Preprocessing:** Provided templates for handling date-time conversions and rolling averages for step data.
- **Documentation:** Helped in formatting the README.md and structuring the academic calendar windows.
- **EDA Support:** Suggested visualization techniques for comparing finals vs. holiday periods.

**Human Oversight:**
All AI-generated code was manually reviewed, debugged, and integrated into the final .ipynb by the student. All interpretations of p-values and findings were written by the student based on the analysis results.
