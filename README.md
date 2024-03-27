# Retail-Star-Schema-DataWarehouse-ETL-Using-DataStage
# Project Overview:
Our scenario assumes a fictitious national department store which decides to build a star-
schema based sales analysis data warehouse with the dimensions of customer, store and  product 
using IBM InfoSphere DataStage then build ETL pipelines to create retail data mart to perform analysis on it.
The requirement is to capture versions the changes of dimensions in the star-schema data warehouse 
in order to deliver accurate results.
# Project Setup
1) Install IBM InfoSphere DataStage.
2) Create the necessary job sequences and stages as per the provided requirements.
3) Execute the DataStage jobs to perform ETL processes.
You can import my jobs and run them in your project.
# Data Source 
The data source for the star-schema is an OLTP system.

![Capture](https://github.com/israa-aly/Retail-Star-Schema-DataWarehouse-ETL-Using-DataStage/assets/68852141/ef48039a-d9f2-40cd-bd2a-b83067a4131a)
# Project Requirements 
1) Need data mart that display each transaction for each customer based on
type of customer “citizen” or “foreign” with information of it information of
product and information of stock which buy with name file
“RETAIL_DATA_MART” with transformation upper case of all customer name
column
2) based on question 1 read data mart “ACTIVATIONSALES_DATA_MART”
Then answer the following business need:
• Display count of all transaction for each employee for each store
• Display max profit made by which customer type.
Illustrate: customer type “foreign” make 5 transactions
, customer type “citizen” makes 3 transactions.
So, max profit made by foreign customers.
Named DataMart “ACTIVATIONSALES_DATA_MART”
• Based on which customer make profit , give them Bouns
Equation = Annual_Incomek$* SpendingScore*100

# Steps 
# 1) Building the star-schema model 
we have three dimensions product, retail, customer , fact table “transactions”.

![Capture](https://github.com/israa-aly/Retail-Star-Schema-DataWarehouse-ETL-Using-DataStage/assets/68852141/d75ae7ef-53c1-4617-ab23-05505bde72f0)
# 2) ETL (Extract,Transform and Load )
1) Extraction:
   Extract The data from the data source (files at the dataset folder or  using database)
2) Transformation:
   perform transformations on the data as needed to meet the business needs.
   Such as :
   - Filter the customer type to include only("citizen" or "foriegn" )
   - transform the customer name to uppercase
3) Loading:
 load the transformed data into Retail_Data_Mart
# 3) Analysis on the Retail_Data_Mart

# Job 1
![Q1](https://github.com/israa-aly/Retail-Star-Schema-ETL-Project-Using-DataStage/assets/68852141/5476a09f-780f-461d-9b0e-ddd80fcea980)
# Job 2
![Q2](https://github.com/israa-aly/Retail-Star-Schema-DataWarehouse-ETL-Using-DataStage/assets/68852141/b522a3d2-5d01-4444-a84c-6ba825d5ba7c)






   
