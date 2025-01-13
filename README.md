# churn_data_analysis
This repository provides a concise analysis of customer churn using machine learning to help businesses predict churn, develop retention strategies, and enhance customer satisfaction.

## Steps Performed:
### 1. Data Exploration
    Queries were written to explore the dataset, calculate distinct values, and generate insights, such as:

    Gender Analysis: Distribution and percentage of customers by gender.
    Contract Analysis: Distribution and percentage of customers by contract type.
    Customer Revenue Analysis: Total revenue per customer status and its percentage of overall revenue.
    State Distribution: The proportion of customers by state, ranked by percentage.
  ![]![Screenshot (840)](https://github.com/user-attachments/assets/02e0f970-23d0-4fbc-83d4-f5671854e2f5)
  
### 2. Checking for Null and Blank Values
    A detailed query was executed to check nulls and blank values across all fields in the dataset. This step ensures the integrity of the data by identifying areas requiring data cleaning.

### 3. Data Cleaning
    Null values and empty strings were handled using SQL operations:

    COALESCE and NULLIF functions replaced missing or blank values with defaults. For example:
    Missing Value_Deal → "None"
    Blank Multiple_Lines → "No"
    Blank Churn_Reason → "Others"

### 4. Creating a Cleaned Table
    A new table, prob_churn, was created with cleaned data, ready for analysis. Fields were standardized to ensure consistency.
### 5. Creating Power BI Views
    To integrate with Power BI for visualization:

    vw_ChurnData: View focusing on customers with a status of "Churned" or "Stayed."
    vw_JoinData: View containing customers who recently joined with the status "Joined."
