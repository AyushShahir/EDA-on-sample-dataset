# Week 1 - Data Preprocessing and Exploration on Iris Dataset

This repository contains the work for **Week 1 Tasks**, focusing on exploratory data analysis (EDA), data cleaning, label encoding, and feature scaling using the classic Iris dataset.

---

## 📌 Project Overview

The objective of this task is to perform foundational data preprocessing and exploratory data analysis using Python and popular data science libraries (`pandas`, `numpy`, `scikit-learn`).

Key preprocessing steps performed:
1. **Data Ingestion**: Loading the Iris dataset from a CSV file.
2. **Exploratory Data Analysis (EDA)**:
   - Inspecting structural information (`df.info()`, `df.shape`).
   - Summary statistics (`df.describe()`).
   - Class/target distribution check (`value_counts()`).
3. **Data Cleaning**:
   - Checking for null/missing values (`df.isnull().sum()`).
   - Checking for duplicated rows (`df.duplicated().sum()`).
4. **Feature Encoding**:
   - Encoding categorical target labels (`Species`) into numerical values using `LabelEncoder`.
5. **Feature Scaling**:
   - Extracting feature matrices.
   - Standardizing numerical features (`SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`, `PetalWidthCm`) using `StandardScaler` (and `MinMaxScaler`).

---

## 📁 Repository Structure

```text
Week1-Tasks/
├── Iris.csv         # Dataset containing flower measurements and species labels
├── task1.ipynb      # Jupyter Notebook containing the data preprocessing pipeline
└── README.md        # Documentation of the project
```

---

## 📊 Dataset Description

The **Iris dataset** comprises 150 records across 3 species of Iris flowers (*Iris-setosa*, *Iris-versicolor*, *Iris-virginica*), with 50 samples per species.

### Features:
- `Id`: Unique row identifier
- `SepalLengthCm`: Length of the sepal (in cm)
- `SepalWidthCm`: Width of the sepal (in cm)
- `PetalLengthCm`: Length of the petal (in cm)
- `PetalWidthCm`: Width of the petal (in cm)
- `Species`: Target flower class

---

## ⚙️ Installation & Setup

### Prerequisites
Make sure you have Python 3.8+ installed.

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/Week1-Tasks.git
cd Week1-Tasks
```

### 2. Create and activate a virtual environment (optional but recommended)
```bash
python -m venv venv
# On macOS/Linux:
source venv/bin/activate
# On Windows:
# venv\Scripts\activate
```

### 3. Install required libraries
```bash
pip install pandas numpy scikit-learn jupyter
```

---

## 🚀 Running the Notebook

Launch Jupyter Notebook or Jupyter Lab:

```bash
jupyter notebook task1.ipynb
```

Make sure to run the cells sequentially from top to bottom.

> **Note**: In `task1.ipynb`, ensure the first import cell (`from sklearn.preprocessing import LabelEncoder, StandardScaler, MinMaxScaler`) is executed before running the feature scaling cell.

---

## 🛠️ Tech Stack

- **Language**: Python
- **Data Manipulation**: `pandas`, `numpy`
- **Machine Learning / Preprocessing**: `scikit-learn`
- **Environment**: Jupyter Notebook
