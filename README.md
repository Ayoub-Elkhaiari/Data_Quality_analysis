# High Data Quality

High data quality means having data that is reliable, accurate, and free from issues. High-quality data is essential as it is used across multiple functions such as operations, customer management, marketing, analysis, and decision-making. **Poor data quality** can lead to wasted time and resources, poor decision-making, and overall frustration for both users and stakeholders.

## Examples of Common Data Quality Issues

1. **Incompleteness**: Missing or incomplete data fields, such as customer contact details or aircraft maintenance records, can hinder operations and customer satisfaction.
2. **Inaccuracy**: Data containing typos, junk values, or column mix-ups affects the reliability of information. For example, incorrectly recording a part’s serial number could lead to confusion in inventory tracking.
3. **Inconsistency**: Inconsistent data, like values in multiple currencies without clear conversion, can complicate data analysis. An example would be tracking costs in both euros and dollars without a standard format.
4. **Invalidity**: Logically incorrect data, such as a negative value for product units (e.g., -10 for units in stock), which could lead to issues in inventory planning and reporting.
5. **Redundancy**: Duplicated data entries, such as repeating the same maintenance report, can lead to incorrect analysis and waste storage space.
6. **Non-standard Formatting**: Differences in decimal precision, such as "13.99" vs. "14.777709," can lead to inconsistency and error in aggregations and reporting.

## The Importance of Data Quality Assurance

To address and prevent these issues, **Data Quality Assurance (DQA)** processes are essential. DQA involves various techniques and practices to ensure that data remains accurate, consistent, and useful.

### Key Components of Data Quality Assurance

1. **Data Profiling**: Profiling is the process of exploring and analyzing data to identify issues. This involves summarizing data characteristics, such as row counts, blank values, duplicates, and outliers. For example, in a Customer table, profiling might reveal that 2% of rows have missing email addresses, which may be acceptable, whereas 20% would indicate a data quality issue needing attention.

2. **Data Quality Metrics**: Data quality is often measured using specific metrics that help quantify its reliability and completeness:
   - **% Complete**: Measures how much of the data is missing. For instance, if Airbus’s Quality Management System (QMS) shows that 98% of maintenance records are complete, the data is considered more reliable.
   - **% Accurate**: Assesses how much of the data accurately represents real-world information. This metric is crucial in areas like part specifications where accuracy is paramount.
   - **% Conformance**: Indicates how much of the data aligns with defined business rules. For example, if there’s a rule that every quality incident must be linked to a maintenance order, the % conformance metric would track how well this rule is followed.

### Tools and Techniques for Data Profiling

You can perform data profiling using SQL queries, which are effective for identifying null values, duplicates, or ensuring field formats are consistent. For example:
   - **SQL Query Example**: `SELECT COUNT(*) FROM Customers WHERE Email IS NULL;` – to count missing email addresses.
   - **SQL Server Data Quality Services (DQS)**: DQS automates profiling processes, allowing you to run checks on the entire dataset efficiently without writing custom SQL code.

For larger datasets or advanced data processing, tools like **Python's pandas library** can provide detailed insights into missing or invalid data, offering additional capabilities for data manipulation and visualization.

### Data Quality Assurance in a Project Context

Data quality assurance is a continuous process and not a one-time step. This is especially important in dynamic environments, such as **Airbus’s Quality Management System**. As new data sources are integrated or updates are made to the system, data quality must be monitored and maintained over time to prevent degradation. Regular profiling and validation ensure that decision-makers can trust the data being used for critical processes.

For instance, in the **aerospace industry**, ensuring high data quality could mean preventing errors in part tracking or maintenance scheduling. Poor data quality in these areas could lead to delays, increased costs, or even safety risks.

### Specific Scenario: Applying Data Quality in Airbus

As a Data Quality Analyst at Airbus, you would focus on improving data reliability and usability within the Quality for Airframe Services (QBSR) department. By ensuring that data on non-conformities and performance metrics is accurate and complete, you enable more effective quality management and operational efficiency.

For example, suppose you identify that maintenance data inconsistently records dates across different systems or formats. By standardizing date formats and setting up automated quality checks, you would help ensure Airbus teams can confidently analyze trends in maintenance records to predict and prevent issues before they arise.

### Summary

In this role, your primary tasks include:
- **Data Profiling and Issue Identification**: Using tools like SQL or DQS to explore and profile data, identify issues, and ensure data quality.
- **Defining Quality Metrics**: Using metrics to quantify completeness, accuracy, and conformance, ensuring data aligns with Airbus’s quality standards.
- **Continuous Quality Assurance**: Treating data quality as an ongoing responsibility, especially in dynamic and regulated environments like aerospace.
- **Communication and Documentation**: Working closely with end-users to understand their needs and ensure they have access to high-quality data for informed decision-making.
