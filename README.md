# Fintech-Customer-loan-Profiling
This project is to help Alo fintech company to ensure create loan eligibility criteria for its customers and ensure targeted campaigns are carried out to increase conversion rate.

# Business Problem
ALO Fintech aims to improve the profitability and quality of its lending portfolio by identifying customers who are most likely to qualify for loans and determining which loan products generate the highest returns. Without these insights, the company risks approving high-risk borrowers, allocating marketing resources inefficiently, and missing opportunities to maximize interest income. This project analyzes customer financial profiles, demographics, and loan preferences to identify eligible borrowers, support data-driven lending decisions, reduce credit risk, and enable targeted marketing campaigns that increase loan adoption and portfolio profitability.

# Business Questions
1. What percentage of customers qualify for loans based on the company's lending criteria?
2. Which financial factors (monthly income and Debt-to-Income ratio) have the greatest influence on loan eligibility?
3. Which customer segments (age, gender, and marital status) represent the most creditworthy borrowers?
4. How do loan preferences vary across different customer age groups?
5. Which loan products are expected to generate the highest annual interest revenue?
6. How can customer eligibility, demographics, and loan preferences be leveraged to improve lending decisions and marketing performance?

# Data cleaning

•	Removed duplicated customer ID in Dim_customers table to ensure the records are accurate.
•	Checked missing values and used the mean value for age to fill the gaps where age was missing.
•	Created the date table for time intelligence purposes
•	A decision table was equally created that had the customers profiled as “High” recognized as the most qualified to be considered for a loan.
•	Standardized data types in the various tables by ensuring the date table is in date format while the age columns shows whole number and the amounts are in currency format.
•	Created calculated decision table and columns for the eligible customers.

### Data Source: Zion Tech Hub

# Exploratory Data Analysis

### Data Summary:
The dataset was made up of 6 distinct tables, four dimensions table and one fact table with additional date-table and decision table created to aid the analysis.

### Customer Distribution:
Total number of customers: 150
Total customers in high profile segment: 68(45%)
Total eligible customers: 47(69%)

### Eligibility Distribution
•	Average income of eligible customers: 3.26M
•	Average income of non-eligible customers: 567.80k
•	Average DTI(debt to income) of eligible customers: 0.09
•	Average DTI of non-eligible customers: 0.54
