# Iris Dataset Exploratory Data Analysis

## Overview

This project performs a structured **Exploratory Data Analysis (EDA)** on the classic **Iris dataset** using Python.  
The goal is to understand the dataset’s structure, validate data quality, analyze feature distributions, and explore relationships between flower measurements and species.

The Iris dataset is a foundational dataset in machine learning and statistics, making this project a clear demonstration of EDA best practices on clean, well-labeled data.

---

## Dataset Description

- **Source:** `sklearn.datasets.load_iris`
- **Records:** 150 samples
- **Features:**
  - Sepal length (cm)
  - Sepal width (cm)
  - Petal length (cm)
  - Petal width (cm)
- **Target Variable:** Species  
  - Setosa
  - Versicolor
  - Virginica

The dataset is saved locally as `iris.csv` for reference and reuse.

---

## Repository Contents

```

├── iris.csv            # Exported Iris dataset
├── EDA notebook/code   # Data loading, analysis, and visualization
└── README.md           # Project documentation

```

---

## Data Loading and Preparation

- Loaded the Iris dataset using `sklearn.datasets.load_iris`
- Converted the dataset into a pandas DataFrame
- Mapped numerical target labels to species names
- Exported the dataset to CSV format

---

## Data Quality Checks

### Data Types
- Numerical features stored as `float64`
- Species stored as categorical (`object`)

### Missing Values
- No missing values detected in any column

This confirms the dataset is clean and suitable for analysis without imputation.

---

## Descriptive Statistics

Summary statistics were computed using `df.describe()` and `df.describe(include='all')` to understand:

- Central tendencies (mean, median)
- Spread (standard deviation, quartiles)
- Range and extreme values
- Species distribution

Each species contains exactly 50 samples, confirming a balanced dataset.

---

## Exploratory Analysis

### Univariate Analysis
- Histograms generated for all numerical features
- Observed distribution shapes and spread across measurements

### Box Plot Analysis
- Box plots created for all numerical features
- Species-wise box plots used to compare feature distributions
- Clear separation observed between species, especially in petal measurements

These visualizations highlight which features are most discriminative across species.

---

## Visualizations Used

- Histograms for numerical feature distributions
- Box plots for:
  - Overall feature spread
  - Feature values grouped by species
- Species-wise comparisons for each feature

Visualization libraries:
- matplotlib
- seaborn

---

## Tools and Libraries

- Python
- pandas
- scikit-learn
- matplotlib
- seaborn

---

## Key Takeaways

- The Iris dataset is clean, balanced, and well-structured
- Petal length and petal width show strong separation between species
- Sepal measurements exhibit more overlap but still provide useful signals
- EDA confirms the dataset is well-suited for classification tasks

---

## Next Steps

- Feature scaling and normalization
- Train classification models (Logistic Regression, KNN, SVM)
- Visualize decision boundaries
- Evaluate model performance using accuracy and confusion matrices

---

This project demonstrates a clear, methodical approach to exploratory data analysis and data understanding, forming a strong foundation for downstream machine learning tasks.
