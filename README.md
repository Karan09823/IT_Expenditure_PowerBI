# IT_Expenditure_PowerBI
# 1. Project Overview
This project provides a comprehensive analysis of IT expenditure across different business areas, IT areas, and cost elements. Using data that captures Actual, Planned, and Forecasted costs, the analysis helps identify budget variances, track spending trends over time, and highlight areas where IT resources are over or under-utilized. The interactive dashboard enables decision-makers to compare budget expectations with real-world outcomes, supporting cost optimization, financial transparency, and strategic IT planning.

# 2. Business Problem and Objective
Managing IT expenditure is critical for organizations, as technology investments represent a significant portion of operational costs. However, discrepancies often arise between planned budgets, forecasted expectations, and actual spending, making it difficult to maintain financial control and allocate resources effectively. Without clear visibility into these variances, organizations risk overspending, underutilization of resources, and missed opportunities for optimization.

This project sets out to:
-Compare Actual vs Planned vs Forecasted IT expenditures to measure budget accuracy.
-Identify spending trends over time to understand how costs evolve monthly and annually.
-Analyze costs across Business Areas, IT Areas, and Cost Element Groups to pinpoint major contributors to IT expenditure.
-Highlight variances and anomalies that may require corrective actions.
-Support strategic IT planning and decision-making through transparent, data-driven insights.

# 3. Dataset Description
The dataset contains detailed IT expenditure records, capturing financial data across business and IT dimensions. Each row represents an expenditure entry with its associated classification and financial values.

Columns Included:
-Date – Reporting period of the expenditure.
-Business Area – Business unit or department incurring the cost.
-Region – Geographical region where the expense is recorded.
-Country – Country of operation.
-IT Sub Area – Specific IT function or activity (e.g., Networking, Cloud Services).
-IT Area – Broader IT category (e.g., Infrastructure, Applications, Security).
-Cost Element Name – Detailed cost type (e.g., Hardware Purchase, Software License).
-Cost Element Group – Grouping of similar cost elements (e.g., Hardware, Software, Services).
-Cost Element Sub Group – Further breakdown of cost elements for granular analysis.
-Actual – Realized expenditure (what was truly spent).
-Forecast – Expected expenditure estimated during reporting.
-Plan – Budgeted expenditure defined at the start of the period.

Dataset Purpose:
-This dataset enables the comparison of Planned vs Forecast vs Actual IT expenditures, facilitating:
-Trend analysis over time.
-Variance identification.
-Business area and IT area cost distribution.
-Strategic planning and resource allocation

# 4. Methodology
Data Cleaning
Handled missing values: wherever null values were present in financial columns (Actual, Forecast, Plan), they were replaced with 0 instead of deletion to preserve the dataset integrity and ensure accurate calculations.
Standardized column names and ensured data types were correctly set (e.g., dates, numerical fields).

KPI Creation
To evaluate IT expenditure performance, several key performance indicators (KPIs) were created in Power BI using DAX formulas:
### Total Actual Expenditure
Total Actual = SUM(Data[Actual])

### Total Forecast Expenditure
Total Forecast = SUM(Data[Forecast])

### Total Planned Expenditure
Total Plan = SUM(Data[Plan])

### Variance (Actual vs. Forecast)
Variance (Actual vs. Forecast) = [Total Actual] - [Total Forecast]

### Variance (Actual vs. Plan)
Variance (Actual vs. Plan) = [Total Actual] - [Total Plan]

### Variance % (Actual vs. Forecast)
Variance % (Actual vs. Forecast) = DIVIDE([Variance (Actual vs. Forecast)], [Total Forecast])

### Variance % (Actual vs. Plan)
Variance % (Actual vs. Plan) = DIVIDE([Variance (Actual vs. Plan)], [Total Plan])

# 5. Insights
The IT expenditure analysis revealed the following key findings:

💰 Total Expenditure Overview
Actual Expenditure: 555.73M

Forecasted Expenditure: 890.54M

Planned Expenditure: 900.40M

📊 Budget Performance
Variance % (Actual vs Forecast): -38%

Variance % (Actual vs Plan): -38%

This indicates that actual spending was significantly lower than both forecasted and planned budgets.

🖥 IT Area Analysis
Infrastructure emerged as the area with the highest expenditure, suggesting major investments in core IT assets and systems.

👷 Cost Element Analysis
Labor was identified as the highest cost element group, highlighting workforce-related expenses as a primary cost driver.

# 6. Reference
<img width="1476" height="731" alt="image" src="https://github.com/user-attachments/assets/21ae8f9e-99c4-4f44-a8f3-506580cae3db" />

