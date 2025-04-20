# Bluebook for Bulldozers - Sale Price Prediction

## Project Goal

Predict the auction sale price of heavy equipment using machine learning, targeting the Kaggle "Bluebook for Bulldozers" competition. This solution uses `fastai` for preprocessing and `scikit-learn`'s `RandomForestRegressor` for modeling.

## Workflow Summary

1.  **Load & Explore Data:** Import `TrainAndValid.csv` and `Test.csv`, perform initial EDA.
2.  **Preprocess with Fastai:** Apply `add_datepart`, `Categorify`, and `FillMissing` to handle dates, categorical features, and missing values. Prepare data using `TabularPandas`.
3.  **Train Random Forest:** Split data (validate on 2012 sales) and train a `RandomForestRegressor`.
4.  **Evaluate & Analyze:** Assess model using RMSLE and R² score; analyze feature importances.
5.  **Save Model:** Persist the trained model (`.pkl`).

## Dataset

*   **Source:** [Kaggle - Bluebook for Bulldozers](https://www.kaggle.com/c/bluebook-for-bulldozers)
*   **Target:** `SalePrice`
*   **Metric:** Root Mean Squared Log Error (RMSLE)

## Key Technologies

*   `fastai.tabular`
*   `pandas`
*   `numpy`
*   `scikit-learn` (specifically `RandomForestRegressor`)
*   `Jupyter Notebook`

## Getting Started

1.  **Clone:** `git clone https://github.com/adarsh070/Bluebook_for_bulldozers.git && cd Bluebook_for_bulldozers`
2.  **Setup Env & Install:** Create a Python virtual environment and install dependencies
    
3.  **Get Data:** Download `TrainAndValid.csv` and `Test.csv` from Kaggle and place them in the repository root.
4.  **Run Notebook:** Launch `jupyter notebook Bluebook_for_Bulldozers_prediction.ipynb` and execute the cells.

## Results

Performance on the validation set (year 2012):

*   **RMSLE:** **9.074178708482999e-05**
*   **R² Score:** **0.9999999831069084**



Adarsh - [https://github.com/adarsh070]
