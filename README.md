# Machine Learning Model – Student Performance Prediction

##  Objective

The objective of this project is to build a **machine learning regression model** to predict student **Exam Scores** based on various input features and evaluate its performance using standard metrics.

---

## Dataset

* **Name:** Student Performance Factors Dataset
* **Target Variable:** `Exam_Score`
* The dataset contains various features related to student study patterns and performance.
* From Kaggle

---

##  Approach

### 1. Data Preprocessing

* Checked and handled missing values:

  * Numerical columns → filled using **median**
  * Categorical columns → filled using **mode**
* Converted categorical variables into numeric using **one-hot encoding (`pd.get_dummies`)**
* Ensured dataset is clean and ready for modeling

---

### 2. Feature Selection

* **Features (X):** All columns except `Exam_Score`
* **Target (y):** `Exam_Score`

---

### 3. Train-Test Split

* Dataset split into:

  * **80% Training Data**
  * **20% Testing Data**
* Used `train_test_split` from sklearn

---

### 4. Models Implemented

The following regression models were trained and evaluated:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

---

### 5. Model Evaluation

Models were evaluated using:

* **RMSE (Root Mean Squared Error)**
* **MAE (Mean Absolute Error)**
* **R² Score (Coefficient of Determination)**

---

##  Results

| Model             | RMSE   | MAE    | R² Score |
| ----------------- | ------ | ------ | -------- |
| Linear Regression | 1.8046 | 0.4503 | 0.7696   |
| Random Forest     | 2.2381 | 1.1817 | 0.6456   |
| Decision Tree     | 4.0365 | 1.9592 | -0.1527  |

---

##  Best Model

* **Selected Model:** Linear Regression
* **Reason:**

  * Lowest RMSE (1.8046)
  * Lowest MAE (0.4503)
  * Highest R² score (0.7696)
  * Better generalization compared to other models

---

##  Visualization

A scatter plot of **Actual vs Predicted values** was used to evaluate performance:

* Most points lie near the diagonal → indicates good predictions
* Some deviation at higher values → indicates minor prediction error

---

##  Conclusion

* Successfully built a **working machine learning model**
* Linear Regression outperformed other models for this dataset
* Decision Tree showed poor performance (negative R²), indicating overfitting
* The model can effectively predict student exam scores with good accuracy

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

##  Output

✔ Working ML model
✔ Model evaluation with metrics
✔ Model comparison
✔ Final model selection
✔ Visualization of predictions

---
