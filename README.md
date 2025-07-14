# 🧠 Breast Cancer Classification using Support Vector Machines (SVM)

This project applies Support Vector Machines (SVM) for binary classification on the **Breast Cancer Dataset** by Yasser H. from Kaggle. The goal is to differentiate between benign and malignant tumors using linear and RBF kernel SVMs, with visualization and performance evaluation.

---

## 📂 Dataset

**Source:** [Kaggle - Breast Cancer Dataset by Yasser H.](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)  
- **Rows:** 569  
- **Features:** 30 numeric features related to tumor characteristics  
- **Target:** Diagnosis (`M` = Malignant, `B` = Benign)

---

## 🎯 Objectives

- Load and preprocess the dataset
- Train SVM models using linear and RBF kernels
- Visualize decision boundaries using PCA
- Tune hyperparameters using GridSearchCV
- Evaluate models using confusion matrix, classification report, and cross-validation

---

## 🛠️ Technologies Used

- Python 3.x
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 📊 Project Workflow

### 1. Data Preprocessing
- Load dataset using `pandas`
- Encode the target variable (`diagnosis`) using `LabelEncoder`
- Split data into features (`X`) and target (`y`)
- Standardize features using `StandardScaler`
- Split dataset into training and testing sets

### 2. Model Training
- Train **SVM with linear kernel**
- Train **SVM with RBF kernel**

### 3. Model Evaluation
- Confusion Matrix
- Classification Report
- Accuracy Score

### 4. Visualization
- Use **PCA** to reduce data to 2D
- Visualize decision boundaries using `matplotlib` and `seaborn`

### 5. Hyperparameter Tuning
- Perform Grid Search on `C` and `gamma` using `GridSearchCV`
- Use 5-fold cross-validation for robust evaluation

---

## ✅ Results

| Model         | Accuracy |
|---------------|----------|
| Linear SVM    | 95.6%    |
| RBF SVM       | 94.7%    |
| RBF (Tuned)   | 94.7% (CV Average) |

---

## 🧪 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/svm-breast-cancer-classification.git
   cd svm-breast-cancer-classification
