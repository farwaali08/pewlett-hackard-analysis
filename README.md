# pewlett-hackard-analysis

## **OVERVIEW**

This analysis was prepared for Pewlett Hackard (PH) to assist with workforce-planning, as the company prepares for a significant number of retirements over the next few years. 

An employee database was created and used to identify the employees eligible for retirement, by title, as well as those that would be able to provide mentorship to their successors. In doing so, PH can best prepare for future staffing needs, and determine a strategy for providing effective onboarding and knowledge transfer resources to new hires. 

Ideally, this is to be completed before the "silver tsunami" makes landfall.

## **TOOLS & QUICK LINKS**

### **TOOLS**

* PostgreSQL 14.0
* pgAdmin 4

[Code](https://github.com/farwaali08/pewlett-hackard-analysis/blob/de0033873d1886e0d2991903844e8629c7ac9a34/Queries/Employee_Database_challenge.sql)

[Retirement Titles CSV](https://github.com/farwaali08/pewlett-hackard-analysis/blob/de0033873d1886e0d2991903844e8629c7ac9a34/Data/retirement_titles.csv)

[Unique Titles CSV](https://github.com/farwaali08/pewlett-hackard-analysis/blob/de0033873d1886e0d2991903844e8629c7ac9a34/Data/unique_titles.csv)

[Retiring Titles CSV](https://github.com/farwaali08/pewlett-hackard-analysis/blob/de0033873d1886e0d2991903844e8629c7ac9a34/Data/retiring_titles.csv)

[Mentorship Eligibility CSV](https://github.com/farwaali08/pewlett-hackard-analysis/blob/de0033873d1886e0d2991903844e8629c7ac9a34/Data/mentorship_eligibility.csv)

## **RESULTS, SUMMARY, AND ANALYSIS**

An employee database was created from 6 different data sets containing company information. The original sets can be found in the "Data" folder. The relationships between the datasets was mapped out in the ERD below:

![alt_text](https://github.com/farwaali08/pewlett-hackard-analysis/blob/22efad72b66ab7eca1206ba7027cf513c3161df3/EmployeeDB.png)



First, a count of the total active employees was obtained:

![alt_text](https://github.com/farwaali08/pewlett-hackard-analysis/blob/01dd05b074246b275e43cc4021e957c518d879c9/current_employees.png)


Next, a list of [employees eligible for retirement](https://github.com/farwaali08/pewlett-hackard-analysis/blob/22efad72b66ab7eca1206ba7027cf513c3161df3/Data/unique_titles.csv) was created, and used to obtain a count of retirements by title, as seen in the image below:

![alt_text](https://github.com/farwaali08/pewlett-hackard-analysis/blob/22efad72b66ab7eca1206ba7027cf513c3161df3/Data/retiring_titles.png)

Currently, there are `90,398` employees that are eligible for retirement, which is almost `38%` of the current total work force of `240,124`. This is means that there will be potentially 90,000+ vacancies that will need to be filled in the near future. The

