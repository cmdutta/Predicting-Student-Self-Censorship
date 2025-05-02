# Predicting Student Self-Censorship: Behavioral Insights from the Campus Expression Survey

Using the 2024 Campus Expression Survey, I model predictors of student reluctance to express honest opinions on controversial topics. A downsampled Random Forest classifier achieves a balanced accuracy of 62%, identifying neuroticism, political orientation, and peer consequence concerns as key predictors. Dimensionality reduction via PCA reveals that discomfort is largely driven by a single latent factor—general reluctance—rather than topic-specific variation, a finding reinforced by latent profile analysis.


## Project Structure

- `data_ingestion/load_clean_data.Rmd` – Loads and cleans raw CES survey data.
- `feature_engineering/feature_generation.Rmd` – Constructs features like composite reluctance scores and political ideology.
- `pca_clustering.Rmd` – Runs PCA and clustering on discussion reluctance patterns.
- ``modeling/`regression_models.Rmd` – Fits linear and logistic regression models.
- `random_forest_cv.Rmd` – Random Forest classification with cross-validation and importance plots.
- `final_project_analysis.pdf` – Final report.

## Getting the Data

Data must be obtained directly from Heterodox Academy. No raw data is included in this repo.

## Reproducing the Report

You can run `report/final_project_analysis.Rmd` after executing the scripts in order:
1. `data_ingestion/load_clean_data.Rmd`
2. `feature_engineering/feature_generation.Rmd`
3. Scripts related to modeling 
4. Finally, knit: `final_project_analysis.Rmd`

## Obtaining the Datatset

This project uses the 2023 Campus Expression Survey (CES) administered by Heterodox Academy.

To obtain the dataset:
1. Visit https://heterodoxacademy.org/campus-expression-survey/
2. Locate the Campus Expression Survey (CES) 2023 report or contact HxA directly
3. Request or download the .Rdata file made available for educational use



