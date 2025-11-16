# Project: Customer Segmentation for E-Commerce
A data-driven approach to identifying and understanding customer personas from sales data using RFM analysis and K-Means clustering.

Project Description

This project analyzes a sample e-commerce sales dataset to identify distinct and actionable customer segments. Instead of relying on simple metrics, this analysis uses the powerful RFM (Recency, Frequency, Monetary) model to quantify and score customer purchasing behavior.

The core of the project involves a robust data preprocessing and clustering pipeline:

Data Preparation: The raw order log is cleaned, and date features are correctly formatted.

Feature Engineering (RFM): Order data is aggregated by customer to create three key metrics:

Recency: How many days ago was their last purchase?

Frequency: How many distinct orders have they made?

Monetary: What is their total lifetime spending?

Outlier Detection: The model first identifies and isolates extreme high-value outliers ("VIP Customers" or "Whales") to prevent them from skewing the main analysis.

Optimal Cluster Selection: For the remaining "normal" customer base, the Silhouette Score is used to determine the optimal number of clusters (K), providing a more robust answer than the subjective "Elbow Method."

K-Means Clustering: A K-Means model is trained on the scaled RFM data to partition the customers into these distinct groups.

Persona Analysis: The final step involves a detailed interpretation of each cluster, assigning actionable personas (e.g., "Loyal Customers," "New & Promising," "At-Risk," "Lost Customers") based on their average RFM values.

The final output provides a clear, data-driven map of the customer base, enabling the business to create targeted marketing strategies, improve retention, and maximize customer lifetime value.
