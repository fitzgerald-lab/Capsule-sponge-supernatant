# Machine Learning Analysis for Cell-Free Capsule Sponge Biomarkers

This repository contains analysis code for the capsule sponge supernatant manuscript (Ustaoglu A, et al) being submitted to Gastroenterology journal

The analyses focus on evaluating the diagnostic performance of a panel of cell-free protein biomarkers measured from capsule sponge supernatant for the detection of Barrett’s oesophagus.

---

## Overview of Notebook Contents

The Jupyter notebook provided in this repository (`MLClassification_exploratory.ipynb`) was used during the study to:

- Train and compare multiple clinically appropriate classification models  
  (logistic regression, random forest, XGBoost, LightGBM)
- Perform cross-validated evaluation of biomarker panels
- Generate visualization outputs corresponding to **Figures 3, 4, and 5** of the manuscript, including:
  - Cross-validated ROC curves
  - Summary performance metrics across models
  - Feature contribution and interpretability analyses (SHAP)

This notebook reflects the exploratory and comparative phase of model development used to inform figure generation and model selection.

---

## Cohort Definitions and Analysis Scope

As described in the manuscript Methods:

- **Cohorts 5 and 6** were used for model development and cross-validation.
- **Cohort 7** was reserved as a locked external validation cohort.

The final reported diagnostic performance metrics in the manuscript were generated using these predefined cohort assignments and a locked analysis pipeline.

The notebook provided here includes exploratory code used during figure development and model comparison. A fully manuscript-aligned analysis script, reflecting the exact cohort separation and reporting logic used for final results, will be released as part of the revision process and/or upon manuscript acceptance.

---

## Reproducibility Notes

- Analyses were performed in Python using `scikit-learn`, `LightGBM`, `XGBoost`, and `SHAP`.
- Random seeds were fixed to ensure reproducibility.
- Standard preprocessing steps (imputation and scaling) were applied consistently across models during cross-validation.

This repository is intended to provide transparency into the modeling approach and figure generation process, rather than serve as a final locked clinical analysis package.

---

## Contact

For questions regarding the analysis or code, please contact the corresponding author.
