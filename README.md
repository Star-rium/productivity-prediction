# Productivity Prediction AI/ML Project

a very scuff ML model to analyze and predict productivity with social media consumption using Linear Regression. This project is my first ML project so i am open to any improvement and suggestion if anyone happened to stumble upon this repo:D

- Dataset: [Social Media Addiction vs Productivity Dataset](https://www.kaggle.com/datasets/asifxzaman/social-media-addiction-vs-productivity-dataset)
- Model Score: 87.93% (R-squared score)

## File Structure

```
    productivity-prediction
    ├── 📂 data_set
    │   ├── 📄 social_media_productivity_6000.csv
    │   ├── 📄 social_media_productivity_train.csv
    │   └── 📄 social_media_productivity_test.csv
    ├── 📂 src
    │   └── 📓 main.ipynb
    ├── 📄 README.md
    └── 📄 LICENSE
```

## Libraries Used

- NumPy: For linear algebra implementation.
- Pandas: Data loading, structuring, EDA.
- Matplotlib & Seaborn: Data visualization, render null value heatmaps.
- Scikit-learn: Evaluation and performance comparison.

## Data Loading and Analysis

- The datasets are loaded from CSV files using pandas.
- Exploratory Data Analysis is used for initial inspection of the data structure summary statistics, and missing value detection visualized via a Seaborn heatmap.

## Data Preprocessing

- Rows containing null values (approximately 2% across all columns) were identified and dropped to ensure mathematical integrity.
- Categorical variables were converted to numerical formats. Specifically, the `addiction_level` feature was ordinal-mapped (Low: 0, Medium: 1, High: 2).

## Model used

- The core of this project is a Multiple Linear Regression (MLR) model built entirely from scratch.
- The project also includes a baseline Single Linear Regression implementation to observe the isolated relationship between study hours and the target productivity score.

## Evaluation method

- Mean Squared Error (MSE)
- R-squared Score

## Whats next?

- Probably revisit and improve this project by implementing multiple regression models and cross-validate them via R-squared score.
