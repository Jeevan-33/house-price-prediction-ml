# 🏠 House Price Prediction using Machine Learning

A machine learning project that predicts residential house prices using property characteristics such as overall quality, living area, garage capacity, and construction year.

Built using Python and Scikit-learn as part of my hands-on learning journey in Machine Learning.

## 📌 Project Overview

The objective of this project is to develop a regression model that can accurately estimate house prices based on historical housing data.

The project follows an end-to-end machine learning workflow, from exploratory data analysis and feature engineering to model training, hyperparameter tuning, and evaluation.

**Dataset:** [Kaggle – House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 📂 Project Structure

```text
house-price-prediction-ml/
│
├── house_price_prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## 🔍 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Analyzed dataset structure and feature distributions.
- Identified and examined missing values.
- Studied correlations between numerical features and SalePrice.
- Visualized relationships using Matplotlib and Seaborn.

### 2. Data Preprocessing
- Handled missing numerical values using median imputation.
- Standardized numerical features for Ridge Regression.
- Split data into training and testing sets.

### 3. Feature Engineering

Created additional features to improve prediction:

- `TotalSF`: Total basement and floor area.
- `TotalBath`: Total bathroom count, including half bathrooms.
- `HouseAge`: Age of the house at the time of sale.
- `RemodAge`: Years since the last remodeling.
- `HasGarage`: Indicates whether the property has a garage.

### 4. Model Development

Implemented and compared:

- Mean Baseline Regression
- Ridge Regression
- Decision Tree Regressor
- Random Forest Regressor

### 5. Model Evaluation and Optimization

- Used 5-Fold Cross-Validation.
- Evaluated Random Forest using Out-of-Bag (OOB) scoring.
- Applied RandomizedSearchCV for hyperparameter tuning.
- Used Permutation Feature Importance to understand feature contributions.

## 📊 Final Model Performance

The final model was evaluated on a separate 20% holdout test set.

| Metric | Result |
|---|---:|
| RMSE | 30,863.67 |
| R² Score | 0.8758 |

The model achieved an R² score of 0.8758, indicating that it explains approximately 87.58% of the variation in house prices on the holdout dataset.

## 🚀 How to Run the Project

**1. Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/house-price-prediction-ml.git
```

**2. Navigate to the project directory**

```bash
cd house-price-prediction-ml
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Download the dataset**

Download `train.csv` and `test.csv` from the [Kaggle competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data).

Place both files in the project directory.

**5. Launch Jupyter Notebook**

```bash
jupyter notebook
```

Open `house_price_prediction.ipynb` and run the cells.

## 🎯 Learning Outcomes

Through this project, I gained practical experience in:

- Exploratory Data Analysis
- Data preprocessing and missing-value handling
- Feature engineering
- Regression algorithms
- Cross-validation
- Hyperparameter optimization
- Model evaluation and interpretation

## 👨‍💻 Author

**Jeevan AE**

AI & Machine Learning Engineering Student

---

⭐ If you find this project useful, feel free to explore the notebook and share your feedback.

**Project Type:** Supervised Machine Learning | Regression
