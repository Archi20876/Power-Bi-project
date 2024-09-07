# Superstore Sales Analysis
![Screenshot 2024-09-07 101304](https://github.com/user-attachments/assets/46fc9673-9268-4835-836f-7756f2299e48)
![Screenshot 2024-09-07 185428](https://github.com/user-attachments/assets/056cf551-52f3-4019-b83c-e975450e88a0)



## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources) 
- [Bussiness Analytics Q/A](#bussiness-analytics-Q/A)
- [Recommendations](#recommendations)

### Project Overview
---

This data analysis project aims to provide insights into the sales performance of an e-commerce company over the past year. By analyzing various aspects of the sales data, we seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the company's performance.

### Data Sources

Sales Data: The primary dataset used for this analysis is the "[SuperStore_Sales_Dataset(1).csv](https://1drv.ms/x/c/64CA0463A0426356/ETvpUelP8XVOmBqvPpor-G0BzYsxBiaT7V6-TqQb8Il47w?e=YXC1YY)" file, containing detailed information about each sale made by the superstore.

### Tools

- Excel - Data Cleaning
  - [Download here](https://1drv.ms/x/c/64CA0463A0426356/Eb3Crys1GZdFrbnJrZCwFKIB7YTT2L_TeDoaN3Wkm6HQlw?e=q6Uxyz) [Cleaned Dataset]
- PowerBI - Data Analysis & Creating Report
  - [Dashboard_link](https://app.powerbi.com/groups/me/reports/3763a026-5f03-47b5-ab34-6e0fb7983da0/9ae2ce62761ec1c9213e?experience=power-bi)


### Data Cleaning/Preparation

In the initial data preparation phase, we performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Performed DAX Query.
4. Data cleaning and formatting.
   

### Bussiness Analysis Q/A
---

In this project, We utilized Power BI to analyze and visualize sales data, addressing key business questions and answers such as:

- Who is the Top Customer by revenue?
  ##### Jamora Chand , Customer ID = TC-20980
- Which Products Or Categories generating the highest revenue?
  ##### Technology , Product ID = TEC-CO-10004722
- Are there any customer segment that are outperforming?
  ##### 1.Segment
  ##### 2.Consumer
  ##### 3.Corporate
  ##### 4.Home Office
- Which Product having highest order sale?
  #####  California
- Which product has the lowest sale?
  ##### Avery Durable Slant Ring Binders With Label Holder, Product ID = OFF-BI-10003727
- Was there any anomalies in the sales?
  ##### Sum of Sales was unexpectedly high on Friday, December 25, 2020. It had a value of 9721.93, which is outside the expected range of 8076.68-9665.15.
- In which region the anomalies were seen?
  ##### Sum of Sales for Region South was unusually high, which may have lifted the Sum of Sales total.
- What are the Trends that can be seen from Forecast?
  ##### Sum of Sales trended up between Thursday, August 13, 2020 and Tuesday, September 22, 2020 with a rise of 5769.05.
- What might be the reason for the upward trend?
  ##### 'Second Class' accounted for the majority of the increase among Ship Mode , offsetting the decrease of 'Standard Class'. The relative contributions made by 'Second Class' and 'Standard Class' changed the most.
  


### Recommendations
---

Based on the analysis, we recommend the following actions:
- Invest in marketing and promotions during peak sales seasons to maximize revenue.
- If certain products consistently have low stock levels or stock-outs, it might indicate a need for better inventory management.
- Analyze the specific needs and preferences of the Consumer, Corporate, and Home Office segments. Introduce new products or services that align with their demands, potentially creating new revenue streams.
- "Avery Durable Slant Ring Binders With Label Holder" (Product ID: OFF-BI-10003727) has low sales but if we offer the binder as part of a bundle with other office supplies, such as dividers, sheet protectors, or paper. Bundling can encourage customers to purchase multiple items together, increasing overall sales.
- Review the product mix available in these regions. Introduce products that align better with the needs of the local market or withdraw items that don’t resonate with customers in those areas.
  

### Limitations
---

I had to remove all zero values from budget and revenue columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both budget and number of votes with revenue.

😊😊😊


