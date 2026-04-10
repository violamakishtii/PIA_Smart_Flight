# PIA_Smart_Flight
# ✈️ PIA 2026 Smart Flight Dataset – Neural Network Project

## 📌 Overview

This project applies **Machine Learning and Neural Networks** to a real-world airline dataset from Pakistan International Airlines (PIA).  

The goal is to predict whether a flight will be **On Time or Delayed**, while analyzing operational, financial, and environmental factors.

The project is built using:
- Python 🐍
- Scikit-learn 🤖
- Neural Networks (MLPClassifier)
- Pandas & NumPy
- Matplotlib & Seaborn

---

## 🎯 Problem Statement

Predict flight punctuality using real airline operational data:

- Input: Flight details (weather, passengers, aircraft, route, etc.)
- Output: `On_Time_Status` (0 = On Time, 1 = Delayed)

---

## 📊 Dataset

The dataset contains 800 flight records with features such as:

- Flight duration
- Passenger count
- Load factor
- Ticket price & revenue
- Delay minutes & categories
- Weather conditions
- Fuel consumption & CO₂ emissions
- Customer rating

---

## ⚙️ Project Pipeline

### 1. Data Preprocessing
- Removed irrelevant columns:
  - `Flight_ID`
  - `Date`
  - `Customer_Feedback`
- Encoded categorical variables using `LabelEncoder`
- Converted target variable:
  - On Time → 0
  - Delayed → 1
- Applied feature scaling using `StandardScaler`

---

## 🧠 Machine Learning Models

### 🔵 Basic Neural Network (Baseline Model)

```python
hidden_layer_sizes=(16,)
