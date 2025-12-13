# Mental Health in Tech: 

This project explores attitudes towards mental health in the tech workspace and how they relate to seeking professional treatment. Using the 2016 OSMI Mental Health Tech Survey (~1400 responses), I applied machine learning models to predict treatment-seeking behavior and analyze feature importance.

## Project Structure

The goal of my project was to explore attitudes towards mental health in the tech workspace and how these attitudes affect an individual’s likelihood to receive professional treatment. My dataset was from the Open Science Monitoring Initiative. Its goals are to fight stigma around mental health disorders by speaking openly about experiences and educate the tech community on the economic impact of mental disorders and how it affects worker productivity. I used their Mental Health Tech Survey from 2016 which includes about 1400 responses measuring mental health in the tech workspace. The primary difficulty of the dataset was missing values due to unanswered survey questions. 

## data/ 
# Raw dataset from OSMI Mental Health Tech Survey 2016

The dataset is from the Open Science Monitoring Initiative’s Mental Health Tech Survey (2016). It includes ~1400 responses measuring mental health in the tech workspace. The dataset contains missing values due to unanswered survey questions.  
**Source:** [OSMI Mental Health Tech Survey 2016](https://www.kaggle.com/datasets/osmi/mental-health-in-tech-2016)

### Environment

- **Python version:** 3.12.10  
- **Key packages and versions:**  
  - numpy 2.2.5  
  - pandas 2.2.3  
  - scikit-learn 1.6.1  
  - matplotlib 3.10.1  
  - seaborn 0.13.2  
  - xgboost 3.0.0  
  - shap 0.47.2  
  - polars 1.27.1  

*You can also run `src/check_environment.py` to verify your Python and package versions match.*

### Usage
To reproduce the analysis:

1. Clone the repository:  
To reproduce the analysis:

```bash
git clone <repo_url>
pip install -r requirements.txt
python src/main.py

Install the required Python packages listed in requirements.txt and run src/main.py to reproduce the analysis.

### figures/   # EDA plots and visualizations
### results/   # Model outputs
### figures/
# EDA plots and visualizations

## results/
# Model outputs: confusion matrices, permutation feature importance, SHAP plots, performance summaries

## report/
# Final project report (PDF)
# Key Findings

The Random Forest model performed best, improving baseline accuracy by ~26%.

Features most associated with seeking professional treatment were prior mental health diagnosis, history of mental illness, and whether treatment interfered with work.

Workplace-specific features (e.g., awareness of employer-provided mental health care or negative workplace experiences) had less impact, suggesting broader personal factors are more influential.

Future work could isolate workplace-specific questions to better understand their predictive contribution.
## src/
# Scripts for data preprocessing, modeling, evaluation, and figure generation

## .gitignore
# Files and directories ignored by git

## LICENSE
# Project license (GPL-3.0)

### License
This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.  
You are free to use, modify, and share this project, but any derivative work must also be released under the same license.  
For more details, see the [LICENSE](https://www.gnu.org/licenses/gpl-3.0.txt) file.

## README.md # Project overview and instructions
