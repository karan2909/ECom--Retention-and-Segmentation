# ECom--Retention-and-Segmentation

## 1) Dataset
- Dataset: [Ecommerce Data](https://www.kaggle.com/datasets/carrie1/ecommerce-data/code?datasetId=1985&sortBy=voteCount)
- Description: Transaction data for an ecommerce online store selling gift items from 2010 to 2011.

## 2) EDA
- Almost 90-95% of the sales are happening from the UK.
- There are customers who are buying in bulk from the website, suggesting they might be wholesalers.
- CustomerID is missing for 25% of the data.
- Most of the sales data is from 2011 (92%), and the rest is from 2010 (8%).
- There are no sales on Saturdays, suggesting the store would be closed.
- There are outliers in quantity at both tail ends, also negative quantity suggesting there is a provision of return back to the store.
- Sales have an upward trend, with an exception being the most recent December month as data has only 9 days of records, which is inconclusive of entire month sales.

## 3) Feature Engineering
- RFM Features: Recency, Tenure, Frequency, Monetary.
- Product Diversity: Number of Products Purchased.
- Behavioral Features: Average Days Between Purchases, Favorite Day for Shopping.
- Geographical Features: Is from UK or not.
- Cancellation Features: Canceled Flag, Number of canceled orders.

## 4) Retention
![Retention Plot](Retention_Plot.png)

## 5) Customer Segmentation - Heuristic and Kmeans
Customers are segmented into different clusters based on:
- Recency: How recently they did the transaction.
- Frequency: How often the customers are doing transactions.
- Monetary: Average Order Value per customer basket.

![Segmentation](Segmentation.png)

![RFM Segmentation](RFM_segmentation.png)
