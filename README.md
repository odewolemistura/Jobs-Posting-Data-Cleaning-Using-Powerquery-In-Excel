# Jobs-Posting-Data-Cleaning-Using-Power Query-In-Excel
## Table of contents
- [Project Overview](project-overview)
- [Data Source](data-source)
- [Tool](tool)
- [Data Cleaning Methodology](data-cleaning-methodology)
- [Insights Generation](insights-generation)
- [Key Learnings](key-learnings)
## Project Overview
This project demonstrates the crucial role of clean data in analytical decision-making and spotting trends. Working with real-world job postings for roles like Data Analyst, Data Scientist, Machine Learning Engineer, and Data Engineer, the objective was to transform messy, inconsistent data into a structured format that supports accurate salary insights.
By organizing and standardizing the data across job roles, company sizes, and locations, the project enabled the discovery of meaningful patterns and comparisons. It reinforces a key principle: clean data is the foundation for reliable insights and smarter business decisions.
## Data Source
The dataset contains the following columns: Job Title,Salary Estimate,Job Description,Rating Company Name, Location, Headquarters, Company Size, Year Founded, Type of Ownership, Industry, Sector, Revenue, Competitors.
## Tool
Microsoft Excel Power Query
## Data Cleaning Methodology
This cleaning process is the main objective of this project and it was done with the specific goal of getting accurate salary insight which answers specific business questions.
- I duplicated the original dataset and began cleaning with the duplicate table so that i can always refer to the source data in case of neccesities.
- I checked for duplicate rows and removed them to ensure accurate insight generation
- I Extracted salary values and split into minimum and maximum salary columns.
- I splited the minimum and max salary using column from example
- I filtered out rows with outliers to avoid false analysis
- I changed datatype and replaced K with the correct integer ( *1000)
- I grouped the job tiles into job roles using add conditional column
- I removed rows withs unknown employee size
- I Removed state from the location column extract using conditional formatting and split
- I Rearranged columns to make it related and reader friendly
  ## Insights Generation
### Salary by job role
- I created a new table by referencing the cleaned
- I selected the columns needed to generate my insight
- I used the group by function to calculate the average minimum and maximum salary
- I added detailed sub-tables (AllRole columns) for deeper drill-downs
### Salary by company size
- I created a new table by referencing the cleaned
- I selected the columns needed to generate my insight
- I used the group by function to calculate the average minimum and maximum salary by company size
-  I added detailed sub-tables (AllRole columns) for deeper drill-downs
### Salary by state
- The state full name is not present in the the source table but in another table (state mapping table) so i merged the cleaned source table and the state mapping table using merge queries in power query. i merged the two tables using the state name abbrevation which is present in both tables. 
- I referenced the merged table and selected the needed columns to generate this insight.
- For those working in states not included or remote workers, i used conditional column to name them 'others'.
- I added detailed sub-tables (AllRole columns) for deeper drill-downs
### Salary by size and role type
- I referenced the cleaned table
- I selected the columns needed to generate my insight
- I used the group by function to calculate the average min and max salary by size
### Key Learnings
Data cleaning is the backbone of reliable data analysis.
- clear cleaning workflow prevents errors later.
- Power Query is a powerful, no-code tool for real-world data transformation.
- Real-world datasets will always be messy — that's part of the challenge!




