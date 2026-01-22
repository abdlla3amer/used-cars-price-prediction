# Used Cars Price Prediction --- End-to-End Regression Analysis

## Project Overview:
End-to-End Regression Analysis to predict used cars prices using Machine Learning, covering everything from Data Cleaning and EDA to Model Building and Evaluation.

## Data License and Attribution:
These data was offered by the 365DataScience.com team as a part of the Machine Learning in Python Course.

## Files:
1. Used Car Price Data.csv:
    * Original Dataset.
1. requirements.txt:
    * Project Dependencies.
1. Used Cars Price Prediction --- End-to-End Regression Analysis.ipynb:
    * Full Regression Analysis Jupyter Notebook File.
1. Used Cars Price Prediction --- End-to-End Regression Analysis.html:
    * Full Regression Analysis in HTML Format.

## Datasets Description:
1. Brand -> str:
    * Car Brand ['BMW', 'Mercedes-Benz', 'Audi', 'Toyota', 'Renault', 'Volkswagen', 'Mitsubishi'].
1. Price -> float:
    * Listed Price in US Dollars.
1. Body -> str:
    * Car Body Type ['sedan', 'van', 'crossover', 'vagon', 'other', 'hatch'].
1. Mileage -> int:
    * Number of miles the Car has run till the selling point.
1. EngineV -> float:
    * Engine Volume (Displacement) in Liters.
1. Registeration -> bool:
    * Whether the car was registered or not.
1. Year -> int:
    * Car production year.
1. Model -> str:
    * Car Model (Sub-Brand)
    * 312 Unique Values.

## Process:
1. Data Wrangling.
1. Data Assessing:
    * Assessing Datatypes.
    * Assessing Missing Values.
    * Assessing Duplicates.
    * Checking the Distribution of columns.
    * Checking for Outliers.
1. Data Cleaning:
    * Dropping 'Model' column.
    * Dropping rows with missing values.
    * Cutting top 1% of the data to remove outliers.
1. Checking OLS Assumptions.
    * Linearity Check (Handling non-linearity via Log-Linear Transformation.
    * Multicollinearity Check.
1. Feature Selection & Variance Inflation Factor Analysis.
1. Handling Categorical Variables.
    * Creating Dummy Variables
1. Fitting an OLS Linear Regression Model.
1. Model Testing.
1. Model Evaluation.

## Libraries Used:
1. numpy v-2.1.3
2. pandas v-2.2.3
3. matplotlib v-3.10.0
4. seaborn v-0.13.2
5. statsmodels v-0.14.4
6. scikit-learn v-1.6.1

## Model Evaluation:
The model was able to predict prices with residual percentage <= 25% of the target 56.77% of the times.
The model was able to predict prices with residual percentage > 25% of the target 43.23% of the times.

## Conclusion:
The model can represent a low percentage of the data with resiudal <= 25% of the target (56.77%).
There's an omitted variable bias.
Model isn't recommended for deployment without furhter adjustments and more data wrangling.
