# Pewlett_Hackard_Analysis

Module 7 - Exploring data with SQL

# Overview

# Resources

Software: PostgreSQL12, PGAdmin4, VSCode, Jupyter Notebook; Anaconda3; QuickDBD
Files: departments.csv; dept_emp.csv; dept_manager; employees.csv; salaries.csv; titles.csv, challenge_starter_code

# Background

Bobby from Pewlett Packard has proven his SQL chops, his manager has given both of you two more assignments: determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Lastly a written report that summarizes your analysis and helps prepare Bobby’s manager for the “silver tsunami” as many current employees reach retirement age.

# Deliverables
Deliverable 1: 

## Retirement Titles

Create a Retirement Titles table that holds all the titles of current employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions—you’ll need to use the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, use the COUNT() function to create a final table that has the number of retirement-age employees by most recent job title.

<img width="561" alt="retirement_titles screenshot" src="https://user-images.githubusercontent.com/85860367/128596492-826219a8-2e2c-45ee-82ac-569e33a9bade.PNG">

<img width="184" alt="count of unique titles" src="https://user-images.githubusercontent.com/85860367/128596500-69d5a82e-76b9-4186-a9aa-54b1ebae6e3c.PNG">

## Unique Titles

There are duplicate entries for some employees because they have switched titles over the years. Use the following instructions to remove these duplicates and keep only the most recent title of each employee.

<img width="457" alt="Unique titles screenshot" src="https://user-images.githubusercontent.com/85860367/128596472-a2aaac3a-6579-44f5-9811-65ca4ff9a473.PNG">

<img width="184" alt="count of unique titles" src="https://user-images.githubusercontent.com/85860367/128596481-fe924669-886b-4e53-b7b5-73c74e844378.PNG">


## Retiring Titles

Retrieve the number of employees by their most recent job title who are about to retire.

<img width="431" alt="retiring_titles screenshot" src="https://user-images.githubusercontent.com/85860367/128596450-d39cf6f4-a903-4fe0-90fc-08d93102d537.PNG">


Deliverable 2: The Employees Eligible for the Mentorship Program

Create a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.

<img width="620" alt="Mentorship" src="https://user-images.githubusercontent.com/85860367/128596540-c83cb916-fe52-4bac-9f1a-53f597e969a5.PNG">
<img width="190" alt="mentor eligibilty count" src="https://user-images.githubusercontent.com/85860367/128596548-52e2536e-395c-445c-bc48-281574be2e61.PNG">


Deliverable 3: A written report on the employee database analysis (README.md)

## Summary: 
Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."
How many roles will need to be filled as the "silver tsunami" begins to make an impact?
Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
