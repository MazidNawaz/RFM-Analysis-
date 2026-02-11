📈 Customer Segmentation using RFM Analysis

This project performs Customer Segmentation using Recency, Frequency, and Monetary (RFM) analysis combined with K-Means clustering on the UCI Online Retail dataset to gain insights into customer behavior and group customers with similar buying patterns.

🔍 Project Description

RFM analysis is a popular and effective marketing technique used to evaluate past customer purchasing behavior. It helps businesses distinguish between their most valuable and least active customers based on three key metrics:

Recency (R): How recently did the customer make a purchase?

Frequency (F): How often does the customer make purchases?

Monetary (M): How much money has the customer spent?

Grouping customers based on these metrics allows companies to tailor marketing campaigns, improve retention, and increase revenue.

🧠 Objective

The primary goals of this project are:

Clean and preprocess the raw retail transaction data

Calculate RFM values for each unique customer

Use K-Means clustering to segment customers into meaningful groups

Interpret and label clusters with business-friendly segment names

Provide actionable marketing insights for each customer group

🧩 Dataset

The dataset used in this project is the Online Retail dataset, which contains transactional records from a UK-based e-commerce store. It includes details like:

Invoice number

Stock code

Product description

Quantity

Invoice date

Unit price

Customer ID

Country

🛠️ Workflow Overview
1. Data Cleaning and Preprocessing

Handled missing CustomerID values

Converted dates to datetime format

Ensured numeric types for quantity and price columns

Removed negative values or returns

Created new feature Total_Spend

2. RFM Feature Engineering

Each customer is summarized by:

Metric	Meaning
Recency	Days since last purchase
Frequency	Number of unique transactions
Monetary	Total money spent
3. Data Scaling

Because Recency, Frequency, and Monetary have different scales, we applied standardization to ensure clusters are not biased toward the largest magnitude feature.

4. Clustering

We applied K-Means clustering to the scaled RFM values to segment customers into distinct groups.

5. Cluster Interpretation

By computing average R, F, M values per cluster, we interpret behavioral profiles like:

Loyal Customers: Recent purchases, frequent buying, high spending

Lost Customers: Infrequent or old purchases

Regular Customers: Moderate behavior

Big Spenders: High monetary value

📊 Results and Insights

The clusters were analyzed to understand customer value distribution. The segmentation provides insights like:

Loyal customers can be targeted with VIP programs

Lost customers can be reactivated with special offers

Regular buyers can receive loyalty rewards

High spenders can be upsold premium products

📈 Visualizations

The project includes visualizations such as:

Customer distribution by RFM values

Cluster counts

Pie charts showing customer segment proportions

Bar plots for segment comparison

These help in both exploring data and presenting results clearly.

💡 Business Applications

Customer segmentation helps answer business questions like:

Who are my most valuable customers?

Which customers are at risk of churn?

How do we tailor offers to different segments?

How can we improve customer retention?

RFM analysis and clustering empower data-driven decision making for marketing strategies.

📌 Technologies Used

Python (Pandas, NumPy)

Scikit-learn (StandardScaler, KMeans)

Matplotlib & Seaborn for visualization

🚀 Future Work

Potential enhancements include:

✔ Finding optimal number of clusters using the Elbow method
✔ Building predictive models (e.g., churn prediction)
✔ Creating an interactive dashboard
✔ Predicting Customer Lifetime Value (CLV)

📝 Conclusion

This project demonstrates how RFM analysis combined with clustering techniques can be used to extract meaningful customer segments from raw transactional data. By translating these segments into actionable marketing strategies, businesses can optimize customer engagement, retention, and profitability.
