# 🛍️ Customer Purchase Prediction using Decision Tree

This project builds a **Decision Tree Classifier** to predict whether a customer will purchase a product or service based on demographic and behavioral attributes from a banking dataset.

---

## 🎯 Objective

To develop a predictive model that identifies customers likely to respond positively to a marketing campaign. This helps businesses focus efforts on the most promising leads, improving campaign efficiency.

---

## 🧹 Process Overview

- Data Cleaning and Preprocessing  
- Encoding Categorical Features  
- Splitting into Training and Test Sets  
- Training a Decision Tree Classifier  
- Model Evaluation  
- Visualization and Key Insights

---

## 🔍 Key Findings

- ✅ The model achieved an **accuracy of 87.18%** on the test dataset.
- 📊 It performs very well at predicting customers who will **not** purchase.
- ⚠️ It struggles to accurately predict **buyers**, due to **class imbalance** in the data.

### 📈 Classification Report

| Class        | Precision | Recall | F1-score | Support |
|--------------|-----------|--------|----------|---------|
| No Purchase  | 0.93      | 0.92   | 0.93     | 807     |
| Yes Purchase | 0.42      | 0.47   | 0.44     | 98      |

---

### 🔁 Confusion Matrix

- 🟩 **743** customers correctly predicted as non-buyers
- 🟩 **46** correctly predicted as buyers
- ❌ **52** buyers missed (false negatives)
- ❌ **64** non-buyers incorrectly predicted as buyers

---

## 🧠 Summary

The model was built to **predict whether a customer will purchase a product or service** (`yes` or `no`) based on their demographic and behavioral attributes.

- The prediction target is the **`y` column**, which indicates if a customer subscribed to the product.
- The model performed well overall (87% accuracy), especially at predicting customers who would **not purchase**,helping reduce marketing costs.
- However, performance for **predicting actual buyers** was weaker due to the imbalance in the dataset.
- To improve results:
  - Apply resampling techniques like **SMOTE**
  - Try ensemble models such as **Random Forest** or **XGBoost**
  - Optimize using hyperparameter tuning or feature selection

---

## 🛠️ Technologies Used

- Python  
- pandas  
- scikit-learn  
- seaborn & matplotlib  

---

## 📁 Files

- `BankData.csv` – Input dataset  
- `decision_tree_model.py` – Code for training and testing the model  
- `confusion_matrix.png` – Heatmap of prediction results  
- `README.md` – Project summary and key findings

---

## 📚 Dataset Source

- **Bank Marketing Dataset** from a Portuguese bank  
- Related to direct marketing campaigns (phone calls)  
- **Goal**: Predict if a client will subscribe to a term deposit (`y`)  
- **Donated on**: 13 Feb 2012


---

Feel free to explore or improve the model further!






