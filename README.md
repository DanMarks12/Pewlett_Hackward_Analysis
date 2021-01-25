# Pewlett_Hackward_Analysis

## Overview of the analysis:
Pewlett Hackward is a massive company with aging employees. In order to get ahead of this, we are tasked with providing analysis on their current work force to create tables and groupings that will provide the company insight moving forward towards the companies "silver tsunami". Not only was it important for us to find employees who are approachign retirement, we need to look at management of these departments, and create mentorship programs so we can better handle the transfer of management moving into the future. We began our research by creating a schema which link all of our database to that we were able to create a relational database. 

![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/ERD_schema.PNG) 

From here, we were able to beging in pgAdmin and create our databases to hold our different DBs. We began by finding our employees who are retiring by joining our employee table and our titles table, looking at only employees born between 1952-1956. 
![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/retirement_titles_sql.PNG)
Upon doing so we found our table included duplicate employees as some employees held multiple positions. So that we are not counting employees twice in our analysis we removed duplicates and created a unique title data which will be more useful for analysis.

![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/unique_titles_sql.PNG) 

![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/unique_titles.PNG)

From here we are able to see that a large portion of our staff will be eligble for retirement in this time: 90,398 employees, 30.13% of the company!

By counting each title we are able to see that Senior Staff (28,255) and Senior Engineer (29,414). These are positions we need to look into developing mentorship programs to replace! 

![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/retiring_titles_sql.PNG)

![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/retiring_titles.PNG)

From here we move into finding solutions. Two department managers suggested the possibility of creating mentorship programs in order to utilize our aging workforce while they are still here and help younger employees get ready to fill the role. 
![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/mentorship_eligibility_sql.PNG)

![](https://github.com/DanMarks12/Pewlett_Hackward_Analysis/blob/main/JPGs/mentorship_eligibility.PNG)

At first we see that some employees are duplicated. This can be seen as a good and bad thing. For one, employees may be eligible to be mentors for multiple positions. On the other hand, after finding the unique employee numbers we find that we only have 1,549 eligble for our mentor ship program. With over 30k employees getting ready for retirement, it will be a scramble to have our 1.5k mentors train enough employees for the coming "tsunami"

## Summary: Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."
How many roles will need to be filled as the "silver tsunami" begins to make an impact?
As stated above, 90,398 employees are eligble for retirement in the coming years. Although the exact date of retirement varies, this wave of retirees presents a massive issue Pewlett & Hackward needs to solve before it is too late. 

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

As it stands now it will be tough for 1,549 mentors to be able to mentor the remaining employees. Pewlett Hackward must look into some aggresive training programs and new hires to get reading for this loss in their workforce. Some positives we can see is many of the almost retirees have been at the company for a long time and have been in multiple roles, so their company has been able to provide an environment of nuturing and growth. Also the fact we found this analysis now before it is too late gives hope that there is time to set plans in place to maintain an efficient workforce. Mentorship programs should be extended to all departments as it is a good idea to use the knowledge these retiree employees have before they are gone. 
