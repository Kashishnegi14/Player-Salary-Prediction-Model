# Player-Salary-Prediction-Model
This project predicts MLB player salaries using machine learning. It processes player data like height, weight, batting/throwing hand, and league info from the mlb_salaries.csv dataset, and trains a Random Forest Regressor to estimate salaries. The model is evaluated using MAE, RMSE, and R² score.
# ⚾ MLB Player Salary Prediction

This project aims to predict Major League Baseball (MLB) player salaries using machine learning techniques based on player attributes like height, weight, batting/throwing hand, and team information.

## 📁 Dataset

The dataset used is `mlb_salaries.csv`, which contains various player details including:

- `player_name`
- `weight`, `height`
- `bats`, `throws`
- `season`, `league`, `team`
- `salary` (target variable)

## 🧹 Data Preprocessing

- Dropped irrelevant columns (`playerid`, `teamid`, `franchise`, etc.)
- Handled missing values
- Converted categorical columns (`bats`, `throws`, `league`) using one-hot encoding
- Normalized features (if required)

## 📊 Exploratory Data Analysis

- Visualized salary distribution
- Checked feature correlations using a heatmap

## 🤖 Model Training

- Used `RandomForestRegressor` for regression
- Trained on `X_train`, evaluated on `X_test`
- Evaluation metrics:
  - **MAE (Mean Absolute Error)**
  - **RMSE (Root Mean Squared Error)**
  - **R² Score**

## 📈 Results

Example model performance:

- **MAE**: 1,856,667.33
- **RMSE**: 3,200,000+
- **R² Score**: ~0.73 (depending on final feature engineering)

## 🛠 Libraries Used

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

## 📌 Future Improvements

- Try different models (XGBoost, SVR)
- Perform hyperparameter tuning
- Include additional player stats if available (e.g., batting average, home runs)


---

