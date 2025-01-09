# TechStream Solutions: Unit Economics Analysis

## Project Overview
This project analyzes the Unit Economics for TechStream Solutions, a SaaS company. Key metrics such as Customer Acquisition Cost (CAC), Average Revenue Per User (ARPU), Cost of Goods Sold (COGS), Gross Margin, Lifetime Value (LTV), and the LTV/CAC ratio are calculated to provide insights into the company's financial health and growth potential.

## Data Sources
The following datasets were used:
1. **Monthly Expense**: Includes operational costs (e.g., Salesforce, AWS, Slack).
2. **Payroll Data**: Details salaries for sales, marketing, and production teams.
3. **Marketing Spending**: Daily marketing expenses.
4. **Receipts History**: Revenue and customer information.
5. **Customer Lifespan**: Dates for customer onboarding and churn.

## Steps and Decisions
1. **Customer Acquisition Cost (CAC)**:
   - Filtered the latest month to focus on recent expenses.
   - Included salaries of sales and marketing teams, as well as marketing and CRM costs.
   - Decided to include managers' salaries as they contribute directly to customer acquisition.

2. **Average Revenue Per User (ARPU)**:
   - Used revenue from new customers to calculate ARPU, focusing on profitability per new user.

3. **Cost of Goods Sold (COGS)**:
   - Included costs for server, software licenses, and engineering team salaries.
   - Allocated shared expenses (e.g., Slack, Zoom) proportionally.

4. **Gross Margin**:
   - Calculated as the percentage of revenue remaining after deducting COGS.

5. **Lifetime Value (LTV)**:
   - Used customer lifespan data to calculate the average lifetime of customers.
   - Multiplied ARPU by average lifespan and Gross Margin to estimate LTV.

6. **LTV/CAC Ratio**:
   - Evaluated to understand the profitability of acquiring new customers.

## How to Schedule the Script (Windows Task Scheduler)
To automate the script execution, follow these steps:
1. Save the script as a `.py` file (e.g., `unit_economics.py`).
2. Open Task Scheduler on your Windows system.
3. Click **Create Basic Task** and provide a name and description.
4. Set the trigger (e.g., daily, weekly) and the time for script execution.
5. Choose the action **Start a Program** and browse to the Python executable (e.g., `python.exe`).
6. Add the script path as an argument (e.g., `C:\path\to\unit_economics.py`).
7. Click **Finish** to save the task.

For detailed instructions, refer to the Colab file provided during the course.

---
