# 📦 E-Commerce Delivery Prediction

## 🎯 Objective

The goal of this project is to predict whether an e-commerce product delivery will be delayed or delivered on time using machine learning techniques.

---

## 💼 Business Problem

Delayed deliveries negatively impact customer satisfaction and operational efficiency. This project aims to proactively identify high-risk shipments so that logistics teams can take preventive actions.

---

## 📊 Dataset Features

* Shipment details (Mode, Warehouse)
* Product attributes (Weight, Cost, Importance)
* Customer behavior (Calls, Ratings, Prior purchases)
* Discounts offered

---

## 🔍 Exploratory Data Analysis (EDA)

Key insights:

* Higher discounts → increased delay probability
* Ship mode → more delays
* Warehouse F → higher workload and delays
* Weight and discount interaction affects delivery

---

## ⚙️ Feature Engineering

* Encoded categorical variables using One-Hot & Ordinal Encoding

---

## 🤖 Models Used

* Logistic Regression
* Decision Tree
* Random Forest
* K-Nearest Neighbors (KNN)

---

## 📊 Model Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Random Forest       | 0.6804   |
| Logistic Regression | 0.6522   |
| KNN                 | 0.6468   |
| Decision Tree       | 0.6277   |

---

## 🏆 Final Model

**Random Forest** was selected due to:

* Highest accuracy
* Better generalization
* Ability to capture complex relationships

---

## ⚖️ Key Trade-Off

The model was optimized for **recall** to reduce missed delays (False Negatives), which are more critical from a business perspective.

---

## 💡 Business Insights

* High discounts increase operational load → more delays
* Shipment mode significantly affects delivery time
* Warehouse workload impacts delay probability

---

## 🚀 Business Recommendations

* Prioritize high-risk shipments
* Adjust shipping method for predicted delays
* Improve logistics at high-load warehouses
* Notify customers proactively

---

## 🧠 Technologies Used

* Python (Pandas, NumPy)
* Scikit-learn
* Matplotlib & Seaborn

---

## 📌 Conclusion

This project demonstrates how machine learning can be used to improve delivery reliability and customer satisfaction through proactive decision-making.
