# 🏨 StaySure: Hotel Booking Prediction Project

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Features Description](#features-description)
- [Project Objectives](#project-objectives)
- [Technologies Used](#technologies-used)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Contributing](#contributing)

---

## 📖 Project Overview
The **StaySure Hotel Booking Prediction Project** is a Machine Learning initiative designed to predict hotel reservation cancellations. By analyzing historical booking data, this project aims to help hotel management anticipate customer behavior, optimize room allocation, reduce revenue loss, and improve overall operational efficiency.

---

## 📊 Dataset Information
The core of this project relies on the `booking.csv` dataset, which contains **36,285 records** and **17 attributes** capturing customer demographics, reservation details, and historical behaviors. 

- **File Name:** `booking.csv`
- **Total Rows:** 36,285
- **Total Columns:** 17
- **Target Variable:** `booking status` (Classifies whether a booking was `Canceled` or `Not_Canceled`)

---

## 🔍 Features Description

Here is a breakdown of the variables available in the dataset:

| Feature Name | Data Type | Description |
| :--- | :--- | :--- |
| **Booking_ID** | `object` | Unique identifier for each booking. |
| **number of adults** | `int` | Number of adults included in the reservation. |
| **number of children** | `int` | Number of children included in the reservation. |
| **number of weekend nights** | `int` | Number of weekend nights (Saturday/Sunday) the guest stayed or booked. |
| **number of week nights** | `int` | Number of weeknights (Monday to Friday) the guest stayed or booked. |
| **type of meal** | `object` | The meal plan chosen by the guest (e.g., Meal Plan 1, Not Selected). |
| **car parking space** | `int` | Indicates if a car parking space was required (1 = Yes, 0 = No). |
| **room type** | `object` | Type of room reserved by the customer. |
| **lead time** | `int` | Number of days between the booking date and the arrival date. |
| **market segment type** | `object` | Market segment designation (e.g., Online, Offline, Corporate). |
| **repeated** | `int` | Indicates if the guest is a returning customer (1 = Yes, 0 = No). |
| **P-C** | `int` | Number of previous bookings that were **canceled** by the customer. |
| **P-not-C** | `int` | Number of previous bookings **not canceled** by the customer. |
| **average price** | `float` | Average price per day for the reservation (in USD). |
| **special requests** | `int` | Total number of special requests made by the customer. |
| **date of reservation** | `object` | The specific date the reservation was made. |
| **booking status** *(Target)* | `object` | Outcome of the booking (`Canceled` or `Not_Canceled`). |

---

## 🎯 Project Objectives
1. **Exploratory Data Analysis (EDA):** Identify trends, seasonality, and factors that highly correlate with booking cancellations (e.g., lead time, deposit type, special requests).
2. **Data Preprocessing:** Handle missing values, encode categorical variables (like `room type` and `market segment type`), and parse dates.
3. **Predictive Modeling:** Train various classification algorithms (e.g., Logistic Regression, Random Forest, XGBoost) to classify the `booking status`.
4. **Evaluation:** Use metrics such as Accuracy, Precision, Recall, and F1-Score to determine the most effective model, minimizing false negatives (unexpected cancellations).

---

## 💻 Technologies Used
- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn`
- **Environment:** Jupyter Notebook / VS Code

---

## ⚙️ Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/MoamenHassaballah/StaySure_Hotel_Booking_Prediction_Project.git](https://github.com/MoamenHassaballah/StaySure_Hotel_Booking_Prediction_Project.git)
   cd StaySure_Hotel_Booking_Prediction_Project
