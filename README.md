# 🏦 Bank Marketing Decision Tree Classifier

This project builds a **Decision Tree Classifier** to predict whether a customer will **subscribe (purchase) a term deposit** based on their **demographic** and **behavioral** data.  
The dataset used is the **Bank Marketing Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing).

---

## 📂 Project Structure
```
SCT_DS_3/
│-- bank_marketing_decision_tree.ipynb   # Jupyter/Colab notebook with full code
│-- bank_cleaned.csv                     # Cleaned dataset after preprocessing
│-- README.md                            # Project documentation
```

---

## 🔧 Steps Performed

### 1. Data Cleaning
- Removed rows with `"unknown"` values in critical columns  
- Dropped duplicate records  
- Handled missing values (filled or dropped where necessary)  
- Verified class balance of target variable  

### 2. Exploratory Data Analysis (EDA)
- **Target distribution** (Subscribed vs Not Subscribed)  
- **Categorical feature distributions** (job, marital status, education, etc.)  
- **Numerical feature distributions** (age, balance, duration, etc.)  
- **Correlation heatmap** for numeric variables  
- Visualized **relationships between features & subscription**  

### 3. Model Building
- Converted categorical features using **One-Hot Encoding**  
- Split dataset into **Train/Test (80/20)**  
- Built a **Decision Tree Classifier** using `scikit-learn`  
- Tuned hyperparameters (`max_depth`, `min_samples_split`, etc.)  
- Visualized the **Decision Tree structure**  

### 4. Model Evaluation
- **Accuracy score** on test data  
- **Confusion matrix**  
- **Classification report (Precision, Recall, F1-score)**  
- **ROC Curve & AUC Score**  

---

## 📊 Key Insights
- Certain **jobs** (e.g., management, retired) had higher subscription rates  
- Customers with higher **balance** and longer **call durations** were more likely to subscribe  
- **Marital status & education** also showed trends in purchase behavior  
- Decision Tree revealed the most important features driving predictions  

---

## ▶️ How to Run

1. Clone this repository:
```bash
git clone https://github.com/<vaishuudgirkar-cloud>/SCT_DS_3.git
cd SCT_DS_3
```

2. Install dependencies
```bash
pip install pandas matplotlib seaborn scikit-learn
```

3. Run the notebook:
- Open in **Google Colab** (recommended)  
- OR run locally with **Jupyter Notebook / VS Code**  

---

## 📌 Dataset Source
- [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

---

👩‍💻 Author: *Vaishnavi*
