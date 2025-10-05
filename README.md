# 💳 Fraud Detection with Isolation Forest

This project detects **fraudulent credit card transactions** using **unsupervised anomaly detection** with the `IsolationForest` algorithm from scikit-learn.

---

## 📂 Files
- `Fraud Detection with Anomaly Analysis.py` — Main Python script  
- `creditcards.csv` — Dataset containing transaction data  

---

## ⚙️ How It Works
1. Loads the dataset (`creditcards.csv`)  
2. Uses the `Amount` column to train an `IsolationForest` model  
3. Predicts anomalies (potential frauds)  
4. Compares detected anomalies with actual fraud labels (`Class` column)  
5. Displays a scatter plot highlighting suspicious transactions  

---

## 🧠 Model
- **Algorithm:** Isolation Forest  
- **Contamination rate:** 1% (assumed fraud rate)  
- **Output:** Fraud or non-fraud classification per transaction  

---

## 📊 Visualization
The script generates a scatter plot where fraudulent transactions appear in different colors based on anomaly detection results.

---

## 📁 Output
The script creates a file named **fraud_transactions.xlsx**  
It contains only transactions flagged as frauds (`Anomaly = 1`).  
Each record includes its predicted label and anomaly score.

---

## 📂 Dataset
- **Full dataset:** `creditcards.zip` (stored with Git LFS)
- **Sample preview:** `creditcards_sample.csv` (first 100 rows for quick inspection)

---

📂 [Download Project File](https://github.com/tiagoalves101-ops/Fraud_Detection_with_Anomaly_Analysis/blob/main/creditcards.csv)
---

## 🚀 How to Run
```bash
pip install pandas matplotlib scikit-learn
python "Fraud Detection with Anomaly Analysis.py"




