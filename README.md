🫀 Heart Disease Classification using KNN and PCA
📌 Project Overview

This project focuses on predicting the presence of heart disease in patients using clinical attributes.
A K-Nearest Neighbors (KNN) classifier is trained and evaluated both with and without Principal Component Analysis (PCA) to study the impact of dimensionality reduction on model performance.

The project demonstrates a complete machine learning workflow, including preprocessing, feature scaling, model training, evaluation, and performance comparison.

📊 Dataset

The dataset contains patient health indicators such as age, cholesterol levels, blood pressure, heart rate, etc.

Target variable:

1 → Presence of heart disease

0 → Absence of heart disease

📁 Dataset location:

data/heart_dataset.csv

⚙️ Technologies & Libraries Used

Python

NumPy

Pandas

Scikit-learn

Jupyter Notebook

🧠 Methodology
1️⃣ Data Preparation

Loaded dataset using Pandas

Separated features (X) and target variable (y)

Performed train–test split (80% training, 20% testing)

2️⃣ Feature Scaling

Applied StandardScaler

Essential for distance-based algorithms like KNN

Prevents features with large values from dominating distance calculations

3️⃣ Model 1: KNN without PCA

Trained KNN classifier on scaled features

Evaluated performance using:

Confusion Matrix

Accuracy Score

4️⃣ Model 2: KNN with PCA

Applied Principal Component Analysis (PCA) to reduce dimensionality

Retained most variance while reducing feature space

Trained KNN on PCA-transformed data

Evaluated performance on test data

📈 Results
Model	Accuracy
KNN (Without PCA)	~67%
KNN (With PCA)	~36%
🔍 Key Insights

Feature scaling significantly impacts KNN performance.

PCA reduced dimensionality but also removed important discriminative information.

PCA is not always beneficial, especially for distance-based classifiers like KNN.

Model selection and preprocessing techniques must align with algorithm behavior.

📁 Repository Structure
heart-disease-classification-knn-pca/
│
├── data/
│   └── heart_dataset.csv
│
├── notebooks/
│   └── heart_disease_classification_using_PCA.ipynb
│
└── README.md

🚀 Future Improvements

Hyperparameter tuning using GridSearchCV

Try alternative classifiers (Logistic Regression, SVM, Random Forest)

Visualize explained variance ratio from PCA

Add ROC-AUC and F1-score evaluation

🧑‍💻 Author

Sandesh Duduskar
Machine Learning & Data Science Enthusiast
