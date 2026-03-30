# E-Commerce Delivery Prediction

## Objective

The goal of this project is to predict whether an e-commerce product delivery will be delayed or delivered on time using machine learning techniques.

---

## Business Problem

Delayed deliveries negatively impact customer satisfaction and operational efficiency. This project aims to proactively identify high-risk shipments so that logistics teams can take preventive actions.

---

## Project Notebook

https://github.com/shewill-gif/E-Commerce-Delivery-Delay-Prediction/blob/main/capstone_project_ecom_delivery_prediction.ipynb

---

## Project Dataset

https://github.com/shewill-gif/E-Commerce-Delivery-Delay-Prediction/blob/main/E_Commerce.xlsx

## Dataset Features

* Shipment details (Mode, Warehouse)
* Product attributes (Weight, Cost, Importance)
* Customer behavior (Calls, Ratings, Prior purchases)
* Discounts offered

---

## Exploratory Data Analysis (EDA)

Key insights:

* Higher discounts → increased delay probability
* Ship mode → more delays
* Warehouse F → higher workload and delays
* Weight and discount interaction affects delivery

---

## Feature Engineering

* Encoded categorical variables using One-Hot & Ordinal Encoding
* Additional features shown below were created to capture interactions that was showing relation with delivery timings
   Discount-weight interaction
   High discount flag
   Heavy product flag
  These features help the model capture non-linear relationships affecting delays. 

---

## Models Used

* Logistic Regression
* Decision Tree
* Random Forest
* K-Nearest Neighbors (KNN)

---

## Model Optimization


Threshold tuning was applied by lowering the classification threshold from 0.5 to 0.4. class_weight also adjusted to {0:1, 1:3} putting more focus on  delayed class. This increased recall by identifying more delayed deliveries, at the cost of slightly  increased false positives. This trade-off was acceptable given the business objective.”

---

## Model Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Random Forest       | 0.6804   |
| Logistic Regression | 0.6522   |
| KNN                 | 0.6468   |
| Decision Tree       | 0.6277   |

---

## Final Model

**Random Forest** was selected due to:

Its high recall in detecting delayed deliveries, which aligns with the business goal of minimizing missed delays.”

---

## Key Trade-Off

The model was optimized for **recall** to reduce missed delays (False Negatives), which are more critical from a business perspective.

---

## Business Insights

* High discounts increase operational load → more delays
* Shipment mode significantly affects delivery time
* Warehouse workload impacts delay probability

---

## Business Recommendations

* Prioritize high-risk shipments
* Adjust shipping method for predicted delays
* Improve logistics at high-load warehouses
* Notify customers proactively

---

## Technologies Used

* Python (Pandas, NumPy)
* Scikit-learn
* Matplotlib & Seaborn

---

## Conclusion

This project demonstrates how machine learning can be used to improve delivery reliability and customer satisfaction through proactive decision-making.
