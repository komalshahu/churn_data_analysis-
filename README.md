# churn_data_analysis
This repository provides a concise analysis of customer churn using machine learning to help businesses predict churn, develop retention strategies, and enhance customer satisfaction.

## Steps Performed:
### 1. Data Exploration
    Queries were written to explore the dataset, calculate distinct values, and generate insights, such as:

    Gender Analysis: Distribution and percentage of customers by gender.
    Contract Analysis: Distribution and percentage of customers by contract type.
    Customer Revenue Analysis: Total revenue per customer status and its percentage of overall revenue.
    State Distribution: The proportion of customers by state, ranked by percentage.
  ![Screenshot (840)](https://github.com/user-attachments/assets/02e0f970-23d0-4fbc-83d4-f5671854e2f5)
  
### 2. Checking for Null and Blank Values
    A detailed query was executed to check nulls and blank values across all fields in the dataset. This step ensures the integrity of the data by identifying areas requiring data cleaning.
![Screenshot (842)](https://github.com/user-attachments/assets/5c02f489-b42f-450c-ad23-864dc2ac4dcb)
![Screenshot (843)](https://github.com/user-attachments/assets/ab85cdb4-a6fb-49b4-8a95-10e516c4cfcb)


### 3. Data Cleaning
    Null values and empty strings were handled using SQL operations:

    COALESCE and NULLIF functions replaced missing or blank values with defaults. For example:
    Missing Value_Deal → "None"
    Blank Multiple_Lines → "No"
    Blank Churn_Reason → "Others"
![Screenshot (844)](https://github.com/user-attachments/assets/302c4f06-952b-42e0-b702-8d858062d389)

### 4. Creating a Cleaned Table
    A new table, prob_churn, was created with cleaned data, ready for analysis. Fields were standardized to ensure consistency.
    
### 5. Creating Power BI Views
    To integrate with Power BI for visualization:

    vw_ChurnData: View focusing on customers with a status of "Churned" or "Stayed."
    vw_JoinData: View containing customers who recently joined with the status "Joined."
![Screenshot (845)](https://github.com/user-attachments/assets/b7d16853-540a-4033-bb61-14e152fcc676)
    
## Churn Data Analysis Dashboard
This project includes a Power BI dashboard built on SQL-processed churn data to analyze customer churn behavior. The dashboard provides comprehensive visual insights into customer retention patterns, revenue generation, churn reasons, and service usage, enabling actionable business strategies.

![project_2_P_1](https://github.com/user-attachments/assets/df3b26d3-0ee1-4d4e-9310-94960c9c859c)
![project_2_P_2](https://github.com/user-attachments/assets/a489cb8d-e74e-4cfd-a031-4eaa5f72c4b2)

Key Features of the Dashboard:
Churn Overview:

Total Customers: 6,418
Churn Rate: 26.99%
Total Churned Customers: 1,732
New Joiners: 411
Demographics and Behavioral Analysis:

Churn distribution by gender, age group, and state.
Analysis of churn rates segmented by tenure groups.
Insights into churners’ marital status.
Contract and Service Utilization Patterns:

Contract type breakdown (Month-to-Month, One Year, Two Year).
Service adoption (e.g., Internet Service, Device Protection Plans, Premium Support).
Churn Drivers:

Common reasons for churn, including service dissatisfaction, product dissatisfaction, high price, and support issues.
Detailed analysis of churn categories and customer feedback.
Payment and Financial Insights:

Churn by payment methods (e.g., Mailed Checks, Bank Withdrawals).
Revenue contribution by customer status.
Key financial indicators (Monthly Charges, Refunds, Total Revenue).
Interactive Visualizations:

Dynamic slicers to filter data by gender, state, and contract type.
Top contributors to churn categorized by services used.
Percentage-based visual representation for intuitive analysis.
Data Pipeline:
SQL Processing:

Data exploration and cleaning using SQL scripts.
Handling missing values and creating a structured dataset (prob_churn).
Creating views for churned and newly joined customers.
Power BI Dashboard:

Connecting cleaned SQL data to Power BI.
Developing visualizations and reports for churn data insights.


