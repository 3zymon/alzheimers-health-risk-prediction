# Alzheimer's Health Risk Prediction
## About the project
Predicting the percentage of older adults experiencing frequent mental distress using previous-year data and demographic information.

## DatasetDataset
The project uses the CDC Healthy Aging Data, focusing on the indicator:

Q03 — Percentage of older adults who are experiencing frequent mental distress.

The dataset contains observations from 2015 to 2022 across different locations and demographic groups.

Source: https://data.cdc.gov/Healthy-Aging/Alzheimer-s-Disease-and-Healthy-Aging-Data/hfr9-rurv/data_preview
## Research question
Can we predict the percentage of older adults experiencing frequent mental distress in the following year based on the previous year’s value and demographic information?

## Methodology
Methodology

* Cleaned and prepared the dataset.
* Created a previous-year feature for the target variable.
* Used a chronological train, validation, and test split.
* Applied one-hot encoding to categorical features.
* Trained and compared three regression models:
    * Linear Regression
    * Random Forest Regressor
    * Gradient Boosting Regressor

## Results
Linear Regression achieved the lowest validation MSE among the three tested models.

On the test set:
* Test MSE: 4.27
* Test RMSE: 2.07
* Baseline MSE: 15.23
* MSE reduction compared with baseline: 72%

## Project structure

```
alzheimers-health-risk-prediction/
├── data/
├── analysis.ipynb
├── README.md
└── .gitignore
```

The dataset is not included in the repository because of its file size.

## How to run

1. Clone the repository.
2. Install the required Python packages.
3. Open analysis.ipynb in Jupyter Notebook.
4. Download the dataset and place it in the data/ directory.
5. Run the notebook cells in order.
