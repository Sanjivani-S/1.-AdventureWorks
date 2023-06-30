# AdventureWorks  (PowerBI Project)
##Project 1 - Adventure Works = Data taken from Microsoft sample database

Business Request :- 

A request for - executive sales report for sales managers - was raised.

Following user stories were refered

| # | As a (Role)          | I want ( request/ demand)                           | so that I ( User Value)                                          | Acceptance Criteria                                        |
|---|----------------------|-----------------------------------------------------|------------------------------------------------------------------|------------------------------------------------------------|
| 1 | Sales Manager        | A dashboard overview of internet sales              | to know highest selling products and top customers               | A dashboard that updates once a day                        |
| 2 | Sales Manager        | A dashboard overview of internet sales              | to sales over time against the budget                            | A dashboard with graphs and KPIs that compares with budget |
| 3 | Sales Representative | A detailed overview of internet sales per customers | to follow up with top customers and find out potential customers | A dashboard that filters data for each customer            |
| 4 | Sales Representative | A detailed overview of internet sales per product   | to follow up highest selling products                            | A dashboard that filters data for each product             |

### Task identified as - Generate Sales Overview Dashboard

Steps followed
1. Data cleaning and Transformation
2. Data modelling
3. Dashboard creation

Data cleaning and Transformation

From a big database, required tables were identified by referring to user stories. Using SQL queries the tables were cleaned. Here are the SQL queries used

In the above SQL statement, DimProduct table is being queried. Only required columns are selected. To get data about Product Category and Product Subcategory, left join is used on two other tables. DimProduct table will be used in the dashboard that presents product wise data.

In above SQL query, DimCustomer table is queried. Only required columns are selected. To get data about customer's location, left join is used on another table. DimCustomer table will be used in the dashboard that presents customer wise data.

 In above SQL query, DimDate table is queried. Only required columns are selected. Customer needs only last 2 years data to be considered. 

In above SQL query, FactInternetSales table is queried. Only required columns are selected. FactInternetSales table will be used in the dashboard that presents internets sales data.

Data Model :-
After identifying and cleaning required tables, they are read into PowerBI. A data model is created and relationships between different tables is defined. Budget is read and included as well.

Sales Management Dashboard
Please click following dashboard to see more reports. Thanks!

![](images/report.jpg)

