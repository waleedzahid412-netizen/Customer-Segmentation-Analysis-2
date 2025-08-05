🛍️ Customer Segmentation Using K-Means Clustering
This project aims to perform customer segmentation on an e-commerce dataset by leveraging data cleaning, feature engineering, exploratory data analysis (EDA), and K-Means clustering to group customers based on purchasing behavior.

📂 Dataset Description
The dataset contains online retail transactions with fields such as:

Invoice

InvoiceDate

Customer ID

Country

StockCode

Quantity

Price

Each row represents a single product in a transaction.

📌 Project Workflow
1. 🧹 Data Cleaning
Removed missing Customer IDs

Filtered cancelled invoices

Removed inconsistent and logically incorrect entries

2. 🏗️ Feature Engineering
Created meaningful features including:

Total_amount = Quantity × Price

Purchaseday and PurchaseHour extracted from InvoiceDate

Aggregated invoice-level data for RFM analysis

3. 📊 Exploratory Data Analysis (EDA)
Visualized:

Sales trends across weekdays and hours

Top customers and countries by purchase value

Purchase frequency vs total spend

Customer behavior segmentation using RFM

4. 📈 Outlier Detection
Used IQR method to detect high-frequency or high-purchase outliers

Separated outliers to treat them as VIP customers

5. ⚙️ Scaling and Clustering
Applied StandardScaler to scale RFM data

Used Elbow method and Silhouette Score to find optimal k

Applied K-Means clustering to segment customers

6. 🧠 Cluster Interpretation
Segmented customers into 4 clusters:

🔴 Occasional Low Spenders

🟡 Moderate Regular Customers

🟢 Valuable Loyal Customers

👑 Top VIP Customers

7. 📢 Retention Strategies
Developed tailored marketing strategies for each cluster, such as:

Welcome offers for new/occasional users

Loyalty rewards for frequent buyers

Exclusive perks for VIPs

📌 Key Tools & Libraries
Python

pandas, numpy for data processing

matplotlib, seaborn for visualization

scikit-learn for scaling and clustering

📊 Results & Insights
Most purchases occurred between 11 AM – 2 PM

Tuesday was the best-performing sales day

Small portion of VIP customers drove most revenue

Cluster segmentation helped identify different customer behaviors for better targeting
