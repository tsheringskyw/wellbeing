# 🌿 Student Wellbeing - Bhutan

Machine learning project built with **Python** and **Streamlit** to demonstrate how a classification model can explore patterns associated with student wellbeing.

> **Important:** This project uses **synthetic data only**. It is an educational demonstration and is **not** a medical, psychological, screening, or diagnostic tool.

## 📌 Project Overview

The application generates fictional student records representing students across **all 20 Dzongkhags of Bhutan**.

The project uses **Logistic Regression** to demonstrate a basic machine-learning workflow:

1. It generates synthetic data
2. Split the data into training and testing sets
3. Preprocess numerical and categorical variables
4. Train a Logistic Regression model
5. Evaluate the model
6. Display the results through an interactive Streamlit application

## 🇧🇹 Bhutan Context

Bhutan is divided into 20 Dzongkhags. This project includes the Dzongkhag field as a categorical feature to demonstrate how location information can be incorporated into a machine-learning dataset.

The 20 Dzongkhags included are:

- Bumthang
- Chukha
- Dagana
- Gasa
- Haa
- Lhuentse
- Mongar
- Paro
- Pema Gatshel
- Punakha
- Samdrup Jongkhar
- Samtse
- Sarpang
- Thimphu
- Trashigang
- Trashiyangtse
- Trongsa
- Tsirang
- Wangdue Phodrang
- Zhemgang

## 📊 Features in the Dataset

Each fictional student record contains information such as:

- Age
- Gender
- Dzongkhag
- Residence
- Sleep hours
- Study hours per day
- Physical activity days per week
- Stress level
- Social support
- Financial pressure
- Academic pressure
- Screen time
- Mental-health awareness

The target variable is:

`support_need`

with two synthetic outcomes:

- `Support recommended`
- `No immediate flag`

## 🖥️ Application Sections

### Overview

Provides the project objective, number of fictional records, number of input features, algorithm used, machine-learning workflow, and Bhutan context.

### Explore Data

Allows users to select numerical variables and view their distributions by synthetic outcome. The application also displays the first 20 fictional records and provides an option to download the generated dataset as a CSV file.

### Prediction Demo

Allows the user to create a fictional student profile using interactive controls and run an educational prediction using the trained Logistic Regression model.

### Model Results

Displays hold-out test results, including:

- Accuracy
- ROC-AUC
- Confusion Matrix
- Classification Report

## 🤖 Machine Learning

The project uses a **Logistic Regression** classifier.

The preprocessing pipeline includes:

- Median imputation and standardization for numerical variables
- Most-frequent imputation and one-hot encoding for categorical variables

The dataset is divided into:

- **80% training data**
- **20% testing data**

A fixed random seed is used so the synthetic dataset and train-test split are reproducible.

## 🧪 Synthetic Data

The dataset is generated directly inside the Python application using NumPy.

No real student survey responses or personal records are used.

The target label is also generated using a transparent fictional rule for educational purposes. Therefore, strong model performance should not be interpreted as evidence of real-world predictive performance.

## ⚠️ Limitations

This project is intended only for learning and demonstration.

The results:

- Do not represent real Bhutanese students
- Do not provide a medical or psychological diagnosis
- Should not be used for healthcare decisions
- Should not be used for academic, employment, or disciplinary decisions
- Do not establish causal relationships between variables

A real-world system would require informed consent, ethics approval, secure data handling, local validation, fairness testing, and appropriate professional oversight.

## 📦 requirements.txt

```text
streamlit
pandas
numpy
scikit-learn
matplotlib
seaborn
```

## 📁 Project Structure

```text
.
├── app.py
├── requirements.txt
└── README.md
```

## 👤 Project

**Tshering Wangchuk**

Educational machine-learning project focused on demonstrating basic data generation, preprocessing, classification, prediction, and model evaluation using fictional student wellbeing data from Bhutan.

---

**Synthetic data | Educational demonstration only**
