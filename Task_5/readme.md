
# 💳 Credit Card Fraud Detection  
### CodSoft Data Science Internship — Task 5  

This project focuses on detecting fraudulent credit card transactions using machine learning techniques.

---

## 📌 Objective  
The goal is to identify fraudulent transactions by analyzing patterns in credit card data. Fraud detection is challenging due to *high class imbalance, so techniques like **SMOTE oversampling* are used.

---

## 📂 Dataset  
- Total rows: 284,807  
- Features: Numerical (V1–V28) + Time + Amount  
- Target:
  - *0 → Genuine*
  - *1 → Fraud*

Because the dataset is very large, a *30,000-row sample* was used for efficient processing.

---

## ⚙ Steps Performed  

### ⿡ Load & Explore Data  
- Checked shape, missing values (none found), and class distribution  
- Identified strong imbalance (~99.8% genuine, ~0.2% fraud)

### ⿢ Feature Selection  
- *X = All features except "Class"*  
- *y = Class*

### ⿣ Data Scaling  
- Standardized numerical features using StandardScaler

### ⿤ Handle Imbalance  
- Applied *SMOTE* to balance classes  
- Fraud = Genuine (same count after oversampling)

### ⿥ Model Building  
- Used *Random Forest Classifier*  
- Trained on balanced SMOTE dataset

### ⿦ Model Evaluation  
- Classification Report  
- Confusion Matrix  

---

## 📊 Results  
- *Accuracy:* Excellent  
- *Precision, Recall, F1-score:* Strong for both classes  
- Confusion matrix shows accurate detection of both genuine and fraudulent transactions.

---

## 📝 Conclusion  
The Random Forest model successfully detected fraudulent credit card transactions after handling class imbalance.  
By using scaling + SMOTE + ensemble learning, the model achieved strong performance and can help in real-world fraud prevention systems.

---

## 🛠 Technologies Used  
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Imbalanced-learn  
- Random Forest Algorithm  

---

## 📎 Internship  
This project is part of the *CodSoft Data Science Internship*.
