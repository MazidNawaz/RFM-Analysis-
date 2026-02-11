# 📊 Customer Segmentation using RFM Analysis

## 🚀 Project Overview

This project performs Customer Segmentation using **RFM (Recency, Frequency, Monetary) Analysis** on the UCI Online Retail dataset.  
K-Means clustering is applied to group customers based on their purchasing behavior and generate actionable business insights.

The goal is to transform raw transactional data into meaningful customer segments for targeted marketing strategies.

---

# 🧠 Problem Statement

Businesses need to understand:

- Who are the most valuable customers?
- Which customers are inactive or at risk of churn?
- How can marketing campaigns be personalized?
- How can customer retention be improved?

This project answers these questions using data-driven customer segmentation.

---

# 📂 Dataset Information

**Dataset:** Online Retail Dataset  
**Source:** UCI Machine Learning Repository  

### Key Columns:
- Invoice Number
- Invoice Date
- Customer ID
- Quantity
- Unit Price
- Country

---

# 🛠️ Project Workflow

## 1️⃣ Data Cleaning & Preprocessing

- Removed missing Customer IDs
- Converted date columns to datetime format
- Converted quantity and price to numeric format
- Removed negative quantity and price values
- Created new feature:


---

## 2️⃣ RFM Feature Engineering

For each customer, the following metrics were calculated:

| Metric | Definition |
|--------|------------|
| Recency | Days since last purchase |
| Frequency | Number of unique transactions |
| Monetary | Total amount spent |

Each customer is represented as:


---

## 3️⃣ Data Scaling

Since Recency, Frequency, and Monetary are on different scales, StandardScaler was applied to normalize the values before clustering.

---

## 4️⃣ Customer Segmentation using K-Means

K-Means clustering was applied:


These numerical clusters were interpreted based on average RFM values.

---

# 📊 Cluster Interpretation

Based on RFM patterns, clusters were labeled as:

| Segment | Behavior Pattern |
|----------|------------------|
| Loyal Customers | Low Recency, High Frequency, High Monetary |
| Lost Customers | High Recency, Low Frequency, Low Monetary |
| Regular Customers | Moderate RFM values |
| Big Spenders | High Monetary value |

---

# 📈 Key Insights

## Loyal Customers
- Purchase frequently
- Spend the most
- Recently active
- Suitable for VIP programs and premium offers

## Lost Customers
- Inactive for a long period
- Low engagement
- Can be targeted with reactivation campaigns

## Regular Customers
- Moderate purchasing behavior
- Potential to convert into loyal customers

## Big Spenders
- High transaction value
- Ideal for upselling premium products

---

# 📊 Visualizations Included

- RFM Distribution Plots
- Cluster Comparison Charts
- Customer Segment Distribution
- Revenue Distribution Analysis

These visualizations help clearly understand customer segmentation patterns.

---

# 💡 Business Applications

Customer segmentation enables:

- Targeted marketing campaigns
- Customer retention strategies
- Revenue optimization
- Personalized engagement

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# 🔮 Future Improvements

- Apply Elbow Method to determine optimal clusters
- Build a churn prediction model
- Predict Customer Lifetime Value (CLV)
- Develop an interactive dashboard

---

# 🎯 Key Learning Outcomes

- Practical implementation of RFM analysis
- Understanding unsupervised learning (K-Means)
- Cluster interpretation and business mapping
- Customer behavior analytics

---

# 📌 Resume Highlight

Performed RFM-based customer segmentation using K-Means clustering on the Online Retail dataset to derive actionable marketing insights and improve customer retention strategies.

---

# 👨‍💻 Author

Mazid Nawaz Ahmad  
Data Science Enthusiast | Customer Analytics | Machine Learning
