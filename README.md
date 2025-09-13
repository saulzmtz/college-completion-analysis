# 🎓 Demographic Factors and College Completion

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)](https://scikit-learn.org/stable/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

## Project Overview  
This repository contains the research, analysis, and modeling from my **ADTA 5410 Research Project** (M.S. in Advanced Data Analytics, University of North Texas).  

The project investigates **college degree completions across 16,000+ U.S. institutions (2022–2023)**, using demographic and institutional data. It combines **exploratory data analysis (EDA)** with **machine learning models** to uncover the strongest demographic predictors of completion.  

---

## 📂 Repository Contents

├── ResearchPaper.pdf # Full research paper
├── PresentationSlides.pdf # Project presentation slides
├── AnalysisNotebook.ipynb # Jupyter Notebook with code
├── README.md # Project documentation


## Dataset  
- **Source:** [IPEDS – Integrated Postsecondary Education Data System](https://nces.ed.gov/ipeds/)  
- **Institutions:** 16,065  
- **Timeframe:** July 1, 2022 – June 30, 2023  
- **Coverage:** Degree completions by race/ethnicity, gender, and age  

---

## Research Question  
**What demographic factors are the strongest predictors of degree completion across U.S. higher education institutions?**  

## Methods  

**Data Preparation**  
- Cleaned and reduced dataset (removed imputation columns).  
- Encoded categorical variables (gender, race/ethnicity).  
- Normalized continuous variables (e.g., tuition, student–faculty ratio).  

**Models Applied**  
- **Logistic Regression** – linear relationships, interpretable coefficients.  
- **Decision Tree** – non-linear splits, interpretable structure.  
- **Random Forest** – ensemble model, robust & less prone to overfitting.  
- **Validation:** 5-fold cross-validation to test model generalizability.  

---

## Results  

| Model              | Accuracy | Key Predictors | Notes |
|--------------------|----------|----------------|-------|
| Logistic Regression | 97% | White completions, Female completions | Strong linear baseline |
| Decision Tree       | 99.6% | Female completions, Male completions, White completions | High accuracy but risk of overfitting |
| Random Forest       | 99.4% | Female completions, Age 25–39 (non-traditional), Male completions | Best balance of accuracy & generalizability |

---

## Key Insights  
- **Female completions** are the strongest predictor of institutional success.  
- **Non-traditional students (ages 25–39)** play a critical role in completions.  
- **White student completions** are highly predictive, though other groups also contribute.  
- **Random Forest** proved most robust, achieving consistent **~99% accuracy** across folds.  

---

## Tools & Technologies  
- **Python**: pandas, NumPy, scikit-learn, matplotlib, seaborn  
- **Jupyter Notebook**  
- **Excel/Spreadsheets** (initial EDA)  

---

## Author  
**Saúl Martínez**  
M.S. in Advanced Data Analytics, University of North Texas  


---

## 🔮 Future Work  
- Expand to **socioeconomic and institutional variables** (e.g., financial aid, program type).  
- Explore **advanced ML methods**    
- Develop **interactive dashboards** to visualize degree completion trends.  

