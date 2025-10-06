# 🐟 Fish Weight Prediction using Polynomial Ridge Regression

This project demonstrates how to predict the **weight of fish** using **Polynomial Regression with Ridge Regularization**.  
It explores the effect of polynomial degrees on model performance, analyzes overfitting/underfitting, and visualizes the regression fit.

---

## 📊 Project Overview

The dataset (`Fish.csv`) contains physical measurements of different fish species.  
The goal is to predict **fish weight** based on these features using a **regularized polynomial regression model**.

### 🔍 Steps Performed

1. **Data Loading**
   - Load the dataset using `pandas`.

2. **Preprocessing**
   - Normalize numeric columns using `MinMaxScaler`.
   - Encode categorical labels (`Species`) using `LabelEncoder`.

3. **Train-Test Split**
   - 80% training data, 20% testing data.

4. **Model Training**
   - Polynomial feature expansion for degrees 1 to 8.
   - Ridge Regression (`alpha = 1.0`) used to control overfitting.

5. **Evaluation**
   - Mean Squared Error (MSE) computed for each polynomial degree.
   - Best model selected based on **lowest test MSE**.

6. **Visualization**
   - MSE vs Polynomial Degree plot.
   - Polynomial regression fit for each feature.
   - Actual vs Predicted weight scatter plot.

---

## 🧩 Technologies Used

| Library | Purpose |
|----------|----------|
| `pandas` | Data loading & manipulation |
| `numpy` | Numerical computations |
| `scikit-learn` | Scaling, encoding, regression, and metrics |
| `matplotlib` | Visualization |

---

## 📁 Dataset

**Sample Columns:**
- `Species`
- `Weight`
- `Length1`
- `Length2`
- `Length3`
- `Height`
- `Width`

---

## ⚙️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/FishWeightRidgeRegression.git
   cd FishWeightRidgeRegression
   ```
2. Install dependencies:
```
pip install pandas numpy scikit-learn matplotlib
```
3. Run the main script:
```
python fish_weight_regression.py
```

4. View the visualizations and printed MSE results in the console.


The name of the jupyter code comes from a juice that i was drinking during the projet. :)
