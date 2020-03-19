# School_District_Analysis
## Project Overview
The math and reading scores of Thomas High School ninth grade have been changed. While administrators do not know the full extent of this academic dishonesty, they want to uphold the standards of state testing and have requested help. It has been decided the best approach is to replace the reading and math scores with NaN values. To accomplish this we will:
- Create a copy of PyCitySchools.ipynb to carry out further analysis
- Correct the students' names so there are no professional prefixes or suffixes.
- Replace the reading and math scores for ninth graders at Thomas High School with NaN.
- Merge the clean student data with the school dataset.
- Recreate District and School Summmary DataFrames and explain:
  - How is the district summary affected?
  - How is the school summary affected?
- Recalculate high and low performing schools and explain:
  - How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
- Recalculate the scores by grade, scores by school spending, scores by school size, and scores by school type and explain how the following are affected:
  - Math and Reading Scores by Grade
  - Scores by School Spending
  - Scores by School Spending
  - Scores by School Type
## Resources
  - Data Source: schools_complete.csv, students_complete.csv
  - Software: Python 3.7.6, Jupyter Notebook 6.0.3
  - Libraries: Pandas, Numpy
## Summary
  The following district summary tables show the impact of the revision:
  
  i. Original District Summary:
  
|Total Schools|Total Students| Total Budget |Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
|------------:|--------------|--------------|-----------------:|--------------------:|-------------:|----------------:|---------------:|
|           15|39,170        |$24,649,428.00|             78.99|                81.88|         74.98|            85.81|           65.17|
  
  ii. Modified District Summary:
  
Total Schools|Total Students| Total Budget |Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
|------------:|--------------|--------------|-----------------:|--------------------:|-------------:|----------------:|---------------:|
|           15|39,170        |$24,649,428.00|             78.93|                81.86|         73.88|            84.65|           64.09|

The correction for the academic dishonesty has impacted the district summary in the following ways:
  - overall passing percentage has dropped 1.10% from 65.17% to 64.09%.
  - Percentage of students who passed reading dropped 1.16% from 85.81 to 84.65.
  - Percentage of students who passed math dropped 1.10% from 74.98 to 73.88.
  - Average reading score dropped by 0.02% from 81.88 to 81.86.
  - Average math score dropped by 0.06% from 78.99 to 78.93.
  
    The following school summary tables show the impact of the revision:
    
    
