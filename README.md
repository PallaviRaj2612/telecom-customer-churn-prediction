# Telecom Customer Churn Prediction

This project predicts whether a telecom customer is likely to **churn** (leave the service) based on usage patterns, billing information, network quality, and customer complaints.  
The goal is to help telecom companies **identify at-risk customers** early and take action to retain them.

---

## Business Problem

Telecom companies lose significant revenue when customers leave (churn).  
Understanding **why customers churn** helps:

- Improve customer experience
- Reduce revenue loss
- Offer targeted retention plans
- Improve service quality

The objective is to build a model that can **predict churn** so the business can **take preventive action**.

---

## Dataset Description

The dataset contains customer-level details such as:

| Feature | Description |
|--------|-------------|
| `monthly_charges` | Monthly bill amount for customer |
| `total_data_usage_gb` | Total monthly data usage |
| `customer_complaints` | Number of complaints in last 3 months |
| `network_quality_rating` | Network satisfaction score (1–5) |
| `tenure_months` | Number of months with the company |
| `contract_type` | Prepaid / Postpaid |
| `churn` | Target variable (1 = churn, 0 = stay) |

---

## Techniques & Tools Used

| Category | Method |
|---------|--------|
| Language | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |
| ML Algorithms | Logistic Regression, Random Forest, XGBoost |
| Class Imbalance Solution | **SMOTE Oversampling** |
| Model Evaluation | Recall, Precision, F1-Score, Confusion Matrix |

---

## Model Results

| Metric | Value |
|--------|-------|
| **Accuracy** | ~62% |
| **Recall (Churn Class)** | ~45% after threshold tuning |

In churn problems, **catching customers who are leaving is more important** than overall accuracy.

A slightly lower accuracy is acceptable if **more churners are detected**.

---

## Feature Importance Insights

Top factors influencing customer churn:

| Feature | Insight |
|--------|---------|
| **Customer Complaints** | More complaints → higher churn risk |
| **Network Quality** | Poor network rating → customers leave |
| **Monthly Charges** | Higher bills → dissatisfaction → churn |
| **Low Data Usage** | Less engagement → silent churn risk |
| **Prepaid Customers** | More churn-prone due to easy switching |


---

## 📂 Project Files

| File | Description |
|------|------------|
| `telecom_churn_prediction.ipynb` | Full model training notebook |
| `telecom_churn_dataset.csv` | Dataset used for training |
| `README.md` | Project explanation |

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Deploy model as API using Flask
- Dashboard in Power BI / Tableau for management team

---

## 💛 Developed By
**Pallavi Raj**  
Aspiring Data Scientist | 6 Years Telecom + M.Tech DS & ML  

