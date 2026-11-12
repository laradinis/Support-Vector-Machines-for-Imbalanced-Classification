# Support Vector Machines for Imbalanced Classification

This project focuses on the implementation and benchmarking of Support Vector Machines (SVMs) for binary classification, with particular emphasis on **class imbalance**.

The main objective is to investigate how class weighting and hyperparameter optimization can improve the ability of an SVM to identify minority-class samples.

## Project Overview

A custom SVM implementation was developed in Python and evaluated across multiple benchmark datasets. The project compares three approaches:

- **Standard SVM:** Baseline implementation without class weighting.
- **Weighted SVM:** Modified implementation using class weights to penalize errors on minority-class samples more heavily.
- **Weighted SVM with Hyperparameter Tuning:** Class-weighted implementation with dataset-specific optimization of the C and gamma parameters.

## Methodology

The project follows several stages:

1. **SVM Implementation:** Study of the theoretical foundations and implementation of the SVM algorithm, including hinge loss and optimization.
2. **Data Preprocessing:** Handling of numerical and categorical features, missing values and feature scaling.
3. **Baseline Evaluation:** Evaluation of the standard SVM across benchmark datasets, focusing on the effects of class imbalance.
4. **Class Weighting:** Modification of the optimization process to account for differences in class frequencies.
5. **Hyperparameter Tuning:** Search for suitable C and gamma values using cross-validation.
6. **Statistical Analysis:** Comparison of model performance using Friedman and Wilcoxon statistical tests.

## Evaluation Metrics

The models are evaluated using classification metrics, including:

- Accuracy
- Precision
- Recall
- Macro F1-score
- Minority-class F1-score

The analysis places particular emphasis on Macro F1 and minority-class performance, since accuracy alone can hide poor results on imbalanced datasets.

## Technologies & Tools

- Python
- NumPy
- Pandas
- Scikit-learn (preprocessing, pipelines and evaluation utilities)
- Matplotlib
- Seaborn
- Plotly
- SciPy
- Jupyter Notebook

## Repository Contents

- `Trabalho1.ipynb` – Main notebook containing the implementation, experiments, visualizations and statistical analysis.
- `AC1_trabalho.pdf` – Original practical assignment instructions.

## Project Status

**Completed**

The project resulted in a comparative study of standard and class-weighted SVM implementations, including hyperparameter tuning and statistical validation across benchmark datasets.
