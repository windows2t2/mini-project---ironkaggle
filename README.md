Overview


Your mission is to delve into a dataset of house sale prices for King County, including Seattle, spanning one year from May 2014 to May 2015. This project encompasses various computational tasks such as data loading, visualization, calculating returns, and portfolio analysis, tailored to the real estate domain. It aims to enhance your Python skills, deepen your understanding of real estate financial data, and hone your analytical prowess. Are you ready to embark on this analytical journey through the housing market?
Setup

You'll be undertaking this project in teams, tackling different components of the analysis across three days. The project is designed to simulate real-world real estate analysis scenarios, fostering collaborative problem-solving and the practical application of Python in real estate finance.
About the Data:

This dataset comprises one-year data (from May 2014 to May 2015) of house sale prices across King County, including Seattle. It features 21 different columns, providing a comprehensive overview of the real estate market:

    id: A unique identifier for a house.
    date: The date on which the house was sold.
    price: The sale price of the house (prediction target).
    bedrooms: Number of bedrooms in the house.
    bathrooms: Number of bathrooms in the house, per bedroom.
    sqft_living: Square footage of the interior living space.
    sqft_lot: Square footage of the land space.
    floors: Number of floors (levels) in the house.
    waterfront: Whether the house has a waterfront view.
    view: Number of times the house has been viewed.
    condition: The overall condition of the house.
    grade: The overall grade given to the house, based on the King County grading system.
    sqft_above: Square footage of the house apart from the basement.
    sqft_basement: Square footage of the basement.
    yr_built: The year the house was built.
    yr_renovated: The year the house was renovated.
    zipcode: ZIP code area.
    lat: Latitude coordinate.
    long: Longitude coordinate.
    sqft_living15: The interior living space for the nearest 15 neighbors in 2015.
    sqft_lot15: The land spaces for the nearest 15 neighbors in 2015.
    TARGET --> Price: Our primary focus is to understand which features most significantly impact the house price. Additionally, we aim to explore properties valued at $650K and above for more detailed insights.

Deliverables:

    A Jupyter notebook detailing the analysis and model for predicting house sales prices.
    A mini-presentation outlining the machine learning process used in the analysis.
    A README file explaining the machine learning steps and decisions made throughout the project.
    Presentation time: 6 - 15min.



For your first Machine Learning project, you’ll build a regression model to predict house prices based on their characteristics. Please follow the steps below:

1. Load the dataset.
2. Explore the data to understand its structure — features, target variable, shape, and data types.
3. Clean the dataset (handle duplicates, missing values, etc.).
4. Split the dataset into features (X) and target (y).
5. Explore correlations between the target and features, and among features. Include your interpretations.
6. Handle categorical variables (encoding).
7. Train baseline models such as Linear Regression and KNN Regressor.
8. Evaluate the models using metrics like R² and MAE.
9. Improve your models:
    - Data side: handle outliers, multicollinearity, feature selection, normalization/standardization, feature engineering, etc.
    - Model side: try other models (especially ensemble methods) and perform hyperparameter tuning.
10. Compare all models and select the best one.
11. Identify which features most strongly influence house prices based on your best model.

Deliverables:
- A Jupyter Notebook containing all analysis, code, and results.
- A Presentation (15 minutes) summarizing your ML process, insights, and final model.
- A README file explaining your workflow, reasoning, and key decisions.
