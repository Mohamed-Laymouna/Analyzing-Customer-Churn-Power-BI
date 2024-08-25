
# Analyzing Customer Churn in Power B
<a name="top"></a>
## Table of Contents
- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Data Overview](#data-overview)

- [Project Steps](#project-Steps)
  - [1. Data Import and Exploration](#1-data-import-and-exploration)
  - [2. Churn Rate Calculation](#2-churn-rate-calculation)
  - [3. Analysis of Churn Reasons and Categories](#3-analysis-of-churn-reasons-and-categories)
  - [4. Geographic Analysis](#4-geographic-analysis)
  - [5. Demographics Analysis](#5-demographics-analysis)
  - [6. Contract and Group Analysis](#6-contract-and-group-analysis)
  - [7. Plan Analysis](#7-plan-analysis)
  - [8. Report Building](#8-report-building)
- [Key Insights Discovered](#key-insights-discovered)
- [Actionable Insights and Recommendations](#actionable-insights-and-recommendations)
- [Skills Acquired](#skills-acquired)
- [How to Run This Project](#how-to-run-this-project)
- [Tools Used](#tools-used)
- [Visual Report](#Visual-Report)
- [Conclusion](#conclusion)

## Overview 

This project focuses on analyzing customer churn for a fictitious telecom provider, Databel. The goal is to discover why customers are churning and to provide actionable insights to reduce churn. The analysis is performed using Power BI, leveraging a dataset containing 29 columns of customer information, demographics, contract details, subscription types, and charges.

## Problem Statement

Databel has identified that the overall churn rate is approximately 27%, with a significant portion of churn attributed to competitor actions and a notably high churn rate in California. The aim is to delve deeper into the data to understand the underlying factors contributing to churn and to develop strategies for customer retention.

## Data Overview

The dataset used in this project is a snapshot of Databel's customer database at a specific moment in time. It contains 29 columns and one row per customer, including information on customer status, demographics, contract details, subscription types, and charges.

### Key Columns:
- **Customer ID:** Unique identifier for each customer.
- **Churn Label:** Indicates if a customer churned ("Yes" or "No").
- **Churn Reason:** Specific reason for churn.
- **Churn Category:** Grouped categories for churn reasons.
- **Under 30:** Indicates if a customer is under 30 years old.
- **Senior:** Indicates if a customer is 65 or older.
- **Age:** Age of the customer.
- **Gender:** Gender of the customer.
- **State:** State code where the customer resides.
- **Payment Method:** Preferred payment method.
- **Contract Type:** Type of contract (Month-to-Month, One Year, Two Year).
- **Account Length:** Duration of the customer's account in months.
- **Monthly Charges:** Average monthly charges to the customer.
- **Total Charges:** Sum of all charges.




## Project Steps
[Return to Top](#top)
### 1. Data Import and Exploration
- **Data Import**: Loaded the dataset into Power BI and performed initial data checks.
- **Data Validation**: Ensured no duplicate customer records by comparing the count of customer IDs with unique customer IDs.

### 2. Churn Rate Calculation
- **Churn Label Conversion**: Converted the "Churn Label" column into a binary format for easier analysis.
- **Churn Rate Measure**: Created a measure to calculate the overall churn rate.

### 3. Analysis of Churn Reasons and Categories
- **Reasons Analysis**: Visualized churn reasons in descending order using a column chart.
- **Categories Analysis**: Grouped churn reasons into broader categories and displayed them in a bar chart.

### 4. Geographic Analysis
- **Churn by State**: Used a map visualization to explore churn rates across different states, including the total number of customers per state.

### 5. Demographics Analysis
- **Age Bins**: Created age bins to analyze the relationship between age groups and churn rate using a combo chart.
- **Demographic Patterns**: Investigated churn patterns across different demographic categories.

### 6. Contract and Group Analysis
- **Contract Type**: Used the SWITCH function to categorize contract types into "Monthly" and "Yearly" for churn analysis.
- **Group vs. Individual**: Analyzed the impact of group contracts on average monthly charges and churn rates.

### 7. Plan Analysis
- **Unlimited Data Plan**: Investigated the churn rate among customers with and without unlimited data plans.
- **International Calls Plan**: Analyzed the churn rate and activity levels of customers with an international calls plan.

### 8. Report Building
- **Overview Page**: Summarized key insights with visualizations of churn rates by state, contract type, and demographic categories.
- **Demographic and Group Analysis**: Developed a dedicated page for age and group-related insights, with dynamic filters for interactivity.
- **Contract and Payment Analysis**: Created a scatter plot and card visuals to analyze the relationship between contract type, payment method, and customer service calls.

## Key Insights Discovered
[Return to Top](#top)
1. **Churn Rate**: The overall churn rate for Databel is around 27%.
2. **Competitor Influence**: Approximately 45% of the churn is related to competitor activities.
3. **Geographic Insights**: California exhibits an abnormally high churn rate of over 60%.
4. **Demographics**: Senior customers have a higher churn rate (~38%) compared to the average. The churn rate increases with age.
5. **Group Contracts**: Customers in group contracts have lower average monthly charges compared to those in individual contracts, and lower Churn rate 6.5%.
6. **Contract Type**: The churn rate for customers on monthly contracts is significantly higher (46.29%) compared to those on yearly contracts (6.6%).
7. **Unlimited Data Plan**: Customers with an unlimited data plan exhibit a higher churn rate, after further investigation i found that customers who have unlimited data plan and use less than 5 GB are more likly to Churn.
8. **International Plan**: Customers with an international calls plan and are not actively using international calls have a churn rate of 71%, often due to inactivity in making international calls.
9. **Average Account Lenth**: As the average account increase, the curn rate decrease.
## Actionable Insights and Recommendations
[Return to Top](#top)
1. **Target High-Risk Demographics**:
   - **Senior Customers**: Given the higher churn rate among senior customers, targeted retention campaigns should be developed. Consider offering personalized plans or discounts to this demographic.
   - **Age-Based Offers**: Since churn increases with age, consider segmenting customers into age brackets and creating tailored offers or loyalty programs for different age groups.

2. **Optimize Group Contracts**:
   - **Promote Group Plans**: The lower churn rate among customers in group contracts suggests that promoting these plans could be beneficial. Marketing campaigns could emphasize the cost savings and other benefits of group contracts.
   - **Analyze Group Dynamics**: Further analysis could be conducted to understand the group dynamics and identify opportunities to convert individual customers to group plans.

3. **Review and Adjust Monthly Contracts**:
   - **Incentivize Yearly Contracts**: Since monthly contracts have a much higher churn rate, consider incentivizing customers to switch to yearly contracts with discounts, added benefits, or other perks.
   - **Review Monthly Contract Terms**: Evaluate the terms and conditions of monthly contracts to identify any factors contributing to the high churn rate. Adjustments could be made to improve customer retention.

4. **Investigate Unlimited Data Plan Usage**:
   - **Data Usage Analysis**: Conduct a detailed analysis of data usage patterns among customers with unlimited data plans. Identify if there are specific usage patterns associated with higher churn.
   - **Personalized Plan Recommendations**: Consider offering personalized data plans based on usage patterns to reduce churn among unlimited data plan customers.

5. **Engage with International Plan Customers**:
   - **Propose Plan Downgrades**: Contact customers on an international plan who are not making international calls and propose they downgrade to a cheaper plan. This could increase customer satisfaction and reduce churn.
   - **Educate Customers**: Develop educational content or campaigns to ensure customers fully understand the benefits and costs associated with their international plans, helping them make informed decisions.

6. **Address Competitor Influence**:
   - **Competitor Analysis**: Conduct a detailed competitor analysis to understand what promotions or offers are leading to customer churn. Adjust Databel’s offerings to be more competitive in the market.
   - **Win-Back Campaigns**: Develop targeted win-back campaigns aimed at customers who have churned due to competitors, offering them exclusive deals or incentives to return.


## Skills Acquired
[Return to Top](#top)
- **Data Analysis**: Developed strong analytical skills, including data validation, data transformation, and creating meaningful insights from raw data.
- **Power BI Proficiency**: Gained expertise in using Power BI for data visualization, including creating measures, calculated columns, and interactive dashboards.
- **Data Storytelling**: Learned how to craft a compelling narrative using data, ensuring insights are clearly communicated to stakeholders.
- **Problem-Solving**: Enhanced problem-solving skills by identifying key factors contributing to customer churn and proposing actionable solutions.
- **Business Acumen**: Improved understanding of business processes, particularly in customer retention and churn management.

## How to Run This Project

1. **Download the Dataset**: Ensure you have the dataset loaded into Power BI.
2. **Follow the Steps**: Proceed through the analysis steps as outlined in the approach section.
3. **Generate Insights**: Use the insights and visualizations created to understand customer churn and propose actionable recommendations.

## Tools Used

- **Power BI**: For data visualization and analysis.
- **Microsoft Excel**: (Optional) For any preliminary data cleaning or exploration.


### Visual Report
- **Overview Page**
  ![image](https://github.com/user-attachments/assets/94d503cb-ccb9-4e43-a3cc-3a8cf50ce8aa)


- **Demographic and Group Analysis**
  ![image](https://github.com/user-attachments/assets/3ec414c8-5ee5-4048-8aba-44d4e3e325c2)


- **Payment and Contract Analysis** 
 ![image](https://github.com/user-attachments/assets/27bdaeba-dde7-487b-b80f-aca977f7c15a)




## Conclusion

This project provides a comprehensive analysis of customer churn for Databel, offering deep insights into the factors driving churn and actionable recommendations for reducing it. The Power BI report created serves as a powerful tool for stakeholders to understand and address churn effectively.


## Acknowledgements

Special thanks to the creators of the fictitious Databel dataset and to all who contributed to the development and testing of this project.

