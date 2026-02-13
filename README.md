# 📌 Task 16: Hyperparameter Tuning using GridSearchCV

## 🧠 Objective
The objective of this task is to improve machine learning model performance using Hyperparameter Tuning with GridSearchCV and compare tuned model performance with default models.

Dataset used: Breast Cancer Dataset

---

## 🛠 Tools & Technologies
Python  
Pandas  
Scikit-learn  
GridSearchCV  
Jupyter Notebook / Google Colab  

---

## 📂 Workflow

### 1. Load Dataset & Preprocessing
- Loaded dataset using Pandas  
- Removed unnecessary column: id  
- Converted target column diagnosis  
  - M → 1  
  - B → 0  
- Applied StandardScaler for feature scaling  

---

### 2. Train-Test Split
Dataset split into:
80% Training  
20% Testing  

Train shape: (455, 30)  
Test shape: (114, 30)  

---

### 3. Models Used
Support Vector Machine (SVM)  
Random Forest Classifier  

---

## Default Model Performance

Model | Accuracy  
SVM | 97.36%  
Random Forest | 96.49%  

---

## Hyperparameter Tuning using GridSearchCV
GridSearchCV applied with 5-fold cross validation.

### SVM Parameter Grid
C: [0.1, 1, 10]  
kernel: linear, rbf  

### Random Forest Parameter Grid
n_estimators: 100, 200  
max_depth: None, 5, 10  

---

## Best Parameters Found

Best SVM Parameters  
C = 0.1  
kernel = linear  

Best Random Forest Parameters  
n_estimators = 200  
max_depth = None  

---

## Tuned Model Performance

Model | Default Accuracy | Tuned Accuracy  
SVM | 97.36% | 98.24%  
Random Forest | 96.49% | 96.49%  

Best Model: Tuned SVM

---

## Classification Report (Tuned SVM)
Accuracy: 98%  
Precision: 99%  
Recall: 98%  
F1-score: 98%  

---

## Project Structure
Task16-GridSearchCV  
breast-cancer.csv  
GridSearchCV.ipynb  
README.md  

---

## Conclusion
Hyperparameter tuning improves model performance.  
GridSearchCV helps find best parameters automatically.  
Tuned SVM achieved highest accuracy.  
Model performance improved after optimization.  

