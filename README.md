# School_District_Analysis.
In this analysis, I helped Maria conduct a study on the school district which include

- An overview of the key metrics for each school (per_school_summary_df)
- Top 5 and bottom 5 performing schools, based on the overall passing rate (top_schools.head() and bottom_schools.head())
- The average math score received by students in each grade level at each school (math_scores_by_grade)
- The average reading score received by students in each grade level at each school (reading_scores_by_grade)
- School performance based on the budget per student (spending_summary_df)
- School performance based on the school size (size_summary_df)
- School performance based on the type of school (type_summary_df)


# Challenge
As the grades of the ninth graders at Thomas High School have been changed, Maria and her supervisors now face a challenge on the accuracy of the analysis. My new task is to remove the ninth-grade math and reading scores from Thomas High School while keeping all other data associated with the ninth-grade students and Thomas High School intact. I have successfully replace the ninth graders' math and reading scores with null value while keeping the other data intact. And below are my observations on the impact of this removal:
- The district summary figures decrease slightly with percentage of students passing math or reading or both dropping by 1%
- For the school summary, only Thomas High School numbers are affected with percentage of students passing math or reading or both significantly dropping from 95 to 98 range to 67 to 70 range, a 28% drop! Whereas, the averages for math and reading score barely change.
- The removal of ninth graders' math and reading grade negatively affects Thomas High performance. Thomas High School falls from the second best-performing school to the lowest-performing school.
- The effect of the removal on: 
    - Math and Reading Scores by Grade: math and reading scores for all grade at all schools are the same except for Thomas High School's ninth graders, which  replaced with NaN
    - Scores by School Spending: while the average scores remain the same, the percentage of students passing math or reading or both drops for the $630 to $644 range, approximately 7% decrease
    - Scores by School Size: average scores remain the same for all size schools while the percentage of students passing math or reading or both drops for the medium size schools, approximately 5.4% decrease
    - Scores by School Type: similar observations for the above, average scores remain the same for charter and district schools while the percentage of students passing math or reading or both drops for the charter schools, approximately 3.7% decrease
