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

[Mentorship Eligibility CSV](https://github.com/farwaali08/pewlett-hackard-analysis/blob/c24e562565b28b3723902f18c9baf66550329bbe/Data/mentorship_eligibility.csv)

## **RESULTS, SUMMARY, AND ANALYSIS**

An employee database was created from 6 different data sets containing company information. The original sets can be found in the "Data" folder. The relationships between the datasets was mapped out in the ERD below:

![alt_text](https://github.com/farwaali08/pewlett-hackard-analysis/blob/22efad72b66ab7eca1206ba7027cf513c3161df3/EmployeeDB.png)



First, a count of the total active employees was obtained:

![alt_text](https://github.com/farwaali08/pewlett-hackard-analysis/blob/01dd05b074246b275e43cc4021e957c518d879c9/current_employees.png)


Next, a list of [employees eligible for retirement](https://github.com/farwaali08/pewlett-hackard-analysis/blob/22efad72b66ab7eca1206ba7027cf513c3161df3/Data/unique_titles.csv) was created, and used to obtain a count of retirements by title, as seen in the image below:

![alt_text](https://github.com/farwaali08/pewlett-hackard-analysis/blob/22efad72b66ab7eca1206ba7027cf513c3161df3/Data/retiring_titles.png)

Currently, there are `90,398` employees that are eligible for retirement, which is almost `38%` of the current total work force of `240,124`. This is means that there will be potentially 90,000+ vacancies that will need to be filled in the near future. This is certainly an undertaking, and will require extensive planning to ensure that these transitions are implemented as seamlessly as possible. Additionally, nearly two-thirds, or `67%` of the potential retirees are currently in Senior Engineer or Senior Staff positions. This indicates that these positions should take priority when making staffing decisions.

With more than a third of the staff approaching retirement, another consideration that needs to be made is ensuring that there is sufficient time and resourcing for knowledge transfer. In anticipation of this task, a [list of mentors](https://github.com/farwaali08/pewlett-hackard-analysis/blob/5501c747ea65b6194b28a1f553e43b99289a9b30/Data/mentorship_eligibility.csv) was created, and a snippet of it is included below:



![alt_text](https://github.com/farwaali08/pewlett-hackard-analysis/blob/9ac74aea7263ac7ee40f8ecb0909877c2bd7b4ab/mentors.png)


The data indicates that there are only `1,549` employees that are eligible to provide mentorship, which will not be sufficient to accommodate the volume of new hires. The majority of the mentors (`797` specifically,) are in senior positions, namely Senior Engineer, Senior Staff, and Technique Leader. It can be assumed that these positions are more specialized than their junior counterparts, and would be better filled with internal candidates, through promotions. In this way, existing staff, who already hold the knowledge and qualifications, can move up within the company, and their vacancies can be filled by new hires. This potentially creates new mentors out of the staff that are being promoted as well, although this will require that a robust transition plan be in place.

Before any additional decisions are made, further analysis is recommended. Additional considerations include the following: the list of retirees and potential mentorships should be modified to include the departments of these employees. This will allow us to assess staffing priority by department, as well as identify disparities in available mentors by department type. Given that the ratio between the number of potential new hires and the total number of available mentors is not favourable, another recommendation would be to expand the mentorship eligibility criteria. This can be done by either modifying the age range, or including additional criteria, such as performance, or the years worked in a specific role.
