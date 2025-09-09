
# 📊 Customer Churn Prediction – End-to-End ML Pipeline

This repository contains an **End-to-End Machine Learning Pipeline** for predicting **customer churn** using the **Telco Churn Dataset**. The project is implemented in **Python** with **scikit-learn Pipelines**.

## 📘 Project Overview

* Implements a **reusable ML pipeline** with preprocessing, modeling, and evaluation.
* Handles **categorical and numerical features**.
* Uses **GridSearchCV** for hyperparameter tuning.
* Saves the trained model with **joblib** for deployment.

## 📂 Repository Structure

```
├── DHC3135_Task_2_Phase_2.ipynb   # Main notebook with implementation
├── churn_pipeline.pkl             # Saved pipeline (after training)
└── README.md                      # Project documentation
```

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ Usage

Run the notebook:

```bash
jupyter notebook DHC3135_Task_2_Phase_2.ipynb
```

Or load the saved pipeline for prediction:

```python
import joblib

# Load trained pipeline
model = joblib.load("churn_pipeline.pkl")

# Example prediction
sample = [[...]]  # Replace with actual feature values
print(model.predict(sample))
```

## 📊 Models Used

* **Logistic Regression**
* **Random Forest**
* (Can easily extend with other classifiers)

## 📌 Requirements

* Python 3.8+
* pandas
* numpy
* scikit-learn
* joblib
