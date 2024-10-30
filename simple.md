# High Data Quality

High-quality data means data that is reliable, accurate, and free of issues. Good data quality is important because it helps in many areas like operations, customer management, marketing, analysis, and decision-making. On the other hand, **poor data quality** can lead to wasted time, wrong decisions, and frustration.

## Common Data Quality Problems

1. **Incompleteness**: Missing data, like incomplete customer information, can cause issues in service and satisfaction.
2. **Inaccuracy**: Data with typos, junk values, or errors can make it hard to trust information. For example, a wrong serial number for a part can confuse inventory tracking.
3. **Inconsistency**: Inconsistent data, such as values in different currencies without conversions, makes analysis difficult. 
4. **Invalidity**: Incorrect data that doesn’t make sense, like a negative number of product units (e.g., -10 for items in stock).
5. **Redundancy**: Duplicate entries in data can cause incorrect analysis and use up storage.
6. **Non-standard Formatting**: Differences in decimal places, like "13.99" vs. "14.777709," can lead to errors in calculations and reporting.

## Why Data Quality Assurance Matters

**Data Quality Assurance (DQA)** is a set of processes to make sure data stays accurate, consistent, and useful.

### Main Parts of Data Quality Assurance

1. **Data Profiling**: This means exploring and analyzing data to find issues. For example, you might check how many rows are blank, duplicates, or outliers. If the Customer table has only 2% of rows missing, it’s okay; but if 20% are missing, it’s a big problem.

2. **Data Quality Metrics**: We can measure data quality with metrics to check if it’s reliable:
   - **% Complete**: Shows how much data is missing. For example, if 98% of maintenance records are filled in, the data is more trustworthy.
   - **% Accurate**: Measures how much data correctly reflects reality, like making sure part descriptions are correct.
   - **% Conformance**: Checks if data follows rules. For example, every quality incident should be linked to a maintenance order.

### Tools and Methods for Data Profiling

You can use SQL queries to profile data, which helps find missing values, duplicates, or check data formats. For example:
   - **SQL Query Example**: `SELECT COUNT(*) FROM Customers WHERE Email IS NULL;` – to find missing email addresses.
   - **SQL Server Data Quality Services (DQS)**: This tool helps automate profiling without needing custom SQL code.

For bigger datasets, tools like **Python’s pandas library** can provide more detail, showing missing or incorrect data and allowing for data visualization and manipulation.

### Keeping Data Quality High

Data quality management is a continuous process. This is especially true in settings like **Airbus’s Quality Management System**. As new data is added or updated, data quality needs regular checks to prevent issues. Consistent profiling and validation help ensure that decision-makers can trust the data they use.

In the **aerospace industry**, high-quality data prevents errors in areas like parts tracking or maintenance scheduling, which could otherwise lead to delays, extra costs, or even safety risks.

### Example: Data Quality Work at Airbus

As a Data Quality Analyst at Airbus, you would focus on improving data reliability in the Quality for Airframe Services (QBSR) department. Ensuring data accuracy in non-conformity reports and performance metrics will help the department make better decisions.

For instance, if maintenance data has inconsistent date formats, standardizing those dates and setting up regular checks would allow Airbus teams to confidently analyze maintenance trends to predict and prevent issues.

### Summary

In this role, your main tasks would include:
- **Data Profiling**: Using tools like SQL or DQS to explore and check data for quality.
- **Setting Quality Metrics**: Measuring data completeness, accuracy, and conformance to ensure it meets Airbus standards.
- **Continuous Data Quality Checks**: Regularly maintaining data quality to keep it reliable in fast-changing environments like aerospace.
- **Communication**: Working with end-users to understand their needs and help them make decisions based on good-quality data.
