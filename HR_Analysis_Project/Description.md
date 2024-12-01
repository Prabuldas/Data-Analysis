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
- Measure Creation: Developed various measures such as Actual Working Days, Total Present Days, Work from Home, Present Onsite, Sick Leave Counts and Percentages, among others. These measures provided critical metrics for analysis.
- New Columns Addition: Added new columns to account for half days and full days (e.g., Half Work from Home and Work from Home) using 0.5 for half days and 1 for full days, ensuring accurate representation of work hours.
- Advanced Filtering: Used advanced filtering techniques to remove days not present in the data and days off, refining the analysis to focus only on relevant working days.
### Key Findings
Let's delve into these findings to extract meaningful conclusions.

- Overall Presence: An impressive overall employee presence rate of approximately 91.8% demonstrates a strong commitment to in-office work. This reflects the dedication and professionalism of the workforce at Atliq Technologies.

- Working from Home (WFH): Around 10% of employees prefer the flexibility of working from home. This insight underscores the importance of providing a work-from-home option to promote employee satisfaction and achieve a healthy work-life balance.

- Sick Leave (SL) Percentage: The sick leave percentage stands at a commendable 1.1%, indicating a culture of strong attendance and minimal sick leave instances among employees.

- Day of the Week and Presence Percentage: Analyzing presence percentages by day of the week reveals interesting patterns: Fridays show a slightly lower presence percentage of 90.1% compared to other weekdays. Mondays witness a high presence percentage of 93.2%, signalling a positive start to the workweek. Thursdays and Wednesdays demonstrate presence percentages of 90.5% and 92.1% respectively, indicating consistent attendance mid-week. Tuesdays mirror Mondays, with a presence percentage of 93.03%.


### Insights and Recommendations
Based on the data analysis, the following insights and recommendations can guide effective decision-making:

- Office Space Utilization:
Leverage higher attendance rates on Mondays and Tuesdays to plan team-building exercises and essential meetings that require maximum employee presence. This approach optimizes office space utilization and fosters collaboration.

- Maintenance and Off-Peak Activities:
Utilize Fridays and Thursdays, which exhibit slightly lower attendance rates, to focus on office maintenance and organize activities that require fewer employees. This strategy ensures efficient space management without disrupting regular work.

- Work-from-Home (WFH) Policy:
Considering the 10% preference for remote work, implementing or strengthening a work-from-home policy can offer employees flexibility and contribute to overall satisfaction and work-life balance.

- Wellness Programs:
While the low sick leave percentage indicates good employee health, introducing wellness programs and initiatives can further nurture a healthy work environment, reduce sick leave instances, and promote employee well-being.

### Conclusion 
In conclusion, the insightful data analysis empowers Atliq Technologies to optimize office space utilization, foster employee engagement, and enhance work-life balance. By leveraging these findings, the company can make informed decisions regarding team activities, maintenance schedules, work-from-home policies, and wellness programs. These measures will ultimately lead to a more productive and satisfied workforce.
### Screenshoot & References
