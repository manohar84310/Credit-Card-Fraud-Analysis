# Credit-Card-Fraud-Analysis
Objective

To detect fraudulent credit card transactions by identifying unusual spending patterns and suspicious activity.
Steps Performed
1️⃣ Data Collection

Generated a dataset of 10,000+ credit card transactions containing transaction amount, time, location, and fraud indicators.

2️⃣ Data Cleaning (SQL / Python)

Performed:

Removed duplicate transactions
Handled missing values
Converted data types
Filtered invalid transaction amounts

Example SQL:

SELECT *
FROM transactions
WHERE Transaction_Amount > 0;
3️⃣ Fraud Detection Logic

Applied rule-based fraud detection:

Rules used:

High transaction amount (> ₹50,000)
Multiple transactions within short time
Transactions from unusual locations
Late-night transactions

Example SQL:

SELECT *
FROM transactions
WHERE Transaction_Amount > 50000
AND Transaction_Time_Hour BETWEEN 0 AND 5;
4️⃣ Power BI Dashboard Created

Dashboard Includes:

Total Transactions
Fraudulent Transactions Count
Fraud Rate (%)
Transactions by Location
Fraud Trend Over Time

Visuals Used:

Bar Chart
Line Chart
KPI Cards
Pie Chart
5️⃣ Key Insights

Example insights you can write:

5% transactions identified as fraud
Most fraud occurs during night hours
High-value transactions show higher fraud risk
Certain locations show repeated fraud activity
