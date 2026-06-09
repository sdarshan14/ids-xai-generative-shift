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


