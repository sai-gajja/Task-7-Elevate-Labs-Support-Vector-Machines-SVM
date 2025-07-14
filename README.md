🧠 Breast Cancer Classification with SVM

This project applies Support Vector Machines (SVM) to the Breast Cancer Dataset by Yasser H. from Kaggle. It demonstrates binary classification (Benign vs Malignant) using both linear and RBF kernels, with dimensionality reduction and hyperparameter tuning.

📌 Project Goals
Load and preprocess the Kaggle dataset

Encode target labels (Benign/Malignant) using LabelEncoder

Split data into train/test sets

Train SVM models with linear and RBF kernels

Visualize 2D decision boundaries using PCA

Tune C and gamma via GridSearchCV

Evaluate performance with cross-validation

Report accuracy, precision, recall, F1-score, and confusion matrices

📥 Dataset
Source: Kaggle – Yasser H.’s Breast Cancer Dataset
🗓 Published December 29, 2021, with 32 feature columns describing tumor characteristics and binary diagnosis (Benign/Malignant) 
arxiv.org
+11
github.com
+11
kaggle.com
+11
github.com
github.com
.

🛠️ Technologies Used
Python

NumPy / Pandas for data handling

Scikit-learn for SVM, encoding, scaling, PCA, grid search, CV, metrics

Matplotlib / Seaborn for visualization

🔁 Workflow Summary
Import libraries

Load data: pd.read_csv('breast-cancer-dataset.csv')

Encode diagnosis column (B → 0, M → 1)

Split features (X) and target (y), then train/test split

Standardize features with StandardScaler

Train SVMs: kernel='linear' and kernel='rbf'

Evaluate with confusion matrix, classification report, and accuracy

Visualize decision boundary after reducing to 2D via PCA

Tune hyperparameters (C, gamma) with GridSearchCV (5‑fold)

Confirm model performance using cross_val_score

🧮 Sample Results (Linear vs RBF)
Linear SVM:

Accuracy ≈ 95.6%

High recall for benign tumors

RBF SVM:

Accuracy ≈ 94.7%

Slightly higher precision, but marginally lower recall

Tuned RBF (best params: C=10, gamma=0.0001):

Cross‑validation accuracy ≈ 94.7% 
