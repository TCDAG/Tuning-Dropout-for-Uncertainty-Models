# Tuning Dropout for Uncertainty Models
Example code for "Tuning machine learning dropout for subsurface uncertainty model accuracy" https://doi.org/10.1016/j.petrol.2021.108975

## Executive summary

Deep learning models focus on **prediction accuracy and minimizing prediction error**. Yet, for spatial models, **accurate predictions along with accurate and precise uncertainty models are critical.** 

Due to limited data veracity, data sparsity, and feature heterogeneity in the spatial setting, uncertainty is significant; therefore, **predicting a single estimate must be replaced with a prediction of the uncertainty distribution**.

**We propose a novel and easy to use objective function to summarize uncertainty model performance**.
The proposed function tunes deep learning models for optimum uncertainty accuracy and precision.

## Data

For this notebook example we have a problem that consists on predicting **permeability** from **porosity** and **acoustic impedance data**. We have selected this problem because we are primarily interested in capturing the uncertainty related to predictions of permeability based on existing data. 

This problem can be expanded to any prediction problem.

## Notebook contents

1. Executive summary
2. Objective
3. Introduction
4. Library importing
5. Functions
6. Dataset exploration
7. Dataset normalization and split
8. Deterministic prediction
  1. Model goodness evaluation
9. Uncertainty model generation
  1. Model goodness evaluation
10. Hyperparameter space exploration
  1. Summary of the training
11. Conclusions and observations

**NOTE**: The hyperparameter space exploration section might be too long to run, we have included the results of the grid search in Search-Space.pkl. Feel free to skip this section and load the results in Summary of the training subsection
