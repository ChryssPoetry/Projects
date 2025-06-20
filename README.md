# Projects

California Housing Data Analysis
A machine learning-ready exploration of California’s housing market, featuring data-driven insights, preprocessing, visualizations, and predictive modeling using scikit-learn. This project is ideal for understanding housing trends, feature importance, and regression performance across California districts.

📊 Dataset Overview
Source: California Census Housing Data

Entries: 20,640

Features: 9

Index: longitude (set as DataFrame index)

🔍 Features
Column Name	Description
latitude	Latitude of the district
housing_median_age	Median age of houses in the district
total_rooms	Total number of rooms in the district
total_bedrooms	Total number of bedrooms in the district
population	Population in the district
households	Number of households
median_income	Median income of households (in tens of thousands)
median_house_value	Median value of houses (target variable, in USD)
ocean_proximity	Categorical value describing the district’s proximity to ocean

🧪 Missing Values
total_bedrooms: ~1% missing

Strategy: Imputation with median, or optionally, use models to predict missing values

🛠️ Project Structure
kotlin
Copy
Edit
├── data/
│   └── california_housing.csv
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_exploration_visuals.ipynb
│   ├── 03_regression_models.ipynb
├── models/
│   └── ridge_model.pkl
├── README.md
└── requirements.txt
🔍 Exploratory Data Analysis
Distributions of price, income, and housing age

Correlations with target (median_house_value)

Geospatial heatmaps using latitude and longitude

Categorical impact of ocean_proximity on prices

📈 Modeling Approach
Objective: Predict median_house_value

Algorithms Used:

Linear Regression

Ridge Regression (with alpha tuning)

Random Forest Regressor

Gradient Boosting Regressor

Evaluation:

MAE, RMSE, R² Score

Grid Search CV for hyperparameter optimization

⚙️ Requirements
bash
Copy
Edit
pip install -r requirements.txt
Key Packages
pandas

numpy

scikit-learn

matplotlib

seaborn

tqdm

ipywidgets (if using JupyterLab for progress bars)

🚀 How to Run
bash
Copy
Edit
# Inside your Jupyter Notebook:
!jupyter notebook
# or if using JupyterLab:
!jupyter lab
Explore each notebook in order (01_ → 03_).

🧠 Insights Gained
Income is the strongest predictor of housing prices

Ocean proximity increases median value significantly

Ridge regularization helps control overfitting in linear models

Tree-based models outperform linear models on this dataset

📂 License
MIT License © 2025 – Franklin Nwafor

🤝 Contributing
Contributions are welcome! Open a pull request or file an issue to improve documentation, modeling, or visualizations.








