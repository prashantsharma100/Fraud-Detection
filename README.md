**Fraud Detection SQL**

**Background :**

Fraud detection is critical in various sectors, from small businesses to large corporations. Although modern technologies like machine learning and AI are evolving, strong data analytics remains essential for identifying unusual transactions. This project applies SQL skills to analyze historical credit card transactions to detect potential fraud.

**Objectives :**
The project involves three primary tasks:

**Data Modeling:** Design a database model to store credit card transaction data and create a PostgreSQL database.

**Data Engineering:** Establish a database schema in PostgreSQL and populate it with data from provided CSV files.

**Data Analysis:** Perform data analysis to identify potentially fraudulent transactions.

**Query Files:**

**schema.sql:** Contains the SQL schema for database creation.

**seed.sql:** Contains SQL statements for populating the database with initial data.

**CSV Files**

card_holder.csv
credit_card.csv
merchant_category.csv
merchant.csv
transaction.csv

**Data Modeling:**

**Entity Relationship Diagram (ERD):** Created by inspecting the provided CSV files. The credit_card table uses VARCHAR(20) for the card column rather than INT.

**ERD Tool:** Quick Database Diagrams

**Data Engineering**
**Schema Creation:** Developed a database schema for each table and defined relationships, data types, primary keys, and foreign keys.

**Data Import:** Populated the database using the provided CSV files.

**Data Analysis**
With the data prepared, the following analyses were conducted to identify fraudulent transactions:

Top 100 Transactions Early Morning: Analyzed transactions between 7:00 to 9:00 AM to find high-value transactions.


Small Transaction Fraud Detection: Counted transactions under $2.00 to detect potential card hacking.

Top 5 Merchants with Small Transactions: Identified merchants frequently associated with small transactions.

Fraudulent Transaction Reports: Created reports for the top two customers based on cardholder IDs 2 and 18.



**Observation**: ID Holder 2 makes numerous small transactions, indicating higher susceptibility to fraud compared to ID Holder 18.

Anomalous Transactions for Corporate Credit Card: Investigated suspected unauthorized transactions in Q1 2018 for cardholder ID 25.


**Observation**: Noted fraudulent transactions in the Restaurant & Food Truck category, with significant outliers.

**Challenge :**
Outlier Detection:

Standard Deviation Method: Identified anomalous transactions based on standard deviation.


Interquartile Range (IQR) Method: Used IQR to detect outliers.


This README outlines the structure and findings of the Fraud Detection SQL project. For further details, refer to the SQL files and CSV data provided.
