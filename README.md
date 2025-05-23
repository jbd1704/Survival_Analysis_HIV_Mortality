# 🧬 Survival Analysis of HIV Mortality in AZT-Intolerant Patients

This project presents a survival and longitudinal data analysis of HIV-infected patients who were either intolerant to or had failed AZT (zidovudine) therapy. These patients were subsequently treated with either **didanosine (ddI)** or **zalcitabine (ddC)**. The study aims to evaluate the impact of treatment type, CD4 cell counts, and clinical variables on survival outcomes using statistical and machine learning approaches in **R**.

## 🎯 Objectives

- Compare the effectiveness of ddI and ddC treatments.
- Investigate the relationship between CD4 counts and mortality risk.
- Identify key factors influencing patient survival using:
  - **Cox Proportional Hazards Models** (linear and generalized)
  - **Random Forests for survival analysis**

## 📊 Dataset Overview

- 467 patients, 1405 observations
- Variables include:
  - **Survival outcomes**: time-to-event, censoring, death status
  - **Biomarkers**: CD4 counts at multiple time points
  - **Demographics**: sex, prior infection (AIDS status)
  - **Treatment info**: ddI/ddC, AZT status (failure/intolerance)

## 🧪 Methodology

- **Feature engineering** to restructure longitudinal data into a start/stop format.
- **Exploratory Data Analysis** with visualizations (Kaplan-Meier curves, correlation matrices).
- Survival modeling:
  - **Linear Cox Model** for interpretability
  - **Generalized Cox Model** with splines for non-linear effects (e.g., CD4)
  - **Random Forest** for robust, non-parametric prediction

## 📈 Key Results

- CD4 count is inversely associated with mortality risk.
- **ddC may be preferable to ddI** for patients with low CD4 (< 20).
- Patients with **no prior infections** or **AZT intolerance** show better survival outcomes.
- Random Forest showed the **best predictive performance** (lowest Brier Score), while Cox models offered better interpretability.

## 🛠 Tools & Packages

- R packages: `survival`, `survminer`, `dplyr`, `ggplot2`, `randomForestSRC`
- Statistical techniques: Kaplan-Meier, log-rank test, Cox regression, Brier score analysis

## 📚 Conclusion

This study highlights how **statistical modeling and machine learning** can complement each other in medical survival analysis. It provides actionable insights into treatment strategies for HIV patients, particularly those with **AZT intolerance or failure**.

---

*Project by Jaad Belhouari – M2 Data Science: Santé, Finance et Assurance – December 2024*

