# Customer Churn Classification Project

## Overview
This project uses machine learning to predict whether a customer will churn (leave a service). It compares five classification algorithms and evaluates their performance using several metrics.

## Algorithms
- Logistic Regression
- Decision Tree
- Random Forest
- Linear Support Vector Machine (SVM)
- XGBoost

## Dataset
The project uses `training.csv` and `testing.csv`, which contain customer information such as age, tenure, usage frequency, support calls, payment delays, subscription type, contract length, and total spend.

The target variable is `Churn`:
- `0` = Customer does not churn
- `1` = Customer churns

## Data Preprocessing
- Handle missing values
- Encode categorical features using One-Hot Encoding
- Scale numerical features when needed
- Remove `CustomerID` from the model features
- Split the data into training, validation, and holdout sets

## Evaluation Metrics
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

The best model is selected based on validation F1-score. Classification threshold tuning is also used to explore the balance between precision and recall.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- Jupyter Notebook

## How to Run
1. Clone or download this project.
2. Place `training.csv` and `testing.csv` in the same folder as the notebook.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost
   ```

4. Open `Customer_Churn_Improved_Classification.ipynb` in Jupyter Notebook or VS Code.
5. Run the notebook cells from top to bottom.

## Results
The notebook compares all five algorithms, displays their validation metrics, and evaluates the selected model on a separate holdout set. It also generates a confusion matrix and saves model comparison results and predictions as CSV files.

Actual performance metrics depend on the dataset and model configuration.

## Future Improvements
- Perform hyperparameter tuning with cross-validation.
- Investigate feature importance.
- Improve model performance through feature engineering.
- Evaluate on a verified, independent test dataset.
