# Loan Risk Classification using Logistic Regression

## 📌 Overview
This project builds a **Logistic Regression Model** to classify loan applications as either:
- **0 (Healthy Loan)** – Low risk
- **1 (High-Risk Loan)** – Potential default risk

The model is trained and evaluated using **lending data**, ensuring accurate predictions.

## 📂 Dataset
The dataset contains the following features:
- `loan_size`: Amount of the loan
- `interest_rate`: Interest rate assigned
- `borrower_income`: Borrower's annual income
- `debt_to_income`: Debt-to-income ratio
- `num_of_accounts`: Number of accounts held
- `derogatory_marks`: Negative credit marks
- `total_debt`: Total outstanding debt
- `loan_status` (Target Variable): **0 = Healthy Loan, 1 = High-Risk Loan**

## ⚙️ Technologies Used
- **Python** 🐍
- **Pandas** for data manipulation
- **NumPy** for numerical operations
- **Scikit-Learn (sklearn)** for machine learning

## 🔍 Model Development
1. **Data Preprocessing**
   - Loaded data using `pandas`
   - Separated features (`X`) and target labels (`y`)
   - Split data into **training (80%)** and **testing (20%)**

2. **Model Training**
   - Used **Logistic Regression** from `sklearn.linear_model`
   - Fit the model with training data (`X_train`, `y_train`)

3. **Predictions & Evaluation**
   - Made predictions on test data (`X_test`)
   - Evaluated using:
     - **Confusion Matrix**
     - **Classification Report** (Precision, Recall, F1-score)

## 📊 Model Performance
| Metric  | Healthy Loan (0) | High-Risk Loan (1) |
|---------|------------------|--------------------|
| **Precision** | 1.00 | 0.86 |
| **Recall** | 0.99 | 0.94 |
| **F1-Score** | 1.00 | 0.90 |
| **Accuracy** | **99%** |

✅ **The model performs exceptionally well, especially in identifying healthy loans.**  
⚠️ **Some high-risk loans are misclassified as healthy (~31 cases).**  

## 🚀 Future Improvements
- **Optimize Class Imbalance**: Use **SMOTE** to balance high-risk loans.
- **Adjust Decision Threshold**: Improve recall for high-risk loans.
- **Try Advanced Models**: Random Forest or Neural Networks for better accuracy.

## 📌 How to Run the Code
1. Clone this repository:
   ```bash
   git clone https://github.com/Neda2020/loan-risk-classification.git
   cd credit-risk-classification
2.	Install dependencies:
bash
CopyEdit
pip install -r requirements.txt
3.	Run the script:
bash
CopyEdit
python credit_classification.py
📜 License
This project is open-source and available under the MIT License.


