# 📊 Assessing Urban-Rural Income Disparities in the USA A Data-Driven Approach Using Predictive Analytics
## 🧠 Project Overview

This project investigates **income disparities between urban and rural counties across the United States** using a data-driven predictive analytics approach. With increasing attention on economic inequality and regional development, understanding such disparities is critical for effective policymaking and social equity.

The primary objective is to classify whether a given county is **urban or rural** based on socio-economic and demographic attributes using machine learning techniques. The classification task was approached using **Logistic Regression**, **Support Vector Machine**, and **XGBoost**, each fine-tuned for optimal performance.

---

## 🗂️ Dataset Description

The dataset consists of **3,222 counties** in the USA and includes the following columns:

- `County`
- `State`
- `FIPS`
- `State FIPS Code`
- `County FIPS Code`
- `Total Population`
- `Median Household Income`
- `Urban-Rural` *(Target)*

---

## 🔍 Exploratory Data Analysis Highlights

- Visualized median household income distributions across urban and rural regions.
- Analyzed population density and income relationships.
- Built interactive choropleth maps to show geographical income disparities.
- Identified urban-rural clusters using income and population indicators.

---

## ⚙️ Data Preprocessing

- Missing values check & validation: None found.
- Encoded target variable (`Urban-Rural`) into binary format.
- Feature scaling using `StandardScaler`.
- Stratified data split into training and testing sets (80/20 split).

---

## 🤖 Modeling & Results

Three classification models were applied and fine-tuned using `GridSearchCV`. Below are the final evaluation metrics:

---

### 🔹 Logistic Regression
- **Accuracy**: `0.9938`

```
              precision    recall  f1-score   support

           0       0.99      0.99      0.99       329
           1       0.99      0.99      0.99       316

    accuracy                           0.99       645
   macro avg       0.99      0.99      0.99       645
weighted avg       0.99      0.99      0.99       645
```

---

### 🔹 Support Vector Machine (SVM)
- **Accuracy**: `0.9829`

```
              precision    recall  f1-score   support

           0       0.99      0.98      0.98       329
           1       0.98      0.99      0.98       316

    accuracy                           0.98       645
   macro avg       0.98      0.98      0.98       645
weighted avg       0.98      0.98      0.98       645
```

---

### 🔹 XGBoost Classifier
- **Accuracy**: `0.9969`

```
              precision    recall  f1-score   support

           0       1.00      0.99      1.00       329
           1       0.99      1.00      1.00       316

    accuracy                           1.00       645
   macro avg       1.00      1.00      1.00       645
weighted avg       1.00      1.00      1.00       645
```

---

## 📈 Business Impact

Understanding and predicting **urban-rural classification** based on income and demographic variables enables:

- 📍 **Policy Makers** to allocate resources more effectively.
- 🏛️ **Governments** to target income-support or development programs based on region-specific needs.
- 🧑‍💼 **Economic Planners** to model infrastructure investments in underserved rural counties.
- 🧭 **Data-driven governance** for sustainable rural development and reduced inequality.


