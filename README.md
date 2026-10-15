# MOKCa-GofLof: Machine Learning Models for Functional Variant Classification

## Overview

This repository contains Jupyter notebooks (`.ipynb`) for machine-learning analyses aimed at classifying genetic variants according to their functional effects. The repository is organised into three directories, each addressing a different classification task: gain-of-function (GOF) versus loss-of-function (LOF), multi-class classification of neutral, GOF, and LOF variants, and binary classification of neutral versus pathogenic variants.

The notebooks document the model training and analysis workflows and provide a reproducible starting point for exploring machine-learning approaches to functional variant classification.

## Repository Structure

### 1. `GOFvsLOF_ML/` — GOF vs LOF Classification

**Task:** Binary classification of gain-of-function (GOF) and loss-of-function (LOF) variants.

This directory contains Jupyter notebooks for training and evaluating machine-learning models to distinguish GOF variants from LOF variants.

Three machine-learning algorithms are used:

- **Random Forest** — an ensemble learning method based on multiple decision trees.
- **XGBoost (XGB)** — a gradient-boosting algorithm that builds an ensemble of decision trees.
- **LightGBM** — a gradient-boosting framework designed for efficient model training.

The objective is to investigate the ability of these algorithms to distinguish between GOF and LOF variants based on the features provided to the models.

[**Explore GOFvsLOF_ML →**](https://github.com/UOSbioinformaticslab/MOKCa-GofLof/tree/main/GOFvsLOF_ML)

### 2. `Multi-class-ML/` — Three-Class Classification

**Task:** Multi-class classification of variants into three categories:

- **Neutral**
- **Gain-of-function (GOF)**
- **Loss-of-function (LOF)**

This directory contains Jupyter notebooks for training machine-learning models to distinguish between neutral, GOF, and LOF variants within a single classification framework.

Unlike binary classification, this task requires the model to discriminate among all three classes. The notebooks support the investigation of machine-learning approaches for identifying the functional category of a variant.

[**Explore Multi-class-ML →**](https://github.com/UOSbioinformaticslab/MOKCa-GofLof/tree/main/Multi-class-ML)

### 3. `NeutralvsPathogenic_ML/` — Neutral vs Pathogenic Classification

**Task:** Binary classification of neutral and pathogenic variants.

This directory contains Jupyter notebooks for training machine-learning models to distinguish between neutral variants and pathogenic variants.

The objective is to investigate whether the features provided to the models can support the classification of variants into these two categories.

[**Explore NeutralvsPathogenic_ML →**](https://github.com/UOSbioinformaticslab/MOKCa-GofLof/tree/main/NeutralvsPathogenic_ML)

## Getting Started

### Requirements

The notebooks are designed to run in a Python environment with Jupyter Notebook or JupyterLab. The exact dependencies depend on the packages imported in each notebook and may include:

- Python
- Jupyter Notebook or JupyterLab
- pandas
- NumPy
- scikit-learn
- XGBoost
- LightGBM
- Matplotlib and Seaborn, where required for visualisation

### Running the Notebooks

1. Clone or download this repository.
2. Set up a Python environment with the dependencies required by the notebook you intend to run.
3. Open the relevant `.ipynb` file in Jupyter Notebook, JupyterLab, or Google Colab.
4. Ensure that any required input datasets are available at the paths specified in the notebook.
5. Execute the notebook cells in order to reproduce the corresponding analysis.

**Note:** The availability of input datasets and the exact steps required to reproduce each analysis depend on the individual notebook.

## Summary of Classification Tasks

| Directory | Classification task | Number of classes | Classes |
|---|---|---:|---|
| `GOFvsLOF_ML/` | GOF vs LOF | 2 | GOF, LOF |
| `Multi-class-ML/` | Functional classification | 3 | Neutral, GOF, LOF |
| `NeutralvsPathogenic_ML/` | Neutral vs pathogenic | 2 | Neutral, Pathogenic |

## Intended Use

This repository is intended for research into machine-learning approaches for genetic variant classification and functional effect prediction. Model performance and predictions should be interpreted in the context of the datasets, feature selection, training procedures, and validation strategies used in the notebooks.

Predictions from these models should not be treated as definitive clinical classifications without appropriate independent validation.

## Repository

GitHub: [UOSbioinformaticslab/MOKCa-GofLof](https://github.com/UOSbioinformaticslab/MOKCa-GofLof)

