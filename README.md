# IDS_XAI_Generative_Shift
# Day 1

## Overview

IDS_XAI_Generative_Shift is a cybersecurity analytics project built using the UNSW-NB15 dataset. The project focuses on intrusion detection, explainable AI (XAI), synthetic data generation, and explanation stability analysis.

The objective is to understand network behavior, detect potential intrusions, and evaluate whether model explanations remain consistent under distribution shifts.

---

## Project Objectives

* Explore and understand the UNSW-NB15 dataset.
* Perform data preprocessing and feature preparation.
* Build a baseline LSTM workflow for intrusion detection.
* Generate synthetic shifted data for distribution shift analysis.
* Apply SHAP-based explainability techniques.
* Analyze explanation stability under shifted data conditions.

---

## Dataset

Dataset Used:

UNSW-NB15

The dataset contains both normal and malicious network traffic records and is widely used for intrusion detection research.

---

## Project Structure

IDS_XAI_Generative_Shift/

├── data/

│   ├── raw/

│   └── processed/

│

├── notebooks/

│   ├── 01_dataset_exploration.ipynb

│   ├── 02_preprocessing.ipynb

│   ├── 03_lstm_gru_baseline.ipynb

│   ├── 04_vae_shift_generation.ipynb

│   ├── 05_xai_shap_lime.ipynb

│   └── 06_explanation_stability.ipynb

│

├── results/

│   ├── tables/

│   ├── figures/

│   └── logs/

│

├── paper_notes/

│   ├── experiment_log.xlsx

│   └── result_summary.docx

│

└── README.md

---

## Workflow

### 1. Dataset Exploration

* Dataset profiling
* Missing value analysis
* Attack category analysis
* Initial visualizations

### 2. Data Preprocessing

* Missing value handling
* Duplicate removal
* Categorical encoding
* Feature scaling

### 3. Baseline Modeling

* LSTM workflow preparation
* Feature-target separation
* Data splitting and scaling

### 4. Synthetic Shift Generation

* Synthetic dataset creation
* Distribution shift simulation

### 5. Explainable AI

* SHAP-based feature importance analysis
* Model interpretation workflow

### 6. Explanation Stability Analysis

* Comparison of explanation consistency
* Stability score generation
* Visualization of explanation behavior

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow
* SHAP

---

## Deliverables

* UNSW_NB15_Master.csv
* preprocessed_unsw.csv
* synthetic_shifted.csv
* Dataset exploration notebook
* Preprocessing notebook
* Baseline modeling notebook
* Explainability notebook
* Stability analysis notebook

---

## Current Status

Initial project structure and workflow completed. Further improvements may include advanced deep learning models, enhanced explainability techniques, and comprehensive evaluation metrics.

---

## Day 2 
We focused on implementing and evaluating deep learning models for intrusion detection using the preprocessed UNSW-NB15 dataset.

Completed Activities:

* Implemented CNN baseline model
* Implemented RNN baseline model
* Implemented LSTM baseline model
* Implemented BiLSTM baseline model
* Implemented GRU baseline model
* Generated evaluation metrics including Accuracy, Precision, Recall, F1-Score, ROC-AUC, Training Time, and Inference Time
* Performed confusion matrix analysis
* Created model comparison documentation
* Prepared baseline hyperparameter documentation
* Generated Day 2 technical report and presentation

Outcome:
All five deep learning models were successfully executed and evaluated. CNN demonstrated the fastest execution time, while RNN, LSTM, BiLSTM, and GRU achieved perfect classification performance on the preprocessed UNSW-NB15 dataset.

# Day 3 – Synthetic Data Augmentation and Validation

## Project

IDS_XAI_Generative_Shift

## Objective

The objective of Day 3 was to address class imbalance in the UNSW-NB15 dataset by generating synthetic samples for minority attack classes using CTGAN (Conditional Tabular Generative Adversarial Network) and validating the quality of the generated data using statistical and machine learning techniques.

---

## Work Completed

### 1. Class Distribution Analysis (CDA)

* Analyzed attack category distribution in the UNSW-NB15 dataset.
* Identified minority attack, classes.
* Evaluated dataset imbalance.
* Generated class distribution tables and visualizations.

### 2. CTGAN-Based Data Augmentation

* Trained CTGAN on the processed UNSW-NB15 dataset.
* Generated synthetic samples for minority attack classes.
* Created an augmented dataset by combining original and synthetic data.
* Evaluated class balance improvement after augmentation.

### 3. Augmented Data Validation (ADV)

* Compared original and augmented datasets.
* Performed Jensen-Shannon Divergence analysis.
* Performed Kolmogorov-Smirnov statistical testing.
* Conducted Random Forest validation to assess distinguishability between real and synthetic samples.
* Generated feature importance analysis.

---

## Folder Structure

```text
Day 3
│
├── CDA
│   └── Class Distribution Analysis files
│
├── CTGAN
│   └── Synthetic Data Augmentation files
│
├── ADV
│   └── Augmented Data Validation files
│
├── Reports
│   └── Documentation and summary reports
│
├── Tables
│   └── CSV output files
│
├── Figures
│   └── Generated graphs and visualizations
│
└── Presentation
    └── Progress presentation
```

---

## Key Outputs

### Generated Datasets

* augmented_dataset_unsw_nb15.csv
* data_balanced_random.csv

### Generated Tables

* Class Distribution Comparison
* Augmentation Comparison
* Jensen-Shannon Divergence Results
* Kolmogorov-Smirnov Test Results
* Feature Importance Results
* Validation Metrics Summary

### Generated Figures

* Attack Distribution Analysis
* Class Distribution Comparison
* Imbalance Ratio Comparison
* CTGAN Augmentation Results
* Jensen-Shannon Divergence Analysis
* Random Forest Validation Results
* Feature Importance Analysis
* KS Test Analysis

---

## Validation Techniques Used

### Statistical Validation

* Jensen-Shannon Divergence (JSD)
* Kolmogorov-Smirnov (KS) Test

### Machine Learning Validation

* Random Forest Classifier
* Feature Importance Analysis

---

## Outcome

* Successfully generated synthetic attack samples using CTGAN.
* Improved minority class representation.
* Created an augmented dataset for future IDS model training.
* Validated the quality and similarity of synthetic data using statistical and machine learning approaches.

---

## Status

Day 3 Completed Successfully

Project: IDS_XAI_Generative_Shift
Dataset: UNSW-NB15
Methodology: CTGAN-Based Synthetic Data Augmentation and Validation

