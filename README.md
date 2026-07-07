# VisualizationTableu_Olistdataset

This project is to make Dashboard View for Olist E-Commerce in 2018 dataset

## Data Resource
The data resource is collected from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

## Data Preprocessing

Step for Preprocessing :
- Checking the missing values
- checcking the duplicated data
- relating data form a view Sheet

## Preparation for dashboard
### 1. Making KPI - Revenuew Worksheet
<img width="816" height="401" alt="image" src="https://github.com/user-attachments/assets/403f0830-c4e5-4591-9907-04bda19146e5" />

We can use a calculated field and we add the formula with payment value from Order_Payments
```
SUM([Payment Value])
```
### 2,Making KPI - Order Worksheet
<img width="741" height="362" alt="image" src="https://github.com/user-attachments/assets/198eba88-f820-439c-88e0-9862a4e09def" />

We can use a calculated field and we add the formula with Order Id from Orders
```
COUNT([Order Id])
```
### 3.Making KPI - Customer Worksheet
<img width="604" height="361" alt="image" src="https://github.com/user-attachments/assets/f0c21199-9603-44e3-bc44-80c1fd574a3f" />

We can use a calculated field and we add the formula with Customer Id from Customers
```
COUNTD([Customer Id])
```
### 4.Making BarChart for Top 10 Sellers
<img width="1694" height="945" alt="image" src="https://github.com/user-attachments/assets/4827a980-5ec3-45b5-bbea-c99827c4036d" />

We can add a SUM(Payment Value) in Coloumns and seller id as a Rows

### 5.Making LineChart for Monthly Revenue Trend
<img width="1675" height="938" alt="image" src="https://github.com/user-attachments/assets/690eb523-e265-4760-92ce-46f0f7d8c2ea" />

We can add Order Purchases Timestamp form Orders to coloumns don`t forget to sort by month after that we can add Total Revenue to Rows

### 6.Making Filled Map for Revenue by Location
<img width="1462" height="945" alt="image" src="https://github.com/user-attachments/assets/8c72d161-22db-4975-9839-e387e2afc4b1" />

We can add Longitude as a coloumns and Latitude as a rows after that we add the Total Revenue to Color and Customer State to Detail

### 7.Making Barchart for Top 10 Customer Sellest
<img width="1304" height="883" alt="image" src="https://github.com/user-attachments/assets/cfc27d02-4250-4498-a9a4-7817a8302a86" />

Wecan add Customer id to cloumns and Total Revenue to Rows

### 8.Making Barchart for Payment Type Percentage
<img width="1299" height="873" alt="image" src="https://github.com/user-attachments/assets/dcf51512-d787-4960-ba20-33784f237749" />

We can add formula at coloumns
```
COUNTD([Order Id]) / TOTAL(COUNTD([Order Id]))
```
At the rows we add Payment Type

## Final Look
<img width="1861" height="989" alt="image" src="https://github.com/user-attachments/assets/e7ec5b3e-d14a-4347-a5bb-63d34ec55ce3" />



