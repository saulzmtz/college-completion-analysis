# Analyze Demographic Factors and Predict College Completion

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)](https://scikit-learn.org/stable/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Data Source](https://img.shields.io/badge/Data%20Source-IPEDS-orange.svg)](https://nces.ed.gov/ipeds/)

## Project Overview  
This project analyzes demographic factors influencing college degree completion rates across 16,065 U.S. higher education institutions using data from the National Center for Education Statistics (NCES) for the 2022-2023 academic year. Through advanced machine learning techniques, I identify the strongest predictors of institutional success in degree completions.

---

## Dataset  
- **Source:** [IPEDS – Integrated Postsecondary Education Data System](https://nces.ed.gov/ipeds/)  
- **Institutions:** 16,065  
- **Timeframe:** July 1, 2022 – June 30, 2023
- **Scope: 16,065 U.S. higher education institutions
- **Variables: Demographics (race/ethnicity, gender, age), degree completion counts
- **Coverage:** Degree completions by race/ethnicity, gender, and age  

---

## Research Question  
**What demographic factors are the strongest predictors of degree completion across U.S. higher education institutions?**  

**Data Preparation and Processing**  
- Comprehensive EDA with 16,065 institutions
- Handled missing values and data imputation 
- Encoded categorical variables (gender, race/ethnicity).  
- Normalized continuous variables (e.g., tuition, student–faculty ratio).  

**Machine Learning Models Applied**  
- **Logistic Regression** – linear relationships, interpretable coefficients 
- **Decision Tree** – non-linear splits, interpretable structure with hyperparameter tuning
- **Random Forest** – ensemble model, robust & less prone to overfitting
- **Validation:** 5-fold cross-validation to test model generalizability  

---

## Tools & Technologies  
- **Python**: pandas, NumPy, scikit-learn, matplotlib, seaborn  
- **Jupyter Notebook**  
- **Excel/Spreadsheets** (initial EDA)  

---

# Methodology

### 1. Exploratory Data Analysis
- Distribution analysis of completion rates
- Demographic breakdowns and correlations
- Missing data assessment and handling

### 2. Feature Engineering
- Binary classification (High/Low completions)
- One-hot encoding for categorical variables
- Normalization of continuous variables

### 3. Model Development
- Train/test split with stratification
- Hyperparameter tuning using GridSearchCV
- Cross-validation for model reliability

### 4. Model Evaluation
- Accuracy, Precision, Recall, F1-score
- Feature importance analysis
- Cross-validation consistency

## Results  

| Model              | Accuracy | Key Predictors | Notes |
|--------------------|----------|----------------|-------|
| Logistic Regression | 97% | White completions, Female completions | Strong linear baseline |
| Decision Tree       | 99.6% | Female completions, Male completions, White completions | High accuracy but risk of overfitting |
| Random Forest       | 99.4% | Female completions, Age 25–39 (non-traditional), Male completions | Best balance of accuracy & generalizability |

---

## Key Insights  

### Demographic Factors 
- **Gender**: Female completions (59.7%) vs Male (40.3%)
- **Female completions** are the strongest predictor of institutional success.
  
- **Age Distribution**: Traditional (51.3%), Adults 25-39 (36.5%), 40+ (11.3%)
- **Non-traditional students (ages 25–39)** play a critical role in completions.

- **Race/Ethnicity**: White (48.9%), Hispanic (18.5%), Black (11.2%), Asian (6.8%)
- **White student completions** are highly predictive, though other groups also contribute.  

### Predictive Factors
1. **CSTOTLW** (Female Completions) - Strongest predictor
2. **CS25_39** (Non-traditional Students) - Critical demographic
3. **CSWHITT** (White Student Completions) - Significant influence
4. **CSTOTLM** (Male Completions) - Important baseline

---
## Practical Applications

### For Educational Institutions
- **Resource Allocation**: Focus support on non-traditional students
- **Program Development**: Tailored interventions for diverse demographics
- **Success Metrics**: Evidence-based completion rate improvement strategies

### For Policymakers
- **Educational Equity**: Address demographic disparities
- **Funding Decisions**: Data-driven institutional support
- **Strategic Planning**: Demographic-aware policy development

## Academic Context

This research builds upon existing literature while providing new insights:

- **Flores & Park (2013)**: Race predicts enrollment but not completion
- **Heil et al. (2014)**: Tuition more predictive than selectivity
- **Eller & DiPrete (2018)**: Resource disparities drive completion gaps
- **Current Study**: Comprehensive demographic analysis with modern ML techniques

## Future Research Directions

- Incorporate socioeconomic variables
- Longitudinal analysis of changing demographics
- Institution-specific characteristics
- Community college and alternative pathways
- Economic impact analysis

---

## Author  
**Saúl Martínez**  
- M.S. in Advanced Data Analytics, University of North Texas  
- Course: ADTA 5410 - Applications and Deployment of Advanced Analytics

---

## 📚 References

1. Flores, S. M., & Park, T. J. (2013). Race, Ethnicity, and College Success. *Educational Researcher*, 42(3), 115–128.
2. Heil, S., Reisel, L., & Attewell, P. (2014). College Selectivity and Degree Completion. *American Educational Research Journal*, 51(5), 913–935.
3. Eller, C. C., & DiPrete, T. A. (2018). The Paradox of Persistence. *American Sociological Review*, 83(6), 1171–1214.
4. National Center for Education Statistics. (2023). Integrated Postsecondary Education Data System.

---
