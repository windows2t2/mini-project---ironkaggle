# 🏠 IronKaggle — King County House Price Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.x-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-2.x-lightgrey?logo=pandas)
![License](https://img.shields.io/badge/License-MIT-green)

A machine learning mini-project that predicts house sale prices in King County (Washington, USA) using **regression models**.  
Part of the **Ironhack Data Analytics Bootcamp**.

---

## 📊 Dataset

The dataset (`king_county_houses_aa.csv`) contains **home sales records** from King County, including Seattle, between May 2014 and May 2015.

| Feature | Description |
|---------|-------------|
| `price` | Sale price (target variable) |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `sqft_living` | Square footage of living area |
| `sqft_lot` | Square footage of the lot |
| `floors` | Number of floors |
| `waterfront` | Waterfront view (0 or 1) |
| `view` | Number of times the house has been viewed |
| `condition` | Overall condition (1–5) |
| `grade` | Construction & design grade (1–13) |
| `sqft_above` | Square footage above ground |
| `sqft_basement` | Square footage of basement |
| `yr_built` | Year built |
| `yr_renovated` | Year renovated (0 if never) |
| `zipcode` | ZIP code |
| `lat` / `long` | Latitude / Longitude |

---

## 🧪 Approach

The analysis follows a structured **10-step workflow**:

1. **Load libraries** — Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
2. **Load the dataset** — Read CSV and inspect shape
3. **Explore the data** — `.info()`, `.describe()`, check for nulls & duplicates
4. **Clean the data** — Parse dates, extract `year_sold`, `month_sold`, `day_sold`
5. **Split** — 80/20 train-test split, drop `id` and `date`
6. **Correlation analysis** — Compute Pearson correlations, visualize with a heatmap
7. **Encode categoricals** — Cast all features to `float`
8. **Standardize** — `StandardScaler` for distance-based models (KNN, Lasso, Ridge)
9. **Train baseline models** — Fit 8 regressors on the scaled training set
10. **Evaluate & compare** — R², MAE, RMSE; bar charts; pick the best model

---

## 🤖 Models Trained

| Model | Type |
|-------|------|
| **Linear Regression** | Baseline linear |
| **Lasso** | Regularized linear (L1) |
| **Ridge** | Regularized linear (L2) |
| **K-Nearest Neighbors** | Distance-based |
| **Decision Tree** | Tree-based |
| **Random Forest** | Ensemble (bagging) |
| **Gradient Boosting** | Ensemble (boosting) |
| **AdaBoost** | Ensemble (adaptive boosting) |

---

## 📈 Evaluation Metrics

- **R² Score** — Proportion of variance explained (higher is better)
- **MAE** (Mean Absolute Error) — Average absolute prediction error
- **RMSE** (Root Mean Squared Error) — Penalizes large errors more heavily

Results are visualized with horizontal bar charts comparing all models across the three metrics.

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/windows2t2/mini-project---ironkaggle.git
   cd mini-project---ironkaggle
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. **Launch the notebook**
   ```bash
   jupyter notebook mycode.ipynb
   ```

4. **Run all cells** — The notebook will load the data, train all models, and display results.

---

## 📁 Project Structure

```
📦 mini-project---ironkaggle
├── 📄 README.md                  # You are here
├── 📊 king_county_houses_aa.csv  # Dataset
└── 📓 mycode.ipynb               # Jupyter Notebook with full analysis
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python 3** | Programming language |
| **Pandas** | Data manipulation & analysis |
| **NumPy** | Numerical computing |
| **Matplotlib / Seaborn** | Data visualization |
| **Scikit-Learn** | Machine learning models & metrics |
| **Jupyter Notebook** | Interactive development environment |

---

## 📝 Future Improvements

- Handle **outliers** and **multicollinearity**
- Apply **feature engineering** (e.g., age of house, renovation flag)
- Perform **hyperparameter tuning** with `GridSearchCV` or `RandomizedSearchCV`
- Try additional models like **XGBoost** or **LightGBM**
- Use **cross-validation** for more robust evaluation

---

> Made with ❤️ during the Ironhack Data Analytics Bootcamp

Overview
Your mission is to delve into a dataset of house sale prices for King County, including Seattle, spanning one year from May 2014 to May 2015.
This project encompasses various computational tasks such as data loading, visualization, calculating returns, and portfolio analysis, tailored to the real estate domain.
It aims to enhance your Python skills, deepen your understanding of real estate financial data, and hone your analytical prowess.
Are you ready to embark on this analytical journey through the housing market?

Setup
You'll be undertaking this project in teams, tackling different components of the analysis across three days.
The project is designed to simulate real-world real estate analysis scenarios, fostering collaborative problem-solving and the practical application of Python in real estate finance.

About the Data
https://www.kaggle.com/datasets/minasameh55/king-country-houses-aa
king_ country_ houses_aa.csv

This dataset comprises one-year data (from May 2014 to May 2015) of house sale prices across King County, including Seattle.

It features 21 different columns, providing a comprehensive overview of the real estate market:
    id: A unique identifier for a house
    date: The date on which the house was sold
    price: The sale price of the house (prediction target)
    bedrooms: Number of bedrooms in the house
    bathrooms: Number of bathrooms in the house, per bedroom
    sqft_living: Square footage of the interior living space
    sqft_lot: Square footage of the land space
    floors: Number of floors (levels) in the house
    waterfront: Whether the house has a waterfront view
    view: Number of times the house has been viewed
    condition: The overall condition of the house
    grade: The overall grade given to the house, based on the King County grading system
    sqft_above: Square footage of the house apart from the basement
    sqft_basement: Square footage of the basement
    yr_built: The year the house was built
    yr_renovated: The year the house was renovated
    zipcode: ZIP code area
    lat: Latitude coordinate
    long: Longitude coordinate
    sqft_living15: The interior living space for the nearest 15 neighbors in 2015
    sqft_lot15: The land spaces for the nearest 15 neighbors in 2015
    TARGET --> Price: Our primary focus is to understand which features most significantly impact the house price. Additionally, we aim to explore properties valued at $650K and above for more detailed insights

Deliverables
    A Jupyter notebook detailing the analysis and model for predicting house sales prices
    A mini-presentation outlining the machine learning process used in the analysis
    A README file explaining the machine learning steps and decisions made throughout the project
    Presentation time: 6 - 15min

For this Machine Learning project, you’ll build a regression model to predict house prices based on their characteristics

Please follow the steps below
1. Load the dataset
2. Explore the data to understand its structure — features, target variable, shape, and data types
3. Clean the dataset (handle duplicates, missing values, etc.)
4. Split the dataset into features (X) and target (y)
5. Explore correlations between the target and features, and among features. Include your interpretations
6. Handle categorical variables (encoding)
7. Train baseline models such as Linear Regression and KNN Regressor
8. Evaluate the models using metrics like R² and MAE
9. Improve your models:
    - Data side: handle outliers, multicollinearity, feature selection, normalization/standardization, feature engineering, etc.
    - Model side: try other models (especially ensemble methods) and perform hyperparameter tuning
10. Compare all models and select the best one
11. Identify which features most strongly influence house prices based on your best model

Deliverables
- A Jupyter Notebook containing all analysis, code, and results
- A Presentation (15 minutes) summarizing your ML process, insights, and final model
- A README file explaining your workflow, reasoning, and key decisions
