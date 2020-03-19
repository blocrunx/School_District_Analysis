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
  1. Original District Summary:
  
|otal Schools|Total Students| Total Budget |Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
|------------:|--------------|--------------|-----------------:|--------------------:|-------------:|----------------:|---------------:|
|           15|39,170        |$24,649,428.00|             78.99|                81.88|         74.98|            85.81|           65.17|
  
Total Schools|Total Students| Total Budget |Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
|------------:|--------------|--------------|-----------------:|--------------------:|-------------:|----------------:|---------------:|
|           15|39,170        |$24,649,428.00|             78.93|                81.86|         73.88|            84.65|           64.09|
