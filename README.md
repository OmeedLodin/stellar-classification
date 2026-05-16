# Stellar Classification Machine Learning Project

## Overview

This project focuses on the development and evaluation of supervised machine learning models for the classification of stellar objects using observational astronomical data from the Sloan Digital Sky Survey (SDSS).

Using photometric and survey-derived measurements, the models aim to classify celestial objects into one of the following categories:

- STAR
- GALAXY
- QSO (Quasar)

The project emphasizes both model performance and scientific interpretability through comparative analysis, feature evaluation, and error investigation.

---

# Objectives

The primary objectives of this project are to:

- Develop multiple machine learning classification models using SDSS observational data
- Compare model performance across several evaluation metrics
- Investigate feature importance and classification behaviour
- Analyze incorrectly classified objects to better understand model limitations
- Evaluate how different feature subsets affect model performance
- Compare results against existing machine learning studies in astronomical literature

---

# Dataset

The project currently uses the SDSS DR18 dataset.

SDSS DR18 was selected because it provides large-scale modern astronomical survey data while remaining highly compatible with prior SDSS-IV stellar classification research and benchmarking methodologies. This enables meaningful comparison against existing peer-reviewed machine learning studies using similar photometric features and classification tasks.

Although DR18 is released under SDSS-V, the underlying photometric classification framework remains closely aligned with earlier SDSS-IV data products commonly used in machine learning literature.

A dedicated SDSS-V-native dataset was not selected due to its stronger emphasis on:

- Time-domain astronomy
- Milky Way spectroscopy
- Black hole mapping

Additionally, many SDSS-V-focused datasets currently contain:

- Less established machine learning benchmarking literature
- Fewer directly comparable classification studies
- More complex observational pipelines and data structures

As a result, SDSS DR18 provides the best balance between:

- Modern survey quality
- Accessibility
- Dataset scale
- Research comparability
- Existing benchmarking support

---

# Input and Output

## Input Features

Astronomical observational features of stellar objects, including:

- Photometric magnitudes
- Flux measurements
- Petrosian radius measurements
- Survey-derived observational parameters

Examples include SDSS photometric bands such as:

- u
- g
- r
- i
- z

along with additional derived measurements.

## Output Classes

The models predict one of the following stellar object classifications:

- STAR
- GALAXY
- QSO (Quasar)

---

# Machine Learning Models

The following supervised learning models are being implemented and evaluated:

- Logistic Regression
- K-Nearest Neighbours (KNN)
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

Additional models may be explored later as the project expands.

---

# Evaluation Metrics

Model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix analysis

The highest-performing model will be selected for deeper analysis and comparison.

---

# Planned Analysis

Beyond standard model evaluation, the project also includes additional analytical phases focused on interpretability and classification behaviour.

## Misclassification Analysis

Incorrectly classified objects will be analyzed to investigate:

- Which classes are most frequently confused
- Which observational variables contribute to incorrect predictions
- Potential overlap between stellar object feature distributions
- Model limitations and edge cases

## Feature Set Analysis

Models will also be trained using different feature subsets in order to evaluate:

- Which variables contribute most strongly to classification performance
- How performance changes when specific features are removed
- Redundant or low-impact observational measurements
- Trade-offs between model complexity and predictive accuracy

This phase aims to improve both interpretability and overall understanding of the astronomical data.

---

# Comparison Against Existing Research

The best-performing model will be compared against results reported in peer-reviewed literature and related SDSS stellar classification studies.

This comparison will evaluate:

- Classification accuracy
- Feature engineering approaches
- Preprocessing methodologies
- Model selection strategies
- Overall effectiveness relative to comparable studies

The goal is to assess how the project performs relative to existing astronomical machine learning benchmarks.

---

# Current Project Status

This project is currently a work in progress.

Ongoing work includes:

- Data preprocessing and cleaning
- Model training and tuning
- Comparative evaluation
- Feature engineering
- Misclassification analysis
- Literature benchmarking

Additional experimentation and documentation will continue as development progresses.

---

# Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- Matplotlib
- Jupyter Notebook

---

# Repository Structure

```text
├── data/
├── notebooks/
├── models/
├── plots/
├── results/
├── requirements.txt
└── README.md
```

---

# Contributors

- Omeed Lodin
- Asad Murad

---

# Future Work

Potential future extensions include:

- Deep learning approaches
- Ensemble optimization
- Dimensionality reduction techniques
- Cross-survey generalization
- Explainable AI methods for astronomical classification
- Expanded astrophysical feature engineering

---
