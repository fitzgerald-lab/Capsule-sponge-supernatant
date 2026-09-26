# Machine Learning Analysis for Cell-Free Capsule Sponge Biomarkers

This repository contains analysis code for the capsule sponge supernatant manuscript (Ustaoglu A, Pavada S, et al) being submitted to Gastroenterology journal

The analyses focus on evaluating the diagnostic performance of a panel of cell-free protein biomarkers measured from capsule sponge supernatant for the detection of Barrett’s oesophagus.

---

## Overview of Notebook Contents

The Jupyter notebook provided in this repository (`Manuscript_Figures.ipynb`) was used during the study to:

- Train a diagnostic log1p logistic regression model 
- Perform cross-validated two-protein biomarker panel across independent prospective cohorts
- Generate visualization outputs corresponding to **Figures 3 and 4** of the manuscript, including:
  - Cross-validated ROC curves
  - Summary protein concentrations across cohorts
  - Feature contribution and interpretability analyses (SHAP)
  - Model's confidence intervals and accuracy in predicting clinical outcome

This notebook reflects the exploratory and comparative phase of model development used to inform figure generation and model selection.

---

## Cohort Definitions and Analysis Scope

As described in the manuscript Methods:

- **Training cohort** was used for model development
- **Dysplasia cohort and prospective cohort** were reserved as a locked external validation and test cohort, respectively.

The final reported diagnostic performance metrics in the manuscript were generated using these predefined cohort assignments and a locked analysis pipeline.

---

## Reproducibility Notes

- Analyses were performed in Python using `scikit-learn`, `matplotlib`, and `SHAP`.
- Random seeds were fixed to ensure reproducibility.
- Standard preprocessing steps (imputation and scaling) were applied consistently across models during cross-validation.

This repository is intended to provide transparency into the modeling approach and figure generation process, rather than serve as a final locked clinical analysis package.

---

## Contact

For questions regarding the analysis or code, please contact the corresponding author.
