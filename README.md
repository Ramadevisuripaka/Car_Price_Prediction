# 🚗 Car Price Prediction System

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Flask](https://img.shields.io/badge/Flask-Web%20App-lightgrey)
![ML](https://img.shields.io/badge/Machine%20Learning-Linear%20Regression-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 🌐 Live Demo

👉 **[Click here to view the live application](https://car-price-prediction-eyp4.onrender.com)**

---

## 📌 About This Project

The **Car Price Prediction System** is a Machine Learning web application that predicts the price of a car based on user inputs such as Brand, Year, Engine Size, Fuel Type, Transmission, Mileage, Condition, and Model.

This project was built to help **buyers and sellers estimate the fair market price of a car** without visiting multiple dealerships. It uses a trained ML model integrated into a Flask web application with a clean and colorful UI.

---

## 🎯 Why I Built This Project

- To apply real-world Machine Learning on a practical dataset
- To learn how to integrate an ML model with a Flask web application
- To understand how multiple features (brand, year, mileage, etc.) affect car price
- To build a complete end-to-end Data Science project from data to deployment
- To strengthen my portfolio as a Data Analyst and ML Engineer

---

## 🛠️ Tools and Technologies Used

| Tool / Technology | Purpose |
|---|---|
| **Python** | Core programming language |
| **Pandas** | Data loading and manipulation |
| **NumPy** | Numerical calculations |
| **Scikit-learn** | Machine Learning model training |
| **Matplotlib & Seaborn** | Data visualization and graphs |
| **Flask** | Web application framework |
| **HTML & CSS** | Frontend UI design |
| **Jinja2** | Template rendering in Flask |
| **Joblib** | Saving and loading the trained model |
| **GitHub** | Version control and project hosting |
| **VS Code** | Code editor |

---

## 📊 Dataset Overview

**Features Used:**
- Brand (Tesla, BMW, Audi, Ford, Honda, Mercedes, Toyota)
- Year of Manufacture
- Engine Size (in litres)
- Fuel Type (Petrol / Diesel)
- Transmission (Manual / Automatic)
- Mileage (in km)
- Condition (New / Used / Like New)
- Model (Model X, 5 Series, A4, Mustang, City, C Class, Innova)

**Target Variable:** Car Price (in currency units)

---

## 🧮 Manual Calculations (Step by Step)

### Step 1 — Label Encoding

Categorical values are converted to numbers before training:

| Brand | Encoded Value |
|---|---|
| Tesla | 0 |
| BMW | 1 |
| Audi | 2 |
| Ford | 3 |
| Honda | 4 |
| Mercedes | 5 |
| Toyota | 6 |

| Fuel Type | Encoded Value |
|---|---|
| Petrol | 0 |
| Diesel | 1 |

| Transmission | Encoded Value |
|---|---|
| Manual | 0 |
| Automatic | 1 |

| Condition | Encoded Value |
|---|---|
| New | 0 |
| Used | 1 |
| Like New | 2 |

---

### Step 2 — Linear Regression Formula

The model uses **Multiple Linear Regression**:
