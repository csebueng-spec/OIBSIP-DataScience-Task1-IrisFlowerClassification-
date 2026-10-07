<img width="1404" height="396" alt="Confusion_MatrixIRIS" src="https://github.com/user-attachments/assets/59d8419f-0b96-4e4e-ab7f-9d5f0fe97a37" />
<img width="1115" height="1025" alt="PAIRPLOTS_IRIS" src="https://github.com/user-attachments/assets/1fbe3034-3dc5-4cba-8daa-aa35d0fcfbe4" />
# OIBSIP-DataScience-Task1-IrisFlowerClassification-
🌸 Iris Flower Classification
Track: Data Science Internship: Oasis Infobyte Task: Task 1 — Iris Flower Classification

Overview
This project builds and evaluates machine learning classification models to identify the species of an iris flower — Setosa, Versicolor, or Virginica — based on four physical measurements: sepal length, sepal width, petal length, and petal width.

Dataset
Source: Built into scikit-learn (sklearn.datasets.load_iris()) — no external download required
Samples: 150 (50 per class)
Features: 4 continuous numerical features (measurements in cm)
Classes: Setosa, Versicolor, Virginica
Missing values: None
Tech Stack
Python 3
Jupyter Notebook
pandas
numpy
matplotlib
seaborn
scikit-learn
Project Structure
OIBSIP/DataScience-Task1-IrisFlowerClassification/
│
├── iris_classification.ipynb   # Main Jupyter Notebook
[IrisFlowerClassification.ipynb](https://github.com/user-attachments/files/33158912/IrisFlowerClassification.ipynb)

├── README.md                   # Project documentation
└── screenshots/                # Output plots and confusion matrices
What the Notebook Covers
Data Loading — Iris dataset loaded from scikit-learn and converted to a pandas DataFrame
EDA — Shape, data types, null value check, descriptive statistics, class distribution
Visualisations — Pairplot (feature distributions by species) and box plots for each feature
Feature Selection — Correlation matrix analysis; petal features identified as most discriminative
Train/Test Split — 80/20 stratified split (120 train, 30 test)
Feature Scaling — StandardScaler applied to features for Logistic Regression and KNN
Model Training — Three classifiers trained and compared:
Logistic Regression
K-Nearest Neighbours (k=5)
Decision Tree
Evaluation — Accuracy score, confusion matrix, and classification report (precision, recall, F1) for each model
Best Model Selection — Justified selection with evidence from evaluation metrics
Results
Model	Accuracy
Logistic Regression	93.33%
K-Nearest Neighbours	93.33%
Decision Tree	93.33%
All three models achieved identical accuracy. Logistic Regression was selected as the best model based on:

Balanced precision and recall (0.90/0.90) for both Versicolor and Virginica
High interpretability via model coefficients
No hyperparameter sensitivity and strong scalability
All models classified Setosa perfectly (precision and recall = 1.00), consistent with its clear linear separability observed in EDA.

Key Findings
Petal length and petal width are the most discriminative features (correlation r = 0.96)
Sepal width is the least discriminative feature, showing significant overlap across all species
Versicolor and Virginica overlap around 6.4 cm in both sepal and petal length — the primary source of misclassification
Setosa is linearly separable and trivially classified by all models
How to Run
Clone the repository
Open iris_classification.ipynb in Jupyter Notebook or JupyterLab
Run all cells top to bottom (Kernel > Restart & Run All)
No additional data downloads required — the dataset is loaded directly from scikit-learn.

Author
Christina Sebueng Data Science Track — Oasis Infobyte Internship


