# NAFLD Mortality Prediction using Logistic Regression

> Machine Learning classification project that predicts patient survival outcomes using clinical data from individuals diagnosed with Non-Alcoholic Fatty Liver Disease (NAFLD).

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Logistic%20Regression-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## Overview

This project applies a **Logistic Regression** classifier to predict patient life status using clinical information from individuals diagnosed with **Non-Alcoholic Fatty Liver Disease (NAFLD)**.

The notebook demonstrates the complete machine learning workflow, including:

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Logistic Regression
- Model Evaluation
- Interpretation of Results

Beyond model development, the project emphasizes the importance of selecting appropriate evaluation metrics when working with **imbalanced medical datasets**.

---

## Project Workflow

```mermaid
flowchart TD
    Dataset[Dataset] --- Clean[Data Cleaning]
    Clean --- EDA[Exploratory Data Analysis]
    EDA --- Feature[Feature Engineering]
    Feature --- Split[Train/Test Split]
    Split --- LogReg[Logistic Regression]
    LogReg --- Eval[Model Evaluation]
    Eval --- Results[Results & Conclusions]

    style Dataset fill:#f9f,stroke:#333,stroke-width:2px
    style Results fill:#bbf,stroke:#333,stroke-width:2px
    style LogReg fill:#ff9,stroke:#333,stroke-width:2px

```

---

## Dataset

**Source**

https://www.kaggle.com/datasets/utkarshx27/non-alcohol-fatty-liver-disease

Dataset includes demographic and clinical measurements collected from patients diagnosed with NAFLD.

Target variable:

- Life Status
    - Alive
    - Deceased

The original dataset is included in the repository for reproducibility.

---

## Features

- Missing value handling
- Feature engineering
- Data normalization
- Exploratory data analysis
- Logistic Regression classifier
- Confusion Matrix
- Classification Report
- Balanced Accuracy
- ROC Curve
- Precision–Recall Curve
- Feature Importance visualization

---

## Repository Structure

```
nafld-mortality-prediction/
│
├── data/
│   └── nafld1.csv
│
├── images/
│
├── report
│   └── nafld_analysis
│
├── nafld_analysis.ipynb
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Installation

```bash
git clone https://github.com/mayramtv/nafld-logistic-prediction.git

cd nafld-logistic-prediction

python -m venv .venv

source .venv/bin/activate

# Windows
.venv\Scripts\activate

pip install -r requirements.txt
```

---

## Results

The Logistic Regression model achieved an overall accuracy of approximately **92%**.

However, because the dataset is highly imbalanced, additional evaluation metrics were used to provide a more comprehensive assessment of model performance.

The analysis showed that while the model correctly classified most surviving patients, it struggled to identify the minority (deceased) class, demonstrating why accuracy alone is not sufficient for evaluating imbalanced classification problems.

---

## Lessons Learned

This project provided practical experience with the complete supervised machine learning workflow while highlighting several important concepts:

- Data preprocessing significantly affects model performance.
- Medical datasets often contain class imbalance.
- Accuracy alone can be misleading.
- Confusion matrices and additional evaluation metrics provide a more complete understanding of classifier performance.
- Interpreting model limitations is as important as reporting model accuracy.

---

## Future Improvements

Possible extensions include:

- Class balancing techniques (SMOTE, class weighting)
- Hyperparameter optimization
- Cross-validation
- Comparison with Decision Trees, Random Forests, and Gradient Boosting
- Feature selection methods
- Model explainability using SHAP values

---

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

## References

Dataset:

https://www.kaggle.com/datasets/utkarshx27/non-alcohol-fatty-liver-disease

---

## License

This project is available under the MIT License.