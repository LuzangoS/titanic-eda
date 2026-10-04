# Titanic Survival: Exploratory Data Analysis

An exploratory data analysis (EDA) of the Titanic passenger dataset. The goal is to understand which passenger characteristics were linked to survival before building any prediction model.

## What the notebook covers

1. **Dataset overview:** shape, column types, and summary statistics
2. **Missing value analysis:** Age (~20% missing), Cabin (~77%), Embarked (2 rows)
3. **Target variable:** 38.4% of passengers survived, 61.6% did not
4. **Univariate analysis:** histograms, box plots (outliers), and bar charts for categorical features
5. **Bivariate analysis:** survival rate by sex, class, port of embarkation, age, fare, and family size
6. **Correlation analysis:** heatmap of how the numeric features relate to survival
7. **Feature engineering:** `FamilySize` (SibSp + Parch + 1) and `Title` (extracted from names)

## Key findings

- Sex was the strongest factor: about 74% of women survived versus about 19% of men.
- Passenger class mattered: first class survived far more often than third class.
- Small families (2 to 4 people) had the best survival rates.
- Cabin has too much missing data to be reliable.

## Requirements

- Python 3.9 or newer
- pandas
- numpy
- matplotlib
- seaborn
- jupyter

Install them with:

```bash
pip install -r requirements.txt
```

## How to run

1. Clone the repository:
```bash
   git clone https://github.com/LuzangoS/titanic-eda.git
   cd titanic-eda
```
2. Install the requirements (see above).
3. Open the notebook in VS Code or Jupyter and choose **Run All**.

## Data

`train.csv` comes from the Kaggle competition [Titanic: Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic). It has 891 passengers and 12 columns.

## Next steps

- Clean the data (fill missing ages, drop Cabin)
- Encode categorical features
- Train and evaluate a prediction model
