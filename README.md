## 🔗 Project Overview
This project predicts delivery delays using machine learning to improve logistics efficiency and customer satisfaction.

## 📎 Project Notebook
[Click here to view notebook](./capstone_project_ecom_delivery_prediction.ipynb)

# E-Commerce Delivery Delay Prediction

## 📌 Problem Statement
Predict whether a product delivery will be delayed to improve logistics efficiency and reduce customer complaints.

## 📊 Dataset
- 10,999 records
- 12 features
- Target: Reached.on.Time_Y.N
  - 0 → On-time delivery
  - 1 → Delayed delivery

## ⚙️ Approach
- Data preprocessing and encoding
- Exploratory Data Analysis (EDA)
- Model building and comparison
- Model validation using Stratified K-Fold

## 🤖 Final Model
Random Forest (tuned)

## 📈 Results
- Accuracy: ~69%
- Strong performance in predicting on-time deliveries
- Moderate recall for delayed deliveries

## 🔍 Key Insights
- Higher discounts are associated with increased delivery delays
- Heavier products are more likely to be delivered on time
- Higher shipment volume in Warehouse Block F may contribute to delivery delays
- Shipment mode impact is volume-driven

## 💡 Business Recommendations
- Balance warehouse load
- Optimize shipment planning
- Manage discount strategies
- Improve inventory distribution
