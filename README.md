

# 💳 Credit Card Fraud Detection

Credit card fraud is a **growing global problem**, costing billions of dollars every year.  
From the bank’s perspective, **every fraud is a direct financial loss**, while for customers, it can mean **loss of savings, identity theft, and emotional distress**.  

This project applies **machine learning techniques** to detect fraudulent credit card transactions in real-time, helping financial institutions minimize risk and protect customers.

---

## 📌 Problem Statement
The aim of this project is to **predict fraudulent transactions** based on transaction features and patterns.  
Given a set of historical transactions labeled as **fraud** or **legitimate**, the goal is to build a model that can accurately identify potential fraud cases.

---

## 📂 Dataset
The dataset contains anonymized credit card transactions with numerical features derived from PCA for confidentiality.  
- **Classes:**  
  - `0` → Legitimate transaction  
  - `1` → Fraudulent transaction  
- **Challenge:** Highly imbalanced data (fraud cases are rare compared to legitimate transactions).

---

## 🛠 Methodology
The project follows a **structured machine learning pipeline**:

1. **Data Exploration & Visualization**
   - Class distribution check (imbalance analysis)
   - Correlation heatmap & feature analysis

2. **Data Preprocessing**
   - Handling missing values (if any)
   - Feature scaling using standardization
   - Handling class imbalance (e.g., SMOTE or undersampling)

3. **Model Training**
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier
   - XGBoost Classifier
   - Support Vector Classifier (SVC)

4. **Model Evaluation**
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - ROC-AUC Curve

5. **Model Comparison**
   - Selection of the best-performing algorithm for fraud detection.

---

## ⚙️ Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/fraud-detection.git
   cd fraud-detection
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   ```bash
   jupyter notebook "Fraud Detection.ipynb"
   ```

---

## 📊 Results
| Model               | Accuracy | Precision | Recall | F1 Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 0.9993   | 0.9999    | 0.6591 | 0.7688   |
| Decision Tree       | 0.9558   | 0.9899    | 0.9217 | 0.9542   |
| Random Forest       | 0.9756   | 0.9758    | 0.8646 | 0.9168   |
| SVC                 | 0.9644   | 0.9645    | 0.8854 | 0.9233   |
| XGBoost             | 0.9516   | 0.9774    | 0.9258 | 0.9504   |

---

## 📌 Key Insights
- **Recall** is a critical metric here — false negatives (missed frauds) are more costly than false positives.
- **Ensemble methods** like Random Forest and XGBoost often outperform single models in fraud detection.
- **Data imbalance handling** significantly improves model performance.

---

## 📜 License
This project is licensed under the MIT License — you are free to use, modify, and distribute it.

---

