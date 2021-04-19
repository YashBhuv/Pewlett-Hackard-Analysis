# Pewlett-Hackard-Analysis
## Project Overview
Analyze Pewlett Hackard employee database using PostgreSQL to help the company anticipate the "silver tsunami" as many current employees will leave to retirement.
For this analysis we will:
- determine the number of retiring employees per title,
- identify employees who are eligible to participate in a mentorship program.
## Resources
Data Source: departments.csv, dept_manager.csv, dept_emp.csv, employees.csv, salaries.csv, titles.csv
Software: PostgreSQL 11.9, pgAdmin 4
Documentation: PostgreSQL documentation, PostgreSQL tutorial, pgAdmin documentation

## Results
### Number of retiring employees per title
Using the ERD created previously, the following Retirement Titles table was created and it holds all the titles of employees who were born between January 1st, 1952 and December 31st, 1955.

![1](https://user-images.githubusercontent.com/64053195/115276606-39baee00-a111-11eb-8bfe-6129ae9c918e.png)

90,398 employees or 37.7% of the company's total current employees will be retiring soon.
Senior Engineer, Senior Staff and Engineer will be the most impacted positions with respectively 29,414, 28,254 and 14,222 futures retirees, which correspond to 12.3%, 11.8% and 5.92% of the company's workforce.
Only 2 Managers will be retiring soon.
It seems that management renewal has been to focus of the company to the detriment of technical positions renewal.

### Employees eligible for the mentorship program
Using the ERD created previously, the following Mentorship Eligibility table was created and it holds all the current employees who were born between January 1st, 1965 and December 31st, 1965.
![2](https://user-images.githubusercontent.com/64053195/115276690-57885300-a111-11eb-9e70-b315d5184b61.png)
Extract of the mentorship eligibility table
 
![3](https://user-images.githubusercontent.com/64053195/115276731-6969f600-a111-11eb-8339-175cd936b5a7.png)
Eligible mentors per job title

- There are 1,549 employees eligible to participate in the mentorship program.
- 294 Senior Engineers, 422 Senior Staffs and 395 Engineers are eligbible mentors.

## Summary
- 90,398 roles will need to be filled as the "silver tsunami" begins to make an impact.
- There are 1,549 eligible mentors in the company.
- If we assume that they will all be willing to participate in the mentorship program, it will imply that each mentor would have an average of 58 mentees, so we can conclude that there is not enough mentors to prepare the next generation of Pewlett Hackard employees.
- The following tables give us the number of retirement-ready employees and the number of eligible mentors per department. It shows that all departments are lacking mentors.

![4](https://user-images.githubusercontent.com/64053195/115276875-9918fe00-a111-11eb-914f-ff5c1e2d585b.png)
Retiring employees per department

![5](https://user-images.githubusercontent.com/64053195/115276922-a504c000-a111-11eb-89ca-5d14d86de134.png)
Eligible mentors per department

- Reviewing the criteria to qualify for the mentorship program would be needed by the company to prepare for the coming "silver tsunami".
