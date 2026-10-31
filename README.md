# Advertising Sales Prediction — Linear Regression

A guided classroom exercise from my **Route Academy AI & Machine Learning diploma**, with brief documentation added as part of my learning portfolio.

## Overview
This notebook explores how advertising spending across **TV, Radio, and Newspaper** relates to **Sales**, using simple and multiple linear regression.

## Dataset
- 200 observations and 4 columns: `TV`, `Radio`, `Newspaper`, `Sales`
- Original classroom data source: https://raw.githubusercontent.com/justmarkham/scikit-learn-videos/master/data/Advertising.csv
- A local copy is included as `advertising.csv`

## Workflow
1. Load and inspect the dataset; check missing values and duplicates.
2. Visualize feature relationships with scatter plots and a correlation heatmap.
3. Train a simple linear regression model using TV spending.
4. Train a multiple linear regression model using all three advertising channels.
5. Evaluate on a held-out 20% test set and compare feature combinations.

## Results (held-out test set)
| Model | R² | MAE | RMSE |
| --- | ---: | ---: | ---: |
| TV only | 0.662 | 2.457 | 3.266 |
| TV + Radio + Newspaper | 0.906 | 1.275 | 1.705 |

The multi-feature model performs better on this split. These figures are from the classroom notebook and should not be interpreted as evidence of causality or production readiness.

## How to run
Keep `Advertising_Linear_Regression_Annotated.ipynb` and `advertising.csv` in the same folder. Open the notebook in Jupyter or upload both files to Kaggle, then run the cells in order. On Kaggle, you may need to adjust the CSV path to the location of the attached dataset.

Python libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`.

## Acknowledgment
Based on a hands-on classroom exercise at **Route Academy**. Grateful to my instructor for the guidance and support throughout the learning process.
