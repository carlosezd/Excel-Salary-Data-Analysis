# Excel-Salary-Data-Analysis
# Introduction 🗣️

This analysis 📊 was created with the objetive of finding new interesting insights about the salary 💵 offered or skills 🥷 needed for data jobs posted in 2023. The data originated from the Excel Data Analysis Course made by Luke Barrouse. 

Link 🔗:    https://www.youtube.com/watch?v=pCJ15nGFgVg&list=PL_CkpxkuPiT-RJ7zBfHVWwgltEWIVwrwb

# Question to answer❓

1. Does having more skills equals to earning a higher salary?
2. What are the top skills of data professionals and how much it pays?
3. What’s the salary for data jobs in different regions?

# Dataset 💽

The data was created by Luke Barousse. The data gather information about different job posting offers related to data across different job platform's. It has columns like:

- Title job
- Date posted
- Salary year average
- Job skills required

Link 🔗https://github.com/lukebarousse/Excel_Data_Analytics_Course/tree/main/0_Resources

# About the Analysis

The analysis begins with the ETL process and ends with the creation of the model, the analysis, and the conclusions obtained.

## ETL & EDA Process 🔄

The dataset is loaded in Power Query. 

![image.png](attachment:7805e9a7-a076-4010-adb4-659d2e04355f:image.png)

Preliminary check of each column with statistical summary.

![image.png](attachment:89026c73-789d-42a4-9733-85059a415fe6:image.png)

Then make a series of transformations:

- Change data types
- Add a index column
- Remove the columns that are not going to be used.
- Filter the data to only rows with salary rate type of “Year”.
- Cleaning of the “job_skills” column via the creation of a new table “job_skills”. For this new table, tools like “replace value”, “Format Text” and “Unpivot Column

![image.png](attachment:8c648ea4-47c9-4e55-b71d-42393467ac80:image.png)

![image.png](attachment:924d312a-57be-4d47-b034-f880288768a8:image.png)

# Analysis 🔎

- Charge “data jobs” and “data skills” tables in Power Query.
- Create a relationship with both tables.

## Does having more skills equals to earning a higher salary?

![05_numberskillspayed.png](attachment:057849f1-c4a2-48d9-b421-5cf9aab9545b:1c23db10-7f41-453f-9886-04cab922c5b3.png)

- 🔨**Tools**: Power Pivot, Pivot tables, Excel Graphs, measures, DAX.
- Create the measure Job Count-Skill Rate that divides “Job Counts” and “Skill Counts”.
- Insert a Scatterplot using the “Median Salary” and “Job Count-Skill ratio”.
- Customize the scatterplot by adding a trend line and adjusting the scale of the X and Y axes. Add a “Data Job” label to each point.
- 

## How much pays the top 10 data skills?

![image.png](attachment:7a665575-5a9e-4fba-9cf2-c99d01d3f7c6:9ec1ca5c-f86b-410e-870d-630eae2447c0.png)

- 🔨**Tools**: Power Pivot, Pivot tables, Pivot Graphs, measures, DAX.
- Establish Create explicit measures for “Median Salary” y “Count Skills.
- Sort Pivot Table by “Median Salary” and Filter Value with TOP 10 by “Count Skills”.
- Minimize the number of elements and optimize distribution for low “Cognitive Load”
- 🎯**Insights**: In general terms, the tool that pays more is “Spark” an open‑source, distributed analytics engine designed for large‑scale data processing. But the most popular skill required is Python and SQL and the salary for this skills is in 5th position.

## **What’s the salary for data jobs in different regions?**

![image.png](attachment:a6f184a6-1e00-485f-b3f7-ade61c1c9d7b:1af4ce4c-a944-4adf-953a-9a396ba3c219.png)

- 🔨**Tools**: Power Pivot, Pivot tables, Pivot Graphs, measures, DAX.
- Create the mesuares “US Median salary” and “No US Median Salary”. Both measures were created to be compared. The first one is static and the second one change by the country filter.
- Create a pivot table that shows the overall "Average Salary", the second table shows only the average salary for the United States because it is the country with the most job postings, and finally, the salary for other countries that are not the United States.
- 🎯**Insights**: Without a doubt, the United States has the most job openings in the data sector. However, Australia, Canada, and European countries also offer well-paying positions.

# Conclusion

These 3 questions about data can reveal new insights that can improve the job search process for any data professional who wants to change jobs to another country or is looking for another job and wants to know which skills they should prioritize learning.
