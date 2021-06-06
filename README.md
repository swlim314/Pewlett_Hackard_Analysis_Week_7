# Analysis of Retiring Employees at Pewlett Hackard
## Overview of Data Analyzed
I was tasked to determine the number of retiring employees at Pewlett Hackard, based on their current  title, as well as identify
employees who are currently eligible to participate in a mentorship program. To do this analysis, I was required to create several tables
using inner joins to map out employees and their titles and keeping a count on that. After these tables were created, another table was
required to identify elgibile employees for the mentorship program. This again required several inner joins based on the employees and
department employees tables, as well as with the employees and the titles table. After the inner joins, they were filtered by only
including current employees, and those that were born in the year 1965.
## Results of the Analysis
### Number of Retiring Employees
- One finding from the analysis on retiring employees was the varying amount of unique titles that the retiring employees had. Using
the following query:

**Unique Titles Query**

![Unique Titles query](https://github.com/swlim314/Pewlett_Hackard_Analysis_Week_7/blob/b73c3a1797bde5d62a056599ce68ea827794bb0c/Resources/Unique%20Titles%20code.png)

I was able to match each of the employees with their unique title. This required making sure to match the employee number with their
most senior ranking position on file. The output looked as follows:

**Unique Titles**

![Unique Titles](https://github.com/swlim314/Pewlett_Hackard_Analysis_Week_7/blob/b73c3a1797bde5d62a056599ce68ea827794bb0c/Resources/Unique%20Titles.png)

- Another major finding from the analysis on retiring employees was the large amount of retiring employees that were experienced/senior
personnel. There were more than double the amount of Senior Engineers (29,414) and Senior Staff (28,254) than Engineer (14,222) and Staff 
(12,243). This is shown in the image below.

**Retiring Titles**

![Retiring Titles](https://github.com/swlim314/Pewlett_Hackard_Analysis_Week_7/blob/efad847ab81f98ed07a2730a00e078138b2bf113/Resources/Retiring%20Titles.jpg)


The query required to show this output was:

**Retiring Titles Query**

![Retiring Titles code](https://github.com/swlim314/Pewlett_Hackard_Analysis_Week_7/blob/9bb1c03934a338b3b915ad2609677e0b8ec1ca2a/Resources/Retiring%20Titles%20code.png)

- Another major finding based off the retiring titles table is that there are only 2 Managers retiring at this time. This seems like an
extremely low number considering the 60,000+ Senior Engineers and Staff that are retiring at this time.
-Looking at the Mentorship Eligibility table, it appears as there are only 1549 available staff members that are able to provided
mentorship roles in the company. The images below show the query that was used to output the requisite mentorship table, as well as the
first 15 rows in that table, and last 15 rows.

**Mentorship Eligibility Query**

![Mentorship Eligibility code](https://github.com/swlim314/Pewlett_Hackard_Analysis_Week_7/blob/0720697415c6f27b96bd4c911683903c6ead5c25/Resources/Mentorship%20Eligibility%20code.png)

**Mentorship Eligibility**

![Mentorship Eligibility](https://github.com/swlim314/Pewlett_Hackard_Analysis_Week_7/blob/0720697415c6f27b96bd4c911683903c6ead5c25/Resources/Mentorship%20Eligibility.png)

**Mentorship Eligibility Last**

![Mentorship Eligibility last](https://github.com/swlim314/Pewlett_Hackard_Analysis_Week_7/blob/7cbf62584eeec2f7022ff3cb3a0c8521424ced62/Resources/Mentorship%20Eligibility%20last.png)

## Summary
- Based on the table, Retiring Tables, the amount of employees that are retiring would be 90,398.
- Based on the table Mentorship Eligibility Last, there are a total of 1549 eligible staff members to provide mentorship. There are
nowhere near enough employees to bridge the gap of the "silver tsunami" of retiring employees.
Two additional tables that might provide more insight into the upcoming "silver tsunami" are a table that shows the seniority of
employees based on years worked at the company (binned for every 5-10 years) to get an idea of where the general experience level is.
Another useful table would be a table that showed the amount of employees retiring from each of the departments. This way the company
would be able to tell where most of the mentorship needed to take place in.
