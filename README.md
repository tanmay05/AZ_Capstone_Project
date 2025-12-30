# AZ_Capstone_Project

Project Use-case :
A third party service drops a file named orders.csv in the landing folder.
Requirement:
As soon as file arrives in landing folder, perform the following checks-
1. Check for duplicate order_id in order_status
2. Check for valid orders_status
If both the conditions are true then move the file to the staging folder else
move it to the discarded folder.

Note: In future, if the list of valid order_status changes, then we should
dynamically be able to incorporate the changes.

Services required to Implement the Solution :
1. As soon as the data is added to the storage

2. Run the Pipeline (Data Factory- trigger is a Storage Event)

3. Databricks Notebook executes the spark code to perform the necessary
   checks

Tools used :
ADLS Gen2,
Azure Databricks,
Azure DataFactory,
Azure Sql DB
