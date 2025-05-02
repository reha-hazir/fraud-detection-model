# 💳 Credit Card Fraud Detection

👉 **[View full results (HTML)](https://reha-hazir.github.io/fraud-detection-model/main.html)**

## 📝 Overview

Credit card fraud is one of the most prevalent forms of identity theft, causing billions in losses globally. This project aims to build a machine learning model to detect fraudulent credit card transactions using real-world transactional features.

- 💡 **Problem Type**: Binary Classification  
- 📊 **Target Variable**: `fraud` (1 = Fraud, 0 = Not Fraud)  
- 📁 **Dataset**: [Kaggle - Credit Card Fraud Dataset](https://www.kaggle.com/datasets/dhanushnarayananr/credit-card-fraud)

---

## 📌 Problem Statement

In 2019 alone, Germany saw losses of €91 million due to credit card fraud. Globally, this number reached $24.2 billion. The goal is to proactively detect fraudulent activity using machine learning to improve security, reduce company losses, and increase user trust.

---

## 🔍 Feature Descriptions

| Feature                         | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| `distance_from_home`             | Distance from user's home to transaction location                          |
| `distance_from_last_transaction`| Distance from the previous transaction                                     |
| `ratio_to_median_purchase_price`| Ratio of transaction amount to median purchase price                        |
| `repeat_retailer`                | Whether the transaction is from a repeated retailer                        |
| `used_chip`                      | Whether the card chip was used                                             |
| `used_pin_number`                | Whether a PIN number was used                                              |
| `online_order`                   | Whether the transaction was an online order                                |
| `fraud`                          | Label indicating if the transaction was fraudulent                         |

---

## 🧪 Data Exploration

- 📊 Checked for missing values, duplicates, and class imbalance  
- 🔄 Dataset is highly imbalanced (fraudulent transactions are rare)  
- 📈 Chose appropriate metrics (Precision, Recall, F1-Score) over Accuracy due to imbalance  
- 🔍 Performed correlation analysis and visualized feature importance  

---

## ⚙️ Data Preprocessing

- ✅ Cleaned missing and duplicate data  
- 📉 Applied **SMOTE** oversampling to handle class imbalance  
- 🔀 Split data into train/test sets  
- 🧼 Standardized features for models that require scaling  

---

## 🤖 Model Training & Evaluation

- 🧠 Trained **Decision Tree** and **Logistic Regression** classifiers  
- 🔍 Tuned hyperparameters using **GridSearchCV**  
- 📊 Evaluated with classification report and confusion matrix  
- 🔎 Analyzed feature importance for interpretability

### 🔑 Key Findings:
- **Top features** for fraud detection: `ratio_to_median_purchase_price`, `distance_from_home`, `online_order`
- **Decision Tree** performed better due to robustness against noise and outliers

---

## ✅ Conclusion

- 📈 **Decision Tree Classifier** outperformed Logistic Regression in all key metrics  
- ⚡ Fast inference time suitable for real-time fraud detection  
- 🧠 Simple yet effective approach without complex tuning

---

## 🧭 Recommendations

- Ensure high-quality and up-to-date training data  
- Regularly retrain the model with new transactions  
- Keep models and features secure to avoid exploitation  
- Continuously evaluate against new state-of-the-art methods  

---

## 📚 References

- [1] [Machine Learning Mastery - Feature Importance](https://machinelearningmastery.com/calculate-feature-importance-with-python/)

---

👉 **[View full results (HTML)](https://reha-hazir.github.io/fraud-detection-model/main.html)**
