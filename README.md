# 🏨Hotel-Reservation-Analysis-and-Prediction

## 🧠 Problem Statement:

Hotel booking cancellations significantly impact business planning and revenue. Understanding which bookings are likely to be cancelled helps hotels:

- Optimize room availability.
- Improve customer experience.
- Increase revenue by reducing last-minute cancellations.

This project aims to **predict whether a hotel reservation will be canceled** using various features such as customer type, booking dates, special requests, and more.

---

## 📂 Dataset:

Source: https://www.kaggle.com/datasets/mojtaba142/hotel-booking
File: `hotel_booking.csv` 

The dataset includes the following features:

- - hotel, lead_time, arrival_date, stays, adults, children, meal, country, market_segment, distribution_channel, repeated_guest, previous_cancellations, reserved_room_type, booking_changes, deposit_type, days_in_waiting_list, customer_type, adr, special_requests, reservation_status_date, is_canceled

---

## 🚀 Approach:

A full machine learning pipeline was built, involving:

### 1. Data Exploration:
- Explored structure and distributions using **pandas**, **numpy**, **matplotlib**, and **seaborn**.
- Plotted booking trends, cancellation patterns, and customer behaviors.

### 2. EDA: Data Cleaning & Feature Engineering:
- **Datetime conversion**: Converted `reservation_status_date` to datetime format.
- **Label Encoding**: Converted categorical features like hotel type, deposit type, and customer type.
- **Scaling**: Not needed for tree-based models but considered for others.
- Removed unnecessary or constant columns.

### 3. Model Building:
Tested the following classification models:

- Random Forest Classifier
- XGBoost Classifier
- (Optional: Logistic Regression, Decision Tree)

### 4. Model Selection & Evaluation:
Evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report

### 5. Testing with New Data:
- Checked model prediction using new, unseen single samples to simulate live inference.

---
## 📚 Libraries Used:

- **pandas** – Data manipulation  
- **numpy** – Numerical operations  
- **matplotlib** & **seaborn** – Data visualization  
- **scikit-learn** – ML algorithms and evaluation  
- **xgboost** – Advanced gradient boosting  
---
