🧩 Customer Segmentation & Recommendation System
📘Project Overview

This project analyzes Flipkart-like sales transaction data to segment customers based on their purchase behavior and recommend products using cluster-based logic.
It applies data preprocessing, exploratory data analysis (EDA), K-Means clustering, and a basic recommendation engine to extract meaningful business insights.

🎯 Objectives

Clean and preprocess raw transaction data
Analyze customer purchase behavior and spending trends
Segment customers using K-Means clustering
Visualize customer clusters and spending patterns
Build a recommendation system based on cluster membership
Generate detailed visual and PDF reports

📂 Project Structure

Customer_Segmentation_Recommendation_System/
    1.data/
        ├── expand_sample_transactions.csv           
    2.images/
      ├── Elbow Curve.png                   ├── customer_segmentation.png         
      ├── Cluster_Spending_Distribution.png 
    3.code/
      ├── customer_segmentation_starter.ipynb  
    4.reports
      ├── Customer_Segmentation_Report_Manasa.pdf  
     5.README.md 

🧾 Dataset Description

| Column Name        | Description                                   |
| ------------------ | --------------------------------------------- |
| **CustomerID**     | Unique ID for each customer                   |
| **ProductID**      | Unique ID for each product                    |
| **Category**       | Product category (e.g., Electronics, Fashion) |
| **PurchaseAmount** | Amount spent per transaction                  |
| **PurchaseDate**   | Date of transaction                           |


🧩 Workflow Steps

1️⃣ Data Preprocessing

-Loaded the Flipkart transaction dataset.

-Handled missing values and ensured correct data types.

-Converted PurchaseDate to datetime format.

-Removed duplicate transactions if any.

2️⃣ Feature Engineering

-Generated customer-level metrics from transaction data:

-TotalSpend – Total amount spent by each customer.

-AvgSpend – Average spend per transaction.

-PurchaseFrequency – Number of purchases per customer.

-PreferredCategory – Most frequent category purchased.

3️⃣ Exploratory Data Analysis (EDA)

-Distribution plots for Total Spend and Purchase Frequency.

-Pairplots and correlation heatmaps for relationship analysis.

-Boxplots to identify potential outliers.

4️⃣ Clustering

-Scaled numerical data using StandardScaler.

-Used the Elbow Method to determine the optimal number of clusters.

-Applied K-Means Clustering to group customers based on their purchasing patterns.

5️⃣ Cluster Profiling

-Each cluster was analyzed to understand:

-Average total spend.

-Purchase frequency.

-Number of customers in each segment.

6️⃣ Recommendation System

-Built a simple rule-based recommendation system that:

-Identifies a customer's cluster.

-Recommends the top products purchased by other customers in the same segment.

🧠 Technologies Used

Python 🐍

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

Jupyter Notebook


📈 Key Visualizations

   Visualization	                              Purpose
Elbow Curve                     -        Determines optimal number of clusters
Customer Segmentation Plot      -        Shows spending & frequency clusters
Cluster Spending Distribution   -        Visual comparison of spending by group


 🧾 Results Summary

Customers were segmented into 2 main clusters:

Cluster 0: Moderate spenders

Cluster 1: High-value customers

Recommendations are made based on cluster-level top products.

🧰 How to Run

1.Clone this repository
git clone https://github.com/your-username/Customer_Segmentation_Recommendation_System.git

2.Navigate to the code directory
cd Customer_Segmentation_Recommendation_System/code

3.Open the notebook
jupyter notebook customer_segmentation_starter.ipynb
 
4.Run all cells sequentially to generate results and visuals.



                          


