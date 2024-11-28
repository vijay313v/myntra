# Myntra Online Retail Customer Segmentation

![rainbow](https://user-images.githubusercontent.com/85065799/204543278-26c507b6-400a-42e0-852f-2e09362f6e12.png)

### <b>Problem statement:</b>
Myntra is a leading Indian fashion e-commerce company known for its wide range of clothing, accessories, and lifestyle products. While Myntra is recognized primarily for fashion, this dataset relates to the company's online retail operations for Myntra Gifts Ltd., a UK-based division specializing in unique all-occasion giftware. This dataset spans transactions from December 1, 2009, to December 9, 2011, and includes detailed records of sales made through Myntra Gifts Ltd.’s non-store online platform. The dataset provides a thorough snapshot of the company's international online retail activities during this period.

![rainbow](https://user-images.githubusercontent.com/85065799/204543278-26c507b6-400a-42e0-852f-2e09362f6e12.png)

### <b>Data description </b>

* InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
* StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
* Description: Product (item) name. Nominal.
* Quantity: The quantities of each product (item) per transaction. Numeric.
* InvoiceDate: Invice Date and time. Numeric, the day and time when each transaction was generated.
* UnitPrice: Unit price. Numeric, Product price per unit in sterling.
* CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
* Country: Country name. Nominal, the name of the country where each customer resides.

![rainbow](https://user-images.githubusercontent.com/85065799/204543278-26c507b6-400a-42e0-852f-2e09362f6e12.png)

### <b>Business context of the problem:</b>

#### <b>Customer Segmentation:</b>
Customer segmentation is the process by which you divide your customers up based on common characteristics so you can market to those customers more effectively.

![pic2](https://user-images.githubusercontent.com/85065799/204151765-54a15ea0-b073-4746-abd9-4b95fa685312.jpg)

#### <b>Different ways of segmentation:</b>

1. Demographic segmentation.
2. Behavioral segmentation.
3. Geographic segmentaion.
4. Needs based segmentation.
  
  and many more... 
  
  

![pic3](https://user-images.githubusercontent.com/85065799/204151805-1648d8ea-d291-4170-bafd-05615df181ee.jpg)

<b>In this project I'll be performing Behavioral segmentation using the classical RFM model.</b>

![pic4](https://user-images.githubusercontent.com/85065799/204151812-045c09d1-300b-4d6b-9c0a-1b62b3d2df69.png)

![rainbow](https://user-images.githubusercontent.com/85065799/204543278-26c507b6-400a-42e0-852f-2e09362f6e12.png)

### <b>Project Flowchart:</b>
1. Initial preparations(Loading the dependencies and the data).

2. Data Cleaning:
   * Data Exploration.
   * Handling null values.
   * Handling duplicate values.
   * Removing Outliers.
   * Removing Cancelled orders.

3. Feature Engineering:
   * Extracting columns from the InvoiceDate column.
   * Forming the total Amount column.
  
4. EDA.

5. Forming the segmentation criteria.

6. Pre Processing the data.

7. Model implementation:
   * K Means.
   * K Means with elbow method.
   * Hierarchical clustering (Agglomerative).
   * DBScan Clustering.

![rainbow](https://user-images.githubusercontent.com/85065799/204543278-26c507b6-400a-42e0-852f-2e09362f6e12.png)

### <b>Conclusion:</b>

#### <b>EDA insights:</b>
  * The product 'White hanging heart t-light holder' is the most frequently ordered product, around 1700 times. 'Jumbo bag red retrospot' is the second most ordered product, around 1300 times.
  * The product 'Pack of 72 retrospot cake cases' has the most quantity ordered, around 15,000 units. 'Assorted colour bird ornament' is second with around 13,000 units ordered.
  * The product "Product Bunting" has made the most money, around 35,000 sterling. "White Hanging heart T-light holder" being the second, which has made around 32,000 sterling.
  * The customer with the ID: 17841 has the highest number of orders and the customer with the ID: 18118 has the lowest number of orders.
  * United Kingdom has the most orders placed, with around 3 lakh orders. Germany being second, but way less than United Kingdom.
  * Most orders are made in the 12th hour, i.e 12pm to 1pm, and the least orders are made in the 6th hour, i.e 6am to 7am.
  * The 6th day of the month has the highest number of orders and the 31st day has the lowest.
  * Most of the orders are made on Thurday,around 66 thousand, and the least number of orders are made on Friday, around 46 thousand.
  * The most number of orders are made in the 11th month, i.e December, and the least in the 2nd month, i.e February.
  
#### <b>Model implementation conclusions:</b>
  * K-Means with optimal clusters = 3 , performed best with a Silhoutte score of 0.5233813538947185 and while cluster profiling , Cluster 2 is the best cluster 
    and cluster 1 is the worst.

  * Hierarchial Clustering : Dendogram results suggests 3 clusters and while performing Agglomerative Clustering on 3 clusters got a Silhouette Score: 
   0.49581156711609203 and while cluster profiling, Cluster 1 is best cluster and cluster 0 is worst.

  * DBSCAN Clustering : No. Of Cluster got is 2 exluding NOISE, and with a Silhouette Score: 0.497433238703058
 
  

  
![rainbow](https://user-images.githubusercontent.com/85065799/204543278-26c507b6-400a-42e0-852f-2e09362f6e12.png)
