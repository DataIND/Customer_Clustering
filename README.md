# Sales Data Analysis
This project analyzes sales transaction data using time series forecasting and KMeans clustering algorithms. The dataset contains information about various products sold, including their descriptions, quantities, prices, and customer details.


Dataset Overview
The dataset consists of the following columns:

  -InvoiceNo: Unique identifier for each invoice
  -StockCode: Unique identifier for each product
  -Description: Description of the product
  -Quantity: Number of items sold
  -InvoiceDate: Date and time of the transaction
  -UnitPrice: Price per unit of the product
  -CustomerID: Unique identifier for each customer
  -Country: Country of the customer


Analysis Techniques :- 
1] Time Series Forecasting
  -Observed: The actual sales data over time.
  -Trend: The long-term progression of the series, showing the overall direction of sales.
  -Seasonal: The repeating patterns or cycles in the sales data, indicating seasonal effects.
  -Residual: The remaining noise after removing the trend and seasonal components, which can help identify anomalies.

2] KMeans Clustering Analysis :- 
  - Data Preparation :- We start by selecting the relevant features for clustering: Recency, Frequency, and Monetary value (though it appears "Frequency" is duplicated in your code). We then scale these features      to ensure that they contribute equally to the distance calculations in KMeans.
  - KMeans Clustering and Elbow Method :- We apply the KMeans algorithm for a range of cluster numbers (from 1 to 9) and calculate the Sum of Squared Errors (SSE) for each clustering result. The SSE measures how      tightly the clusters are packed.
  - Interpretation of the Elbow Method:- The elbow method involves plotting the SSE against the number of clusters. The point where the curve starts to flatten (the "elbow") indicates the optimal number of            clusters. This point represents a balance between having a low SSE and a manageable number of clusters.

