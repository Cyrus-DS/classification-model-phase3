# 🚗 Car Crash Severity Classification

This project focuses on building a classification model to predict the **severity of car crashes** based on crash-related features such as posted speed limit, traffic control devices, lighting and weather conditions, and more. The primary goal is to help identify patterns that can assist in minimizing the impact of future traffic incidents.

---

## 📌 Problem Statement

The objective is to classify the severity of a crash—based on vehicle damage—using various features present in traffic crash data. The classification categories were simplified to two:

- **$500 OR LESS** (Minor)
- **OVER $1,500** (Severe)

---

## 🔍 Key Questions

- Can we predict crash severity using available features?
- Which features have the greatest impact on crash severity?

---

## 📊 Dataset Overview

- **Total Records:** 669,927
- **Features Used:**
  - `POSTED_SPEED_LIMIT`
  - `TRAFFIC_CONTROL_DEVICE`
  - `DEVICE_CONDITION`
  - `LIGHTING_CONDITION`
  - `WEATHER_CONDITION`
  - `DAMAGE` (target variable)

### Data Preprocessing:
- Filtered for two severity levels
- One-hot encoding of categorical variables
- Train-test split (80/20)
- Standardization of numerical features

---

## 🧠 Models Implemented

### 1. Logistic Regression
- **Initial Accuracy:** 85%
- **Issue:** Model biased toward the majority class
- **Weighted Logistic Regression:**
  - **Accuracy:** 48%
  - Improved recall for the minority class

### 2. Random Forest Classifier
- **Accuracy:** 51%
- **Better handling of class imbalance**
- Performed better than Logistic Regression in identifying minor crashes

---

## 📈 Evaluation Metrics

Models were evaluated using:
- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix

Visualizations using Seaborn were created to better understand model predictions.

---

## 🧪 Tools & Libraries

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook

---

## 🚀 Future Improvements

- Try advanced models like **Gradient Boosting** and **XGBoost**
- Apply **SMOTE** or similar techniques to balance classes
- Introduce additional features and perform feature selection
- Conduct temporal or geographical analysis of crash patterns

---

## 📂 Project Structure

```

📁 project-root/
├── data/
│   └── Traffic\_crashes.csv
├── notebook/
│   └── crash\_severity\_classification.ipynb
├── models/
│   └── logistic\_regression.pkl
├── README.md
└── requirements.txt

```

---

## 📬 Contact

Have questions or suggestions? Feel free to:

- Open an [issue](https://github.com/Cyrus-DS/YourRepositoryName/issues)
- Connect with me on [LinkedIn](linkedin.com/in/cyrus-wambugu-b9476195)
- Visit my [GitHub profile](github.com/Cyrus-DS) for more projects


Feel free to open an issue or submit a pull request if you'd like to contribute or discuss improvements!

```




