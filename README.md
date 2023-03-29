# Market-Segmentation
This project involves segmenting customers based on their purchase behavior using K-means algorithm. 
The aim of this project is to provide insights into customer behavior and help businesses tailor their marketing strategies to better meet the needs of their customers.

## Data
The data used in this project was collected from an E-commerce platform and includes those variables : 

* InvoiceNo: The unique identifier of each customer invoice.

* StockCode: The unique identifier of each item in stock.

* Description: The item purchased by the customer.

* Quantity: The number of each item purchased by a customer in a single invoice.

* InvoiceDate: The purchase date.

* UnitPrice: Price of one unit of each item.

* CustomerID: Unique identifier assigned to each user.

* Country: The country from where the purchase was made.

### Using the customer buying behavior features “Quantity”, “InvoiceDate” and “UnitPrice, we are going to derive a customer’s RFM profile - Recency, Frequency, Monetary Value.

## Steps 

- Data cleaning and preparation: The data was cleaned and prepared for analysis, including removing missing values, outliers, and scaling the data.

- Segmentation: The K-means algorithm was used to segment customers based on their purchase behavior. The algorithm groups customers with similar buying patterns and assigns them to different clusters.

- Cluster profiling: The characteristics of each cluster, such as the average purchase amount, frequency, and recency of purchases, were analyzed to identify meaningful segments.

- Interpretation and Visualization: The findings of the segmentation were used to tailor marketing campaigns and offerings to the different customer segments.

# Requirements

Pandas (pip install pandas)

seaborn (pip install seaborn)

Matplotlib (pip install matplotlib)

scipy (pip install scipy)

Scikit-learn (pip install sklearn)

plotly (pip install plotly)


#  Insights 

This project provides valuable insights into customer behavior and can help businesses tailor their marketing strategies to better meet the needs of their customers.

We have 4 clusters : 

- **cluster 0** : This cluster includes customers with low recency, frequency and monetary value scores . These are people who have made only a few purchases and have not been active in recent periods.

- **cluster 1** : This cluster groups customers with medium recency, high frequency, and low monetary value scores . These are people who make frequent purchases of lower-priced items.

- **cluster 2** : This cluster includes customers with medium recency, medium frequency, and high monetary value scores . These are people who make regular purchases of higher-priced items.

- **cluster 3** : This cluster groups customers with high recency, medium frequency, and low monetary value scores. These are people who haven't made a purchase recently, but when they do, they tend to buy less expensive items.

## The table below presents some strategies that can be made for each cluster

| Cluster | Description | Strategies |
|---------|-------------|------------|
| 0 | people who haven't made a purchase recently, but when they do, they tend to buy less expensive items. | Customer re-engagement strategies: It might be worth creating targeted re-engagement strategies to encourage them to return. These strategies could include personalized email campaigns, targeted promotions, or incentives to come back and shop.<br>- Understanding the reasons for inactivity: It's important to understand why this cluster has not been active. This could be due to a variety of reasons, such as a poor shopping experience, a lack of interest in the products, or simply forgetting about the brand. By understanding these reasons, we can develop strategies to address them and encourage customers to come back.<br>- Identifying product gaps: This cluster's low monetary value might indicate that they have not yet found products that they are interested in. By analyzing their purchase history, it's possible to identify product gaps and develop new product lines or promotions that might better meet their needs.  |
| 1 | People who make regular purchases of higher-priced items | - Targeted promotions: Since this cluster tends to purchase lower-priced items, it might be worth creating targeted promotions to encourage them to make additional purchases. These promotions could focus on complementary items that are in the same price range as their previous purchases or provide incentives to encourage them to spend more.<br>- Upsell opportunities: While this cluster tends to buy lower-priced items, there may still be opportunities to upsell them to higher-priced items that are within their budget.|
| 2 | People who make frequent purchases of lower-priced items. | - Targeted marketing campaigns: It might be worth creating targeted marketing campaigns to keep them engaged and encourage them to make even more purchases. The campaigns could highlight products that are complementary to their previous purchases or provide exclusive discounts to incentivize them to shop more.<br>- Customer loyalty programs: creating a loyalty program could be a way to retain these customers and encourage them to make more frequent purchases. The program could offer rewards such as exclusive discounts, early access to new products, or free shipping.<br>- Product recommendations: By analyzing the types of products that this cluster tends to buy, it's possible to identify related or complementary products that they might be interested in.  |
| 3 | People who haven't made a purchase recently, but when they do, they tend to buy less expensive items. | - Targeted promotions: Since these customers haven't made a purchase recently, it might be worthwhile to send them targeted promotions to encourage them to come back and make a purchase. The promotions could focus on lower-priced items that are more likely to appeal to this group.<br>- Upsell opportunities: While this cluster tends to buy less expensive items, there may still be opportunities to upsell them to higher-priced items that are within their budget. By understanding what items this cluster tends to buy, we can identify related products that might be a good fit for them.|
