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
  
The following school summary DataFrame snippets show the impact of the revision:
 
  i. Original School Summary(Thomas High School Row):
 
 |School Type|Total Students|Total School Budget|Per Student Budget|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|Spending Ranges (Per Student)|   School Size    |
|-----------|-------------:|-------------------|------------------|-----------------:|--------------------:|-------------:|----------------:|----------------:|-----------------------------|------------------|
|Charter    |          1635|$1,043,130.00      |$638.00           |             83.42|                83.85|         93.27|            97.31|            90.95|$630-644                     |Medium (1000-2000)|
  
  ii. Modified School Summary(Thomas High School Row):
  
  |School Type|Total Students|Total School Budget|Per Student Budget|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|Spending Ranges (Per Student)|   School Size    |
|-----------|-------------:|-------------------|------------------|-----------------:|--------------------:|-------------:|----------------:|----------------:|-----------------------------|------------------|
|Charter    |          1635|$1,043,130.00      |$638.00           |             83.35|                83.90|         66.91|            69.66|            65.08|$630-644                     |Medium (1000-2000)|

The correction for the academic dishonesty has impacted the school summary for Thomas High School in the following ways:
  - Overall passing percentage dropped 25.87% from 90.95% to 65.08%
  - Percentage of students who passed reading dropped 27.65% from 97.31% to 69.66%
  - Percentage of students who passed math dropped 26.36% from 93.27% to 66.91%
  - Average reading score increased 0.05% from 83.85% to 83.90% 
  - Average math score dropped by 0.07% from 83.42% to 83.35%

Recalculating the highand low performing schools has also negatively affected Thomas High School's performace relative to other schools:
  - Pre-correction ranking: 2/15
  - Post correction ranking 8/15
  
 Math and Reding Scores By Grade:
  - Thomas High School grade 9 reading score: NaN
  - Thomas High School grade 9 math score: NaN
 
 Math and Reading Scores by School Spending in $630-$644 Range:
        
  i. Original Spending Analysis:
      
   |Spending Range|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
   |-------------:|-----------------:|--------------------:|-------------:|----------------:|----------------:|
   |      $630-644|              78.5|                 81.6|            73|               84|               63|
   
  ii. Modified Spending Analysis:
  
   |Spending Range|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
   |-------------:|-----------------:|--------------------:|-------------:|----------------:|----------------:|
   |      $630-644|              78.5|                 81.6|            67|               77|               56|

Scores Based on Spending were affected in the following ways:
 - Overall percentage of students who passed dropped 7% from 63% to 56%.
 - Precentage of students who passed reading dropped 7% from 84% to 77%.
 - Percentage of students who passed math dropped 6% from 73% to 67%.
 - Average reading and math scores were not significantly impacted.
  
 Scores Based on School Size in the Medium(1000-2000) Range
 
  i. Original Size Analysis for Medium(1000-2000) Range
    
   |           Range|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
   |---------------:|-----------------:|--------------------:|-------------:|----------------:|----------------:|
   |Medium(1000-2000|              83.4|                 83.9|            94|               97|               91|
   
  ii. Modified Size Analysis for Medium(1000-2000) Range
   |           Range|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
   |---------------:|-----------------:|--------------------:|-------------:|----------------:|----------------:|
   |Medium(1000-2000|              83.4|                 83.9|            88|               91|               85|
   
Scores for Large(2000-5000) and Small(<1000) schools remained the same while scores for Medium(1000-2000) schools were affected in the following ways:
  - Overall percentage of students who passed dropped 6% from 91% to 85%.
  - Precentage of students who passed reading dropped 6% from 97% to 91%.
  - Percentage of students who passed math dropped 6% from 94% to 88%.
  - Average reading and math scores were not significantly impacted.

Math and Reading Scores by School Type:

  i. Original Type Analysis:
  
   |    Type|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
   |-------:|-----------------:|--------------------:|-------------:|----------------:|----------------:|
   | Charter|              83.5|                 83.9|            94|               97|               90|
   |District|              77.0|                 81.0|            67|               81|               54|
   
  ii. Modified Type Analysis:
   
   |    Type|Average Math Score|Average Reading Score|% Passing Math|% Passing Reading|% Overall Passing|
   |-------:|-----------------:|--------------------:|-------------:|----------------:|----------------:|
   | Charter|              83.5|                 83.9|            90|               93|               87|
   |District|              77.0|                 81.0|            67|               81|               54| 
  
Scores for District Schools were not affected while the scores for Charter Schools were affected in the following ways:
  - Overall percentage of students who passed dropped 3% from 90% to 87%.
  - Precentage of students who passed reading dropped 4% from 97% to 93%.
  - Percentage of students who passed math dropped 4% from 94% to 90%.
  - Average reading and math scores were not significantly impacted.

