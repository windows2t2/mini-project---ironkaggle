# 🏠 IronKaggle — King County House Price Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.x-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-2.x-lightgrey?logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)

A machine learning mini-project that predicts house sale prices in King County (Washington, USA) using **regression models**.  
Part of the **Ironhack Data Analytics Bootcamp**.

---

## 📖 Overview

Your mission is to delve into a dataset of **house sale prices for King County** (including Seattle), spanning one year from **May 2014 to May 2015**. This project encompasses:

- 📥 **Data loading** & cleaning
- 📊 **Exploratory visualization** & correlation analysis
- 🤖 **Training multiple regression models**
- 📈 **Evaluating and comparing performance**
- 🏆 **Selecting the best model** for price prediction

The goal is to enhance your Python skills, deepen your understanding of real estate data, and hone your analytical prowess.

---

## 👥 Setup

This is a **team-based project** tackled over **three days**, simulating real-world real estate analysis scenarios. It fosters:

- Collaborative problem-solving
- Practical application of Python in real estate finance
- End-to-end machine learning workflow experience

---

## 📊 About the Data

> 📥 Source: [Kaggle — King County Houses AA](https://www.kaggle.com/datasets/minasameh55/king-country-houses-aa)

The dataset (`king_county_houses_aa.csv`) contains **home sales records** from King County with **21 columns**:

### 🏷️ Property Features

| Column | Description |
|--------|-------------|
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms (per bedroom) |
| `sqft_living` | Square footage of interior living space |
| `sqft_lot` | Square footage of the land space |
| `floors` | Number of floors (levels) |
| `waterfront` | Whether the house has a waterfront view |
| `view` | Number of times the house has been viewed |
| `condition` | Overall condition of the house |
| `grade` | Grade based on King County grading system |
| `sqft_above` | Square footage apart from the basement |
| `sqft_basement` | Square footage of the basement |
| `yr_built` | Year the house was built |
| `yr_renovated` | Year the house was renovated |

### 📍 Location & Neighborhood

| Column | Description |
|--------|-------------|
| `zipcode` | ZIP code area |
| `lat` | Latitude coordinate |
| `long` | Longitude coordinate |
| `sqft_living15` | Living space of the nearest 15 neighbors (2015) |
| `sqft_lot15` | Land space of the nearest 15 neighbors (2015) |

### 🔑 Identifiers & Target

| Column | Description |
|--------|-------------|
| `id` | Unique identifier for a house |
| `date` | Date on which the house was sold |
| `price` | 🎯 **Sale price** — our prediction target |

> 🎯 **Primary Focus:** Understand which features most significantly impact house price. Properties valued at **$650K and above** are explored for deeper insights.

---

## 🧪 Approach

The analysis follows a structured **11-step machine learning workflow**:

| Step | Action | Details |
|:----:|--------|---------|
| 1 | **Load** | Import libraries and read the CSV dataset |
| 2 | **Explore** | `.info()`, `.describe()`, check for nulls & duplicates |
| 3 | **Clean** | Parse dates, extract `year_sold`/`month_sold`/`day_sold` |
| 4 | **Split** | 80/20 train-test split; drop `id` and `date` |
| 5 | **Correlate** | Pearson correlation heatmap; identify top predictors |
| 6 | **Encode** | Cast categorical features to `float` |
| 7 | **Standardize** | `StandardScaler` for distance-based models |
| 8 | **Train** | Fit 8 baseline regression models |
| 9 | **Evaluate** | R², MAE, RMSE; bar-chart comparison |
| 10 | **Improve** | Handle outliers, feature engineering, hyperparameter tuning |
| 11 | **Select** | Pick the best model; identify key price drivers |

---

## 🤖 Models Trained

| Model | Type |
|-------|------|
| **Linear Regression** | Baseline linear |
| **Lasso** | Regularized linear (L1) |
| **Ridge** | Regularized linear (L2) |
| **K-Nearest Neighbors** | Distance-based |
| **Decision Tree** | Tree-based |
| **Random Forest** | Ensemble — bagging |
| **Gradient Boosting** | Ensemble — boosting |
| **AdaBoost** | Ensemble — adaptive boosting |

---

## 📈 Evaluation Metrics

| Metric | Meaning | Goal |
|--------|---------|------|
| **R² Score** | Proportion of variance explained | Higher is better |
| **MAE** | Mean Absolute Error | Lower is better |
| **RMSE** | Root Mean Squared Error | Lower is better (penalizes large errors) |

Results are visualized with horizontal bar charts comparing all models across the three metrics.

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/windows2t2/mini-project---ironkaggle.git
cd mini-project---ironkaggle

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# 3. Launch the notebook
jupyter notebook mycode.ipynb

# 4. Run all cells → see results!
```

---

## 📁 Project Structure

```
📦 mini-project---ironkaggle
├── 📄 README.md                  # You are here
├── 📊 king_county_houses_aa.csv  # Dataset (21 columns)
└── 📓 mycode.ipynb               # Jupyter Notebook — full analysis
```

---

## 📦 Deliverables

- ✅ **Jupyter Notebook** — detailed analysis & prediction model
- ✅ **Mini-Presentation** — ML process overview (6–15 min)
- ✅ **README** — machine learning steps & decisions

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
- Apply **feature engineering** (e.g., house age, renovation flag)
- Perform **hyperparameter tuning** with `GridSearchCV` / `RandomizedSearchCV`
- Try **XGBoost**, **LightGBM**, or **CatBoost**
- Use **cross-validation** for more robust evaluation

---

> Made with ❤️ during the Ironhack Data Analytics Bootcamp
