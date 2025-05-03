# 📦 Customer Segmentation Using RFM Analysis

## 📚 Overview

This project implements a comprehensive RFM (Recency, Frequency, Monetary) analysis to segment e-commerce customers and drive strategic business decisions. It focuses on understanding customer behavior and value through advanced data analytics and clustering, enabling more targeted marketing and improved customer retention.

Developed as part of **IE6400 – Foundations of Data Analytics Engineering**, this project is a collaborative effort to convert raw transaction data into actionable insights using Python-based tools and machine learning techniques.

---

## 🔍 Objectives

- Perform end-to-end customer segmentation using RFM metrics.
- Use clustering algorithms to group customers based on behavior.
- Identify high-value and at-risk customers.
- Recommend personalized marketing strategies.
- Analyze patterns in customer orders, returns, geographies, payments, and sentiments.

---

## 🛠 Tools & Technologies

- **Languages**: Python
- **Libraries**: pandas, numpy, seaborn, matplotlib, scikit-learn
- **Techniques**: RFM analysis, K-Means clustering, Elbow Method, Silhouette Score
- **Visualization**: 3D scatter plots, bar charts, heatmaps, line graphs
- **Sentiment & Profitability Analysis**: Custom logic for customer rating, returns, and product margins

---

## 📁 Project Structure

- `Customer_segmentation.ipynb` – Code implementation of the entire pipeline.
- `rfm_clusters.csv` – Final segmented dataset with RFM scores and cluster labels.
- `REPORT.pdf` – Detailed report including methodology, analysis, and business insights.

---

## 🧪 Methodology

### 1. Data Preprocessing
- Loaded and cleaned e-commerce transactional data.
- Handled nulls, corrected data types, and transformed time-based features.
- Added derived columns for `TotalPrice`, `OrderProcessingTime`, etc.

### 2. RFM Metrics Calculation
- **Recency**: Days since last purchase.
- **Frequency**: Number of unique transactions.
- **Monetary**: Total spending per customer.

### 3. RFM Scoring & Aggregation
- Calculated **R_Score**, **F_Score**, **M_Score** using quartiles.
- Generated combined `RFM_Score = 100*R + 10*F + M`.

### 4. Customer Segmentation with K-Means
- Standardized RFM scores.
- Determined optimal `k` using Elbow Method and Silhouette Score.
- Applied **K-Means** to segment customers into 4 groups.

### 5. Cluster Profiling
| Cluster | Characteristics | Description |
|--------|------------------|-------------|
| 0 | High Frequency, Low Recency, High Monetary | Active & High-Value Customers |
| 1 | Low Frequency, High Recency, Low Monetary | Dormant or Lapsed Customers |
| 2 | Moderate Frequency & Recency, High Monetary | Occasional High Spenders |
| 3 | Low Monetary, Moderate Frequency & Recency | Moderately Engaged Customers |

---

## 📊 Additional Analyses

### 📦 Product Insights
- Top-selling products by quantity and revenue.
- Categories with highest returns.
- Most profitable items by margin.

### 🕒 Time-based Patterns
- Most active days: **Fridays & Mondays**.
- Peak hours: **12–2 PM** and **6–8 PM**.
- Summer months (June–Aug) had the highest order volumes.

### 🌍 Geographical Trends
- **Top 5 countries** by order count: UK, Germany, France, EIRE, Spain.
- Heatmap of average order value vs. quantity per country.

### 💳 Payment Trends
- Simulated data to assess payment methods: Internet Banking and Google Pay had higher order amounts.

### 📈 Sentiment Analysis
- Customer ratings categorized into **Positive**, **Neutral**, **Negative**.
- Most customers rated neutrally (50%), followed by equal parts positive and negative (25% each).

---

## 📌 Key Business Recommendations

### 🎯 Segment 0 – Active High Spenders
- Run loyalty programs, upsell, personalized offers.

### 💤 Segment 1 – Dormant
- Reactivation campaigns, reminders, satisfaction surveys.

### 💰 Segment 2 – Occasional High Spenders
- Promote premium products, offer VIP benefits.

### 🛍 Segment 3 – Moderate Buyers
- Increase frequency with deals, product discovery incentives.

---

## ✅ Conclusion

This project demonstrated the power of RFM analysis in understanding and segmenting customers based on their purchasing behavior. By integrating data preprocessing, RFM scoring, clustering, and various business intelligence techniques, we uncovered valuable insights into customer patterns and proposed data-driven strategies for customer engagement and retention. The incorporation of product, payment, temporal, sentiment, and profitability analysis further deepened our understanding of customer value.

Through effective visualization and profiling, this framework empowers businesses to:
- Identify and reward loyal customers,
- Reactivate dormant users,
- Optimize inventory and marketing efforts,
- Enhance customer satisfaction and profitability.

This analysis lays a strong foundation for implementing more advanced customer lifecycle management systems and supports data-informed business decision-making.


