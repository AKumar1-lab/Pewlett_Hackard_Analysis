# Pewlett_Hackard_Analysis

Module 7 - Exploring data with SQL

Completed by Angela Kumar

# Overview

Create entity relationship databases(ERDs), Perform data modeling, and complete analysis on an employee database using SQL techniques.
Applying knowledge of DataFrames and tabular data, to create entity relationship diagrams (ERDs), import data into a database, troubleshoot common errors, and create queries that use data to answer questions. Databases are used everywhere—small and large businesses, and even individuals working on personal projects—and SQL is one of the most widely used query languages. Its ability to organize and query data, especially on a large scale, makes SQL knowledge a highly sought after skill in the workforce

# Resources

Software: PostgreSQL12, PGAdmin4, VSCode, Jupyter Notebook; Anaconda3; QuickDBD

Files: departments.csv; dept_emp.csv; dept_manager; employees.csv; salaries.csv; titles.csv, challenge_starter_code

# Background

Bobby from Pewlett Packard has proven his SQL chops, his manager has given both of you two more assignments: determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Lastly a written report that summarizes your analysis and helps prepare Bobby’s manager for the “silver tsunami” as many current employees reach retirement age.

# Deliverables

## Deliverable 1: 

## Retirement Titles

Create a Retirement Titles table that holds all the titles of current employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions—you’ll need to use the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, use the COUNT() function to create a final table that has the number of retirement-age employees by most recent job title.  

<img width="561" alt="retirement_titles screenshot" src="https://user-images.githubusercontent.com/85860367/128596492-826219a8-2e2c-45ee-82ac-569e33a9bade.PNG">

<img width="194" alt="retirement titles count" src="https://user-images.githubusercontent.com/85860367/128609363-a0bd0bed-0361-43c7-b8e8-29aed4f657a1.PNG">

The current age group is between 66-69.  The retirement analysis retrieved 133,776 employees; however due to promotions the number has employees with duplicate positions for their employee number.  The next step would be to reformat the retirement titles database and only retrieve the current title for the employee as seen in unique titles.

## Unique Titles

There are duplicate entries for some employees because they have switched titles over the years. Use the following instructions to remove these duplicates and keep only the most recent title of each employee.

<img width="457" alt="Unique titles screenshot" src="https://user-images.githubusercontent.com/85860367/128596472-a2aaac3a-6579-44f5-9811-65ca4ff9a473.PNG">

<img width="184" alt="count of unique titles" src="https://user-images.githubusercontent.com/85860367/128596481-fe924669-886b-4e53-b7b5-73c74e844378.PNG">

The database retrieved 90,398 employees that are set to retire within the age group of 66-69  and current role.  Many of them are senior staff or provide expert level of services.  The current list of employees at Pewlett Hackard is 300,024.  The percentage of retiring staff is about 30% of the Pewlett Hackard employees.  The average age where people retire is about 67, this is because you must be 67 to receive the full social security benefits. 
source: https://www.annuity.org/retirement/retirement-statistics/
So Pewlett Hackard should not be surprised as it is the norm.

## Retiring Titles

Retrieve the number of employees by their most recent job title who are about to retire.

<img width="188" alt="Screenshot of full retiring titles" src="https://user-images.githubusercontent.com/85860367/128609679-775ad09d-d351-4f92-895d-2dc573b7779d.PNG">

The data analysis reveals that at least 45,397 or 50.22% of engineers of the 90,398 are set to retire!  Another point that is revealed is that 57,668 are Senior Staff and Engineers, that is about 63.79% of the 90,398. This should be alarming to the organization and to Human Resources as that is a lot of people leaving the organization.  This should really be the concern as staff with expert level and experience leave the organization, this results in a huge brain drain and a skills gap. Many organization grapple to find eligible workers with equal expertise or experience level.

<img width="400" alt="screenshot of graph of retiring titles" src="https://user-images.githubusercontent.com/85860367/128610771-1ea91f8e-1525-4464-9fd0-fbbfad6036b4.PNG">


## Deliverable 2

## The Employees Eligible for the Mentorship Program

Create a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965. 
Current age of employees within this group is 56. The number of employees retrieved for the mentorship program is 1,549, this is not enough to cover the number of employees planning to retire.  The percentage results in only 1%, which will be a huge employee and skills gap.

<img width="620" alt="Mentorship" src="https://user-images.githubusercontent.com/85860367/128596540-c83cb916-fe52-4bac-9f1a-53f597e969a5.PNG">

<img width="190" alt="mentor eligibilty count" src="https://user-images.githubusercontent.com/85860367/128596548-52e2536e-395c-445c-bc48-281574be2e61.PNG">


Deliverable 3: A written report on the employee database analysis (README.md)

## Summary: 
Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."

How many roles will need to be filled as the "silver tsunami" begins to make an impact?
The immediate concern is to fill 90,398 positions as previously discussed.

<img width="184" alt="count of unique titles" src="https://user-images.githubusercontent.com/85860367/128596481-fe924669-886b-4e53-b7b5-73c74e844378.PNG">
The immediate need would be for those retiring that are born during 1952-1955 (Age group is 66-69), with a hire date of 1985-1988 (Service of 33-36 years; this is about 41,380 staff.  

<img width="300" alt="Number of employees retiring" src="https://user-images.githubusercontent.com/85860367/128612636-4862186b-3995-43bb-af66-0eb94010425a.PNG">

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees? no there isn't, we would need to expand the mentor eligibility to analyze staff between the years 1960-1985.  This query results in 93,756 employees, this should be able cover the 90,398 that are planning to retire.

<img width="200" alt="Expanded mentorship screenshot" src="https://user-images.githubusercontent.com/85860367/128613453-26f3ac34-6763-43c3-ae89-3c9b9351d637.PNG">

<img width="82" alt="screenshot of expanded mentorship" src="https://user-images.githubusercontent.com/85860367/128613463-7b480daf-db01-477a-91a4-033d679b8460.PNG">

It also may be of interest to increase salaries for the Senior Engineers, Senior Staff and also increase the number of Managers.  The organization would benefit if they offer more promotions and salary increments to retain the employees they have.
When we did the analyis on the Managers there are only 2 active managers in the entire organization, with 2 retiring, there would not be any to run the day-to-day operations of an institution specifically in Sales and Research.

<img width="300" alt="Managers Info screenshot" src="https://user-images.githubusercontent.com/85860367/128614164-a44d1e50-7c72-402c-8f5f-0cb5323795c9.PNG">

Increasing salaries for Senior Engineers and Senior Staff will appeal in recruitment, hiring and promotions. It will be of interest to be competitive in salaries within the industry. Managers do not make $70K, and Engineers do not make $60K; it appears that salaries have not been updated since day of hire.  That could be a problem for the retiring staff as well because retirement or pension is based on the last highest salary.

In conclusion, it is understandable that this analysis is based a learning tool to work with SQL.  In real life event; someone will need to manage and analyze the data much more frequently especially with employee data to ensure that there are no duplication of records, fraud, ensure accuracy with the head count, and current salaries.  It is extremely important for database managers to prevent over-riding information. Internal controls must be in place and followed to ensure the highest accuracy with employee or human resource analytics as the data feeds into many other data pools at the local, state, and federal levels.  Higher salaries and promotions motivate employees with job satisfaction, comfortable lifestyle, and decrease attrition rates.  



