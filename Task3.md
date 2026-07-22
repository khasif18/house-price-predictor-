# **ARTIFICIAL INTELLIGENCE & MACHINE LEARNING INTERNSHIP**

## **Task 3: Model Validation, Overfitting Control & Hyperparameter Tuning**

### **Submitted By**

**Name:** Khasif Khamar

**Internship:** Artificial Intelligence & Machine Learning

**Task:** Task 3

**Date:** 22/07/2026

---

# **1. Objective**

The objective of this task is to understand and implement machine learning model validation techniques, reduce overfitting, and improve model performance through hyperparameter tuning. The project demonstrates the complete workflow of training, validating, optimizing, and comparing regression models using the California Housing dataset.

---

# **2. Introduction**

Machine Learning models often perform well on training data but may fail to generalize to unseen data due to overfitting. Therefore, proper model validation and hyperparameter optimization are essential before deploying any machine learning model.

In this project, a Linear Regression model was first used as the baseline model. Later, a Decision Tree Regressor was optimized using GridSearchCV to improve prediction performance while reducing overfitting. Model performance was evaluated using Cross Validation, Root Mean Squared Error (RMSE), and R² Score.

---

# **3. Dataset Description**

The California Housing dataset available in the Scikit-learn library was used for this task.

The dataset contains information related to housing prices in California and includes features such as:

* Median Income
* House Age
* Average Rooms
* Average Bedrooms
* Population
* Average Occupancy
* Latitude
* Longitude

The target variable is the **Median House Value**, which is predicted using regression algorithms.

---

# **4. Tools and Technologies Used**

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook / Python IDE

---

# **5. Methodology**

### Step 1: Data Loading

The California Housing dataset was imported using the Scikit-learn dataset module. The feature variables and target variable were separated for training and testing.

### Step 2: Data Splitting

The dataset was divided into training and testing datasets using the Train-Test Split method.

* Training Data: 80%
* Testing Data: 20%

This ensures that the model is evaluated on unseen data.

### Step 3: Linear Regression Model

A Linear Regression model was trained using the training dataset.

The model was evaluated using:

* Root Mean Squared Error (RMSE)
* R² Score

This model served as the baseline for comparison.

### Step 4: Cross Validation

Five-Fold Cross Validation was performed using the `cross_val_score()` function.

Cross-validation repeatedly divides the training dataset into different subsets and evaluates the model multiple times.

This provides a more reliable estimate of model performance and helps detect overfitting.

The average cross-validation score and standard deviation were calculated to measure model stability.

### Step 5: Hyperparameter Tuning

A Decision Tree Regressor was used for hyperparameter tuning.

GridSearchCV was applied to automatically search for the best combination of parameters including:

* max_depth
* min_samples_split
* min_samples_leaf

The best parameter combination was selected based on the highest cross-validation score.

### Step 6: Model Evaluation

The optimized Decision Tree model was tested using the testing dataset.

Performance metrics calculated include:

* RMSE
* R² Score

Finally, the tuned Decision Tree model was compared with the baseline Linear Regression model.

---

# **6. Overfitting Control**

Overfitting occurs when a model learns the training data too well, including noise and unnecessary patterns, resulting in poor performance on unseen data.

To reduce overfitting, Decision Tree hyperparameters were optimized using GridSearchCV.

The following parameters were tuned:

* Maximum depth of the tree
* Minimum samples required to split a node
* Minimum samples required at each leaf node

These parameters prevent excessive tree growth and improve model generalization.

---

# **7. Performance Metrics**

## Root Mean Squared Error (RMSE)

RMSE measures the average prediction error made by the regression model.

A lower RMSE indicates better prediction accuracy.

---

## R² Score

R² Score measures how well the model explains the variance in the target variable.

Its value ranges between 0 and 1.

A value closer to 1 indicates better prediction performance.

---

# **8. Model Comparison**

Two regression models were compared in this project:

* Linear Regression
* Decision Tree Regressor (Tuned using GridSearchCV)

The comparison was performed using:

* RMSE
* R² Score

The tuned model was selected based on improved prediction performance and better generalization capability.

---

# **9. Results**

The following objectives were successfully achieved:

* Dataset successfully loaded.
* Data preprocessing completed.
* Train-Test Split performed.
* Linear Regression model trained.
* Five-Fold Cross Validation completed.
* Decision Tree Regressor implemented.
* Hyperparameter tuning performed using GridSearchCV.
* Best parameters identified.
* RMSE calculated.
* R² Score calculated.
* Model comparison completed.
* Performance visualized using graphs.

---

# **10. Conclusion**

This task provided practical knowledge of machine learning model validation and optimization techniques.

Cross Validation helped evaluate the consistency of the model across multiple data splits, while GridSearchCV automatically selected the best hyperparameter combination for the Decision Tree Regressor.

The project demonstrated the importance of reducing overfitting and selecting the best-performing model using objective evaluation metrics such as RMSE and R² Score.

Overall, the task improved understanding of regression modeling, model validation, hyperparameter tuning, and performance evaluation using Scikit-learn.

---

# **11. Future Scope**

Future improvements can include:

* Implementing Random Forest Regression
* Using Gradient Boosting algorithms such as XGBoost
* Performing feature engineering
* Using RandomizedSearchCV for faster hyperparameter optimization
* Comparing additional regression models

---

# **12. References**

1. Scikit-learn Documentation – https://scikit-learn.org/
2. Python Documentation – https://docs.python.org/3/
3. NumPy Documentation – https://numpy.org/
4. Pandas Documentation – https://pandas.pydata.org/
5. California Housing Dataset – Scikit-learn
