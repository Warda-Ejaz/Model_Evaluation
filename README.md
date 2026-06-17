PROJECT DAY 3 TASK - MODEL EVALUATION

1. Project Overview
This project demonstrates the evaluation of a Regression model using the California Housing dataset from `sklearn.datasets`.  
The task was completed as part of "Project Day 3" requirements which focus on model performance metrics.

Task Requirements Covered:
1. Accuracy Score
2. Mean Absolute Error (MAE)
3. Mean Squared Error (MSE)  
4. R² Score
5. Results displayed in a clear, professional format

2. Dataset Used
Dataset Name: California Housing  
Source: `sklearn.datasets.fetch_california_housing`  
Type: Regression
Description: Predicts the median house value in California districts based on 8 features like income, house age, population, etc.  
Size: 20,640 samples, 8 features  
Target: `MedHouseVal` - Median house value in $100,000 USD

4. Model Used
Algorithm: Ridge Regression  
Library: `sklearn.linear_model.Ridge`  
Parameters: `alpha=1.0, random_state=42`  
Reason: Ridge regression prevents overfitting and gives stable results on this dataset.

5. Methodology
1. Data Loading: Dataset loaded directly from sklearn - no external CSV needed.
2. Train-Test Split: 80% training, 20% testing with `random_state=42` for reproducibility.
3. Model Training: Ridge Regression trained on training set.
4. Prediction: Model predictions generated on test set `X_test`.
5. Evaluation: 4 metrics calculated and displayed in tabular format.

Note on Accuracy Score:  
Since this is a regression task, direct accuracy is not applicable. Accuracy is calculated by converting the continuous target into binary classes using median threshold. Values > median = Class 1, Values ≤ median = Class 0. This approach satisfies the task guideline.

5. Results
Results obtained after running the code:

PROJECT DAY 3 TASK - MODEL EVALUATION

1. Accuracy Score : 82.34%
2. Mean Absolute Error MAE : 0.5331
3. Mean Squared Error MSE : 0.5559
4. R² Score : 0.5758

Clear Results Table for Submission:
Metric          Value
Accuracy Score 82.34%
           MAE 0.5331
           MSE 0.5559
      R² Score 0.5758

Interpretation:
- R² = 0.5758: Model explains ~57.6% variance in house prices. Good baseline for this dataset.
- MAE = 0.5331: On average, prediction error is $53,310.
- MSE = 0.5559: Squared error is low, means no large outliers in error.

6. How to Run
1. Make sure you have Python 3.8+ installed
2. Install required libraries:
   ```bash
   pip install scikit-learn pandas numpy
3. Run the Jupyter Notebook cell or Python file
4. First run will download ∼10MB dataset automatically

7. Files in this Project
Day3_Model_Evaluation.ipynb  - Main Jupyter notebook with complete code
README.md                    - This documentation file
8. Conclusion
All 4 evaluation metrics required for Day 3 Task have been calculated and displayed in a clear, formatted table. The Ridge Regression model performs reasonably well on California Housing dataset and can be further improved with feature engineering or advanced models like RandomForest.

---
Submitted by: Warda Ejaz  
Date: 17-June-2026 
Project Day 3 - Model Evaluation
