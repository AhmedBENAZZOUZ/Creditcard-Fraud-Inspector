# 💳 Credit Card Fraud Detection with Machine Learning

This project applies machine learning techniques to detect fraudulent transactions in credit card data, following the **CRISP-DM** methodology. The objective is to build a predictive system that can effectively distinguish between genuine and fraudulent transactions, despite the strong class imbalance.

---

## 📁 Dataset

The dataset used is publicly available on [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud) and contains **284,807** transactions, of which only **0.17% are frauds**.

---

## 📌 Project Structure

This notebook is structured using the **CRISP-DM** data science methodology:

1. **Business Understanding**  
   - Goal: Detect fraudulent transactions to reduce financial loss.

2. **Data Understanding**  
   - Explore distributions, visualize fraud vs. non-fraud transactions.
   - Analyze correlations and identify key trends.

3. **Data Preparation**  
   - Normalize features, handle class imbalance with **SMOTE**.
   - Apply **PCA** for dimensionality reduction.

4. **Modeling**  
   - Models used: Logistic Regression, LDA, SVM, Random Forest.
   - Hyperparameter tuning and ensemble techniques.

5. **Evaluation**  
   - Metrics: Precision, Recall, F1-score, ROC-AUC.
   - Visuals: Confusion Matrix, ROC Curve, Feature Importance.

6. **Deployment/Conclusion**  
   - Random Forest offered the best recall.
   - Future work: Model explainability (e.g., SHAP), real-time detection pipeline.

---

## 📊 Key Results

| Model               | Precision | Recall | F1-Score | ROC AUC |
|--------------------|-----------|--------|----------|---------|
| Logistic Regression| 0.89      | 0.62   | 0.73     | 0.96    |
| SVM (RBF Kernel)   | 0.90      | 0.68   | 0.77     | 0.97    |
| Random Forest      | **0.94**  | **0.82** | **0.87** | **0.99** |

> ⚠️ Class imbalance was addressed with **SMOTE**, improving recall significantly.

---

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/fraud-detection-system.git
   cd fraud-detection-system
