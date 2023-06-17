# Maven-Market-Project

### Background


Maven Market is a fictional multi-national grocery chain with locations in Canada, Mexico and the United States.

The management team needs a way to track KPIs (sales, revenue, profit, returns), compare regional performance, and identify high-value customers. All you’ve been given is a folder of raw csv files, which contains information about transactions, returns, products, customers, and sales territories.


### Steps I went through
#### 1. Connect and transform the raw data using Power Query
This include: 
* Ensured all the data types are correct
* Created customers' full name by merging the "first name" & "last name" columns in **_Customers_** table
* Replaced null values with zeros in "recyclable" & "low-fat" columns in **_Products_** table
* Generated start of month, start of quarter and year through a list of date in **_Calendar_** table

#### 2. Build a relational data model
This include:
* Identified primary keys and foreign keys in each table
* Connected the tables via the keys to construct star & snowflake schema
* Ensured the filters are one-way filters
* Hided all the foreign keys in the table to prevent invalid filter context

#### 3. Create calculated columns and measures with DAX
This include:
* Added price tiers for the products listed in **_Products_** table
* Created measures to calculate price, cost, profit, profit margin, number of transactions and return rates.

#### 4. Design an interactive dashboard to visualize the data



_(Data Source: Microsoft Power BI Desktop for Business Intelligence (2023) in Udemy)_
