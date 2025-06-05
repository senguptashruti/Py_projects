# Py_projects
# Project 1: Beauty and Wage Analysis in Python
## Project Details
This project investigates the relationship between perceived attractiveness and wages using a publicly available “beauty” dataset. The analysis is implemented in Python, with a Jupyter Notebook (“Biz_eco_ass.ipynb”) that demonstrates data preparation, descriptive statistics, regression modeling (with and without gender interactions), and hypothesis testing. The primary objective is to determine whether individuals rated above or below average in attractiveness earn different wages, while controlling for gender, education, and experience.
## Files
- **['data/beauty.xlsx'](https://github.com/senguptashruti/Py_projects/blob/main/beauty.xlsx)**  
  Raw dataset (Excel format) containing variables:  
  - `wage` (numeric)  
  - `female` (binary indicator for gender)  
  - `belavg` (binary indicator for below-average attractiveness)  
  - `abvavg` (binary indicator for above-average attractiveness)  
  - `educ` (years of education)  
  - `exper` (years of work experience)  
  - `expersq` (experience squared)

- **['notebooks/Biz_eco_ass.ipynb'](https://github.com/senguptashruti/Py_projects/blob/main/Biz_eco_ass.ipynb)**  
  Jupyter Notebook with the full analysis workflow. Steps include:  
  1. Loading and cleaning the dataset  
  2. Computing descriptive statistics  
  3. Estimating a pooled regression model for log(wage)  
  4. Extending the model with gender interaction terms  
  5. Conducting joint significance tests on interaction coefficients
## Results
### Descriptive Statistics

| Group       | % Above Average Looks | % Below Average Looks |
|-------------|-----------------------|------------------------|
| Male        | 29.0%                 | 11.7%                  |
| Female      | 33.0%                 | 13.5%                  |
| Full Sample | 31.0%                 | 12.6%                  |

## Summary
- Individuals rated below average (`belavg = 1`) earn approximately 15.4% less than those at average attractiveness (p < 0.01).  
- There is no statistically significant positive premium for above-average attractiveness (`abvavg = 1`).  
- A substantial gender wage gap is observed: women (`female = 1`) earn about 45% less than men, controlling for other factors (p < 0.01).  
- Interaction terms between gender and human capital variables (education and experience) are jointly significant (p ≈ 0.0022), indicating that the returns to education and experience accumulate differently for men and women.  
- Attractiveness effects on wages do not significantly differ by gender in this sample.

This Python-based analysis provides a reproducible framework for examining sociological and economic questions about beauty, gender, and earnings. Feel free to explore further by modifying model specifications or applying similar workflows to other datasets.  
