# 💳 Credit Card Fraud Detection System

This project focuses on detecting **fraudulent credit card transactions** using **Machine Learning** techniques.  
It addresses the major real-world challenge of **highly imbalanced data** and builds reliable models that prioritize **fraud detection (recall)** over misleading accuracy.

---

![Credit_card_fraud_detection](banner.jpg)

## 📌 Project Overview

- **Problem Type:** Binary Classification  
- **Dataset:** Credit Card Transactions (Kaggle dataset)
- **Goal:** Identify whether a transaction is **Fraudulent (1)** or **Legitimate (0)**
- **Main Challenge:** Extreme class imbalance (Fraud ≈ 0.17%)

> In real banking systems, missing a fraud is more costly than flagging a genuine transaction.

---

## 🧠 Machine Learning Approach

### ✔ Key Steps Followed
1. Data loading and inspection  
2. Handling highly imbalanced data  
3. Exploratory Data Analysis (EDA)  
4. Model training and evaluation  
5. Probability (score-based) fraud prediction  

---

## 📊 Dataset Description

| Feature | Description |
|-------|-------------|
| `Time` | Seconds elapsed between transactions |
| `V1`–`V28` | PCA-transformed numerical features |
| `Amount` | Transaction amount |
| `Class` | Target variable (0 = Legit, 1 = Fraud) |

- Total transactions: **284,807**
- Fraud transactions: **492**
- Legit transactions: **284,315**

---

## ⚖️ Handling Imbalanced Data

This dataset is **highly imbalanced**, so:
- Accuracy alone is **misleading**
- Focus is placed on:
  - **Recall**
  - **Precision**
  - **F1-score**

### Technique Used:
- **Under-sampling** (for learning & experimentation)
- Balanced dataset for fair model training

---

## 🤖 Models Used

### 1️⃣ Logistic Regression
- Strong baseline model
- Works well with PCA features
- Low risk of overfitting
- Easy to interpret

### 2️⃣ XGBoost (Advanced Model)
- Handles non-linear patterns
- Learns complex fraud signatures
- Industry-standard for fraud detection
- Provides **fraud probability scores**

---

## 📈 Model Evaluation Metrics

- Accuracy  
- Precision  
- Recall (most important)  
- F1-score  

📌 **Recall is prioritized** because missing a fraud is costlier than a false alarm.

---

## 📉 Visual Analysis

The project includes:
- Class distribution plots
- Transaction amount distribution
- Line graphs comparing:
  - Train vs Test performance
  - Logistic Regression vs XGBoost
- Fraud probability (score) line plots

---



## 🛠️ Tools & Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- XGBoost  
- Jupyter Lab  

---

## 🚀 Future Improvements

- Deploy model using **FastAPI**
- Add **Streamlit dashboard**
- Use **class-weighted learning instead of under-sampling**
- Monitor fraud prediction thresholds dynamically

---

## 📌 Conclusion

This project demonstrates how to:
- Work with real-world imbalanced data
- Build robust fraud detection models
- Use probability-based predictions instead of only labels
- Evaluate models correctly using appropriate metrics

---

## 👤 Author

**M. Abhilash**  
Computer Science Engineering Student  
Interested in Machine Learning & Real-World Problem Solving

---

⭐ If you like this project, consider giving it a star!
