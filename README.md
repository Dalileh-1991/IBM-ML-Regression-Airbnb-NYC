# NYC Airbnb Price Prediction (Regression Models) — IBM Coursera Assignment

This repository contains my final project notebook for an **IBM Coursera Machine Learning / Regression assignment**.  
The goal is to build and compare several **linear regression** models on the **NYC Airbnb 2019** dataset, select the best model based on performance, and communicate insights clearly.

## Project Objective
Predict Airbnb listing **nightly price** (using `log1p(price)` for better modeling) and identify key drivers of price using interpretable regression models.

## Dataset
- **Dataset:** NYC Airbnb Open Data (2019)
- Commonly available on Kaggle as `AB_NYC_2019.csv`
- **Target variable:** `price` (modeled as `log1p(price)`)

> Note: The notebook expects the dataset file `AB_NYC_2019.csv` to be available in the working directory (Colab/Kaggle).

## Methods & Models Compared
This notebook follows a beginner-friendly workflow:
1. **Data Summary** (size, variables, missing values)
2. **Objective of the Analysis**
3. **Data Preparation** (cleaning, handling missing values, log transform)
4. **Model Comparison**
   - Linear Regression
   - Ridge Regression
   - Lasso Regression
   - ElasticNet
   - Polynomial Features (degree=2) + Ridge (to capture mild nonlinearity)
5. **Findings & Interpretation** (feature importance via coefficients)
6. **Limitations & Next Steps**

## Evaluation Metrics
- **RMSE (log scale)** and **R²** on the test set  
- (Optional) **Cross-validation** can be enabled inside the notebook

## How to Run
### Option 1: Google Colab
1. Open the notebook in Colab
2. Upload `AB_NYC_2019.csv`
3. Run all cells (**Runtime → Restart and run all**)

### Option 2: Kaggle
1. Add the NYC Airbnb 2019 dataset to your Kaggle notebook
2. Make sure the filename matches `AB_NYC_2019.csv`
3. Run the notebook

## File
- `IBM_ML_Regression_AirbnbNY_Project_Dalileh_RubricReady_Updated.ipynb` — final cleaned notebook

## Key Takeaways (High Level)
- Regularized models (Ridge/Lasso/ElasticNet) can improve generalization vs. plain linear regression.
- Polynomial features may capture mild nonlinearity, but can increase complexity.
- Coefficients offer interpretable insights into which features are associated with higher/lower prices.

## Author
Dalileh Oladzadeh AbbasAbadi

## License
For educational use.
