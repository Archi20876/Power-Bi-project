# Customer Churn Dashboard

### Dashboard Link : https://app.powerbi.com/links/TrBWLBo8dZ?ctid=b93ac9ba-3a71-4f45-be88-3c6f51b36180&pbi_source=linkShare
## Problem Statement

The company is facing challenges with customer retention, leading to a decline in revenue and growth. To tackle this issue, the management seeks to gain a deeper understanding of the factors driving customer churn and identify customers at risk of leaving. The objective is to leverage Power BI for analyzing historical customer data, uncovering trends, and delivering actionable insights that can help the company reduce churn rates.




### Steps followed 👇
#### Data Prepartion- Cleaning ,Formatting & Reshaping the Data.

- Step 1 : Load data into Power BI Desktop, dataset is a csv file and click on Load & Transform Data option.
- Step 2: Assign meaningful and descriptive names to each column to enhance clarity and improve the overall visualization of the Power BI report.
- Step 3: Replace the values in the "Credit Card Status" column by converting 0 to "Not Owned" and 1 to "Owned" using the "Replace Value" option.
- Step 4 : Repeat  Step 3 for Activity Status column where the 0 & 1 has been replaced with Active & Passive respectively.The same goes for Churn Status column.
- Step 5 : Click on view tab and click on  column profile and column distribution option for analyzing the column statistics.
- Step 6: Group the data by creating conditional columns for age, credit scores, and account balance using the "Conditional Column" feature found under the "Add Column" tab.
- Step 7 : Change the Data Types of columns.

#### Data Modeling- Create Queries To Model your Data for analysis and visualisation.
- Step 8 : Right-click on the "Customer Data" table, and from the drop-down menu, select the "Reference" option. This will create a duplicate of the Customer Data table, which can then be used for building the model. 
- Step 9 : Create Conditional Column  by adding conditions in each clause for Age group , Account Blance and Credit Scores (REMOVE  DUPLICATES). 
- Step 10 : In the Model view, create a model by establishing relationships with Reference tables (also known as Look Up Table) . This will help in managing and analyzing the data effectively within the model. 

#### Data Analysis- Create measures using DAX

- Step 12 : Calculate Total Customers.
 CUSTOMERS = COUNT('CUSTOMER DATA' [CUSTOMER ID])

- Step 13 : Calculate Total Customers lost.
 CUSTOMER LOST = CALCULATE(COUNT('CUSTOMER DATA'[Churn]),'CUSTOMER DATA'[Churn] = "Churned")
 
- Step 14 : Calculate Churn Rate.
 CHURN RATE = 'CUSTOMER DATA'[CUSTOMER LOST]/'CUSTOMER DATA'[CUSTOMERS]
  #### Note :- Create KPI for Total Customers  and Gauge to highlight the Target Churn Rate.

  ![Screenshot 2024-09-06 084006](https://github.com/user-attachments/assets/3b6c651b-b365-471f-9046-4c0375702cf5)




#### Data visualisation - Choosing  and formatting the visual elements.

        
- Step 15 : Create visualisation with Donut chart for analyzing the Number of Customers by gender,activity,credit card status,products and country. 
        
 - Step 16 : Create visualisation with line and stacked column chart for analyzing number of customers and churn rate by age group,credit scores group and account balance group.

 - Step 17 : Add slicer to the report which makes it more dynamic and tailored to individual preferences, enabling users to focus on the most relevant data.


 - Step 18 : Enhance the power bi report by adding filters to charts and bar chart to make the report look user-ineteractive.
  
 #### Publish the Report to Power Bi service
 ![Dashboard](https://github.com/user-attachments/assets/d707fe28-58ef-47b8-b7dc-614b615cf644)


# Insights🔍

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 10K

   Number of satisfied Customers (Male) = 3k (42.75%)

   Number of satisfied Customers (Female) = 5k (57.25%)

   Number of unsatisfied customers (Male) = 1k (44.08 %)

   Number of unsatisfied customers (Female) = 1k (55.92 %)


           
### [2] Customers by Activity
  - The churn rate is 26.9%.
  - The activity status of men are higher comapared to female by 12.78% ,having age group of 41-50 being the highest.

  ### [3] Customers by Credit card status
  
  - The credit card status is highest in France. 
  - The satisfied customers are males who has owned the credit  card.

   
 ### [4] Customers By Products
 - The satisfied customers did not buy Product 4 .
 
### [5] Customers By Country
 - The column chart is showing downfall in credit scores for France having the least churn rate of 16.6%.

 - The churn rate is almost 100% in each country with a total 2037 customers.

 
