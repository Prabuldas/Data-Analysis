<h1 align="CENTER"> Atliq HR Data Analysis </h1>


<H2>Table of Contents</H2>

- [Project Summary](#Project-Summary)
- [Data Source](#Data-Source)
- [Business Understanding](#Business-Understanding)
- [Data understanding](#Data-understanding)
- [ETL](#ETL)
- [Analysis and Dashboard Development](#Analysis-and-Dashboard-Development)
- [Key Findings](#Key-Findings)
- [Insights and Recommendations](#Insights-and-Recommendations)
- [Conclusion](#Conclusion)
- [Screenshoot & Reference](#Screenshoot-&-References)
### Project Summary
AtliQ Hardware, with multiple branches across India, provides computer hardware and peripheral manufacturers to its clients. The HR department of a company is facing challenges in monitoring employee attendance and identifying patterns of absenteeism. They need to have a comprehensive view of the attendance records of all employees, including the number of leaves taken and reasons for absence.

### Data Source
We are provided with the Excel datasheet which contains the employees data for 3 months between April 2022-June 2022. Data set contains employees attendance data along with attendance keys Eg: SL --> Sick Leave.
### Business Understanding
- Find Total Employees Attendance %, Sick Leave % and Work from home %
- Find the trends for it over time
- Analyzing the same trends in weekdays
### Data understanding
### ETL

- Data Loading
    - Loaded the employee data into Power BI to start the analysis.
- Data Transformation
    - Filtering Data: Filtered the data to include only April, ensuring the analysis was specific to this period.
    - Table Duplication: Duplicated the table to have a working copy for all necessary transformations while preserving the original data.
    - Header Promotion: Promoted the first row to headers for better data organization.
    - Row Removal: Removed the top row to clean the dataset.
    - Column Renaming: Renamed the columns to more meaningful names for clarity and consistency.
    - Data Unpivoting: Selected the employee code and name columns and unpivoted other columns to restructure the data for easier analysis.
    - Invalid Rows Removal: Changed the data type of the date column to DATE to identify and remove invalid rows by filtering out errors, automating the process for future data updates.
    - Parameter Creation: Created a parameter to dynamically filter the sheet names.
    - Function Creation: Created a function called GetData from the template table. Changed the filter of the template column to use the parameter instead of text, ensuring flexibility and automation.
    - Function Invocation: Applied the GetData function using 'Invoke Custom Function' on the original data to transform it accordingly.
    - Column Cleanup: Removed unnecessary columns to streamline the dataset and focus on relevant information.
    - Final Data Load: Loaded only the transformed and clean data into Power BI for analysis and visualization.
### Analysis and Dashboard Development
### Key Findings
Let's delve into these findings to extract meaningful conclusions.

- Overall Presence: An impressive overall employee presence rate of approximately 91.8% demonstrates a strong commitment to in-office work. This reflects the dedication and professionalism of the workforce at Atliq Technologies.

- Working from Home (WFH): Around 10% of employees prefer the flexibility of working from home. This insight underscores the importance of providing a work-from-home option to promote employee satisfaction and achieve a healthy work-life balance.

- Sick Leave (SL) Percentage: The sick leave percentage stands at a commendable 1.1%, indicating a culture of strong attendance and minimal sick leave instances among employees.

- Day of the Week and Presence Percentage: Analyzing presence percentages by day of the week reveals interesting patterns: Fridays show a slightly lower presence percentage of 90.1% compared to other weekdays. Mondays witness a high presence percentage of 93.2%, signalling a positive start to the workweek. Thursdays and Wednesdays demonstrate presence percentages of 90.5% and 92.1% respectively, indicating consistent attendance mid-week. Tuesdays mirror Mondays, with a presence percentage of 93.03%.


### Insights and Recommendations
### Conclusion 
### Screenshoot & References
