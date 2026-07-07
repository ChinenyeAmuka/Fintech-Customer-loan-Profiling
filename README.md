# Fintech-Customer-loan-Profiling
This project is to help Alo fintech company to ensure create loan eligibility criteria for its customers and ensure targeted campaigns are carried out to increase conversion rate.

## Table of Content
1. [Business_Problem](#Business_Problem)
2. [Business_Questions](#Business_Questions)
3. [Tools Used](#Tools_Used)
4. [EDA](#Exploratory_Data_Analysis)
5. [Data Cleaning](#Data_Cleaning)
6. [Data Source](#Data_Source)
7. [Key_Insights](#Key_Insights)
8. [Recommendations](#Recommendations)
9. [Dashboard](#Dashboard)
10. [Connect_with_me](#Connect_with_me)

# Business_Problem
ALO Fintech aims to improve the profitability and quality of its lending portfolio by identifying customers who are most likely to qualify for loans and determining which loan products generate the highest returns. Without these insights, the company risks approving high-risk borrowers, allocating marketing resources inefficiently, and missing opportunities to maximize interest income. This project analyzes customer financial profiles, demographics, and loan preferences to identify eligible borrowers, support data-driven lending decisions, reduce credit risk, and enable targeted marketing campaigns that increase loan adoption and portfolio profitability.

# Business_Questions
1. What percentage of customers qualify for loans based on the company's lending criteria?
2. Which financial factors (monthly income and Debt-to-Income ratio) have the greatest influence on loan eligibility?
3. Which customer segments (age, gender, and marital status) represent the most creditworthy borrowers?
4. How do loan preferences vary across different customer age groups?
5. Which loan products are expected to generate the highest annual interest revenue?
6. How can customer eligibility, demographics, and loan preferences be leveraged to improve lending decisions and marketing performance?

# Data cleaning

- Removed duplicated customer ID in Dim_customers table to ensure the records are accurate using power quary.
- Checked missing values and used the mean value for age to fill the gaps where age was missing.
- Created the date table for time intelligence purposes
- A decision table was equally created that had the customers profiled as “High” recognized as the most qualified to be considered for a loan.
- Standardized data types in the various tables by ensuring the date table is in date format while the age columns shows whole number and the amounts are in currency format.
- Created calculated decision table and columns for the eligible customers usinf DAX formula

# Tools Used: 
Powwer BI, power query and DAX
---
### Data Source: Zion Tech Hub
---
# Exploratory Data Analysis

### Data Summary:
The dataset was made up of 6 distinct tables, four dimensions table and one fact table with additional date-table and decision table created to aid the analysis.

### Customer Distribution:
Total number of customers: 150
Total customers in high profile segment: 68(45%)
Total eligible customers: 47(69%)

### Eligibility Distribution
- Average income of eligible customers: 3.26M
- Average income of non-eligible customers: 567.80k
- Average DTI(debt to income) of eligible customers: 0.09
- Average DTI of non-eligible customers: 0.54
---
# Insights
1. 69% of the "high" profile segment (47 of 68 customers) met loan eligibility criteria, but this segment is only 45% of the total customer base, meaning just 31% of ALO's total customers (47 of 150) are currently loan-eligible. This is a strong screening rate within qualified prospects, but a signal that eligibility criteria may be filtering out a large share of the wider customer base, this is worth investigating whether marketing is reaching the right segment upstream.
2. Eligible customers have an average monthly income roughly 6x higher than non-eligible customers ($3.26M vs. $567.80K) and a substantially lower DTI ratio (0.09 vs. their non-eligible counterparts0.54). This confirms income and DTI are the two clearest discriminators of loan eligibility and should anchor any pre-qualification scoring model.
3. Within the eligible pool, 55.32% are male, the 46–55 and 56–65 age brackets show the highest concentration of eligible borrowers, and married customers make up the largest marital-status group (21 customers, 47%). This profile — mid-to-late career, married, represents ALO's core creditworthy segment and should anchor persona-based marketing.
4. Loan preference varies clearly by age: customers aged 46–65 skew toward car loans (12 and 7 customers respectively), while younger customers (under 25 through 36–45) skew toward school loans. Product messaging should be age-segmented rather than one-size-fits-all.
5. Car loans generate the highest projected annual interest yield at $16.1M, out of $39.22M total projected interest across all products, making it the single highest-value product to prioritize for eligible customers in the 46–65 bracket.
6. Combining eligibility, demographics, and loan-preference data lets ALO move from broad marketing to precision targeting, reaching the right customer, with the right product, at the right lifecycle moment.
---
# Recommendations
1. Build a pre-qualification funnel using income and DTI thresholds before marketing spend is allocated, since these two factors are the clearest eligibility drivers. This reduces wasted campaign spend on the 69% currently ineligible.
2. Prioritize car loan campaigns toward the 46–65 age bracket, ALO's highest-yield, highest-demand combination ($16.1M projected interest). Consider a pre-approved offer for eligible customers in this segment to shorten the conversion cycle.
3. Run a parallel school-loan campaign targeted at customers under 46, since this segment shows a distinct preference pattern that a single car-loan-focused campaign would miss.
4. Segment marketing messaging by eligibility status, not just by demographics e.g., pre-approved/fast-track messaging for eligible customers vs. "improve your eligibility" nurture content (debt paydown tips, income verification support) for non-eligible customers, to convert more of the 69% currently filtered out over time.

---
# Connect with me
Linkedin: www.linkedin.com/in/ chinenye-amuka-79a992137
---

# Dashboard

<img width="777" height="438" alt="Screenshot (312)" src="https://github.com/user-attachments/assets/30602add-93e0-4b6c-9973-abecd7a8b6f5" />

