# House Price Prediction using Machine Learning

### Overview

This project explores how different property attributes affect house prices and uses machine learning to estimate price from those features. The goal is to understand the strongest price drivers and compare a few regression approaches on the same dataset.

The notebook covers the full workflow: exploratory analysis, preprocessing, model training, evaluation, and visual interpretation of the results.

---

## Dataset Snapshot

**Dataset:** Housing Prices Dataset

**Rows:** 545

**Columns:** 13

**Target:** Price

### Input Features

* Area
* Bedrooms
* Bathrooms
* Stories
* Main Road Access
* Guest Room Availability
* Basement Availability
* Hot Water Heating
* Air Conditioning
* Parking
* Preferred Area
* Furnishing Status

---

## Methodology

### Data Understanding

* Reviewed the structure and summary statistics of the dataset
* Checked for missing values and duplicate records
* Studied feature relationships using visual analysis

### Data Preparation

* Converted yes/no fields into binary values
* Applied one-hot encoding to furnishing status
* Prepared the feature matrix for regression modeling

### Modeling

The following models were tested:

* Linear Regression
* Random Forest Regressor
* Tuned Random Forest Regressor

### Evaluation Metrics

Model quality was measured using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

---

## Model Results

| Model               |          MAE |         RMSE | R² Score |
| ------------------- | -----------: | -----------: | -------: |
| Linear Regression   |   970,043.40 | 1,324,506.96 |   0.6529 |
| Random Forest       | 1,022,560.05 | 1,401,496.84 |   0.6114 |
| Tuned Random Forest | 1,088,859.38 | 1,447,653.20 |   0.5854 |

### Best Result

The **Linear Regression** model performed best on the test set with an R² score of **0.6529**. It showed stronger generalization than the Random Forest-based variants for this dataset.

---

## Main Observations

### Most Important Features

1. Area
2. Bathrooms
3. Air Conditioning
4. Parking
5. Stories

### Practical Takeaways

* Larger properties generally have higher prices.
* Bathrooms have a strong positive effect on price.
* Comfort-related features such as air conditioning and parking add noticeable value.
* Furnishing status also influences the final market price.
* The dataset shows a fairly clear linear pattern, which explains why Linear Regression performed well.

---

## Visual Outputs

The repository includes charts for:

* House price distribution
* Correlation heatmap
* Actual vs predicted prices
* Price vs area relationship
* Feature importance comparison

---

## Tools and Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Project Layout

```text
HousePricePrediction_Binaha/
├── Housing.csv
├── analysis.ipynb
├── README.md
└── charts/
    ├── house_price_distribution.png
    ├── correlation_heatmap.png
    ├── actual_vs_predicted.png
    ├── price_vs_area.png
    └── feature_importance.png
```

---

## Author

**Binaha Mary**

AI & Data Science Intern

Xylofy AI
