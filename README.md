# Employee Data Analysis and Modeling

This project provides a complete end-to-end analysis of an employee dataset using Python. The code performs:

- **Data Cleaning and Preprocessing:**  
  Removing unnecessary columns, handling missing values, and preparing numerical and categorical features for modeling.

- **Exploratory Data Analysis (EDA):**  
  - **Univariate Analysis:** Histograms, boxplots, and summary statistics for numerical features.  
  - **Categorical Analysis:** Countplots and frequency tables for categorical features.  
  - **Multivariate Analysis:** Comparing features with the target variable (`Attrition`) using boxplots and stacked bar plots.

- **Hypothesis Testing:**  
  - **T-Test:** Comparing the mean `TotalWorkingYears` between employees with and without attrition using Welch's t-test.  
  - **ANOVA:** Checking if there are significant age differences across departments (when exactly three departments exist).

- **Classification Modeling:**  
  The target variable is `Attrition` (whether an employee left or stayed).  
  Models used include:  
  - Logistic Regression  
  - Decision Tree Classifier  
  - XGBoost Classifier  
  Each model is tuned using GridSearchCV and evaluated using accuracy and classification reports.

- **Regression Modeling:**  
  The regression task predicts `MonthlyIncome`. Two models are compared:  
  - Polynomial Regression (Linear Regression with Polynomial Features)  
  - XGBoost Regressor  
  Model performance is evaluated using R², MSE, RMSE, MAE, and MAPE.

- **Clustering:**  
  KMeans clustering is performed on the dataset (excluding `Attrition` and `MonthlyIncome`) after preprocessing.  
  The code uses the Elbow Method and Silhouette Score to determine the optimal number of clusters.  
  Finally, the resulting cluster labels are added to the dataset.

## How to Run

1. **Upload Dataset:**  
   Run the code in a Google Colab notebook (or similar environment). When prompted, upload the `employee.csv` file.

2. **Install Dependencies:**  
   The script installs any necessary packages (like `scipy`) automatically.

3. **Execute the Notebook:**  
   The notebook is divided into sections covering data loading, EDA, hypothesis testing, classification, regression, and clustering.  
   Simply run all cells to reproduce the analysis and model tuning.

## Contact

For any questions or further information, please contact:  
**donny.landscape@gmail.com**
