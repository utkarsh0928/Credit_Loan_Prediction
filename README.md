# 🏦 Credit Risk Prediction System

A Machine Learning solution designed to automate the loan eligibility process. It analyzes customer demographics and financial history to predict whether a loan application should be **Approved** or **Rejected**.

### 📊 Project Overview

- **Goal:** Minimize financial risk for banks by accurately identifying potential defaulters.
- **Algorithm:** Random Forest Classifier (chosen for its high accuracy on non-linear data).
- **Accuracy:** Achieved **82%** accuracy on the test dataset.
- **Techniques:** Data Cleaning (Pandas), Feature Engineering, One-Hot Encoding, Model Serialization.

### 🛠️ Tech Stack

- **Language:** Python 3.9+
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
- **Serialization:** Joblib (for model persistence)

### 📂 Dataset

The model was trained on a dataset containing the following key features:

- `Gender`, `Marital Status`, `Dependents`
- `ApplicantIncome`, `CoapplicantIncome`, `LoanAmount`
- `Credit_History` (Key indicator), `Property_Area`

### 🚀 How to Run

1.  **Clone the repository**

    ```bash
    git clone [https://github.com/utkarsahil/Credit-Loan-Prediction.git](https://github.com/utkarsahil/Credit-Loan-Prediction.git)
    cd Credit-Loan-Prediction
    ```

2.  **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Train the Model**
    Run the training script to process data and generate the `.pkl` file:

    ```bash
    python train_model.py
    ```

    _Output:_ `Model saved to loan_predictor_model.pkl`

4.  **Test Predictions**
    Run the prediction script to see the model in action:
    ```bash
    python predict.py
    ```

### 📈 Results & Visualizations

- **Confusion Matrix:** Shows false positives vs false negatives.
- **Feature Importance:** Identified `Credit_History` and `ApplicantIncome` as the top factors influencing approval.

### 🔮 Future Scope

- Deploy the model as a REST API using **Django/FastAPI**.
- Implement a frontend dashboard for bank officers to input details manually.
