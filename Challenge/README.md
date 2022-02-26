# Module 4 | Assignment - PyCitySchools

Use Python and the Pandas library to analyze school district data and showcase trends in school performance.

## OVERVIEW OF PROJECT: SCHOOL DISTRICT ANALYSIS

The school board has a suspicion of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders, this after reviewing some reports from all schools.

The next analysis will be used to validate or not, the above suspicions. The strategy to analyze all data collected is to exclude the math and reading scores for Thomas High School, while keeping the rest of the data intact. Once this specific data is isolated, we will run another school district analysis to describe how these changes affected the overall analysis.

## RESULTS

#### •	How is district summary affected?

After isolating the 461 reading and math grades for 9th grades in Thomas High School (replacing grades wiht NaN values) we starting analizing grades data for 15 schools and 38,709 students in the school district.

The next table, shows a summary for this data (average grades, percentage of students passing both classes and overall passing rate) for all schools in math and reading:

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/district_summary_df.png?raw=true) 

After reviewing the general data, the percentage of passing math in the district and the overall passing show an important decrease, which will be analyzed to a deeper lever to infer anomality in these grades.

#### •	How is the school summary affected?

When analysing the school summary data, it can be summarized as follow:

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/per_school_summary_df.png?raw=true) 

In general, Thomas High School, after isolating the 461 reading and math grades for 9th grades and comparing with other schools, with no distinctions, math and reading scores do not show an important difference compared with other schools.

#### •	How does replacing the ninth grader's math and reading scores affect Thomas High School's performance relative to the other schools?

When excluding all 9th graders from THC, and running the analysis again same results show up f0r the district summary.

#### •	How does replacing the ninth-grade scores affect the following:

###### Math and Reading scores by grade

After analyzing the math scores by grades for the 15 schools and not including 9th grades we get the next table:

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/math_scores_by_grade_with_NaN.png.png?raw=true) 

The results show that in general math grades has a higher standard deviation of 3.38 for the 15 schools in the data set. Thomas High School had an average grade of 83 points for 9,10 and 11th grades, which is above the mean in the district, altogheter with other four schools. Based on these numbers, no special data suggest some potential fraud in grades.

The reading scores by grade show a more stable statistic results withing all the district with a  standard deviation of only 1.57 points, with THS with one of the highest grades. No special data show fraud in the reading scores for this school.

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/reading_scores_by_grade_with_NaN.png?raw=true) 

###### Scores by School Spending

After grouping the data set by spending, the data shows that the biggest the per capita budget, the lowest percentage of passing for both classes as shown in the next table:

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/Grades_percapita_budget_range.png?raw=true) 

###### Score by School Size

If grouping by school size, no special data can be noted for the analysis.

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/Grades_perSchool_Size.png?raw=true) 

###### Score by School Type

The analysis by school type shows interesting data. If the dataset is grouped by the type of schools, as summary, the math and reading scores show a very similar trend and ranges between the 7 schools.

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/Grades_perType.png?raw=true) 

But, when we analyze the results grouping by charter schools, Thomas High School has an important  difference for the percentage passing math compared to the other schools. THS has a very low 67% of passing, compared to the otyhers 7 schools which have an average of 93%, as shown in the next table.

![alt text](https://github.com/Robcaze1980/School_District_Analysis/blob/main/Challenge/Images_challanges/Summary%20for%20Charter%20Schools.png?raw=true) 

## SUMMARY OF RESULTS

After replacing ninth-grades scores we can make next conclusions, based on the analysis methodology used:

- The scores data set for grades, per capita budget and school size don't show a relevant anomality to infer dishonesty in THS ninth-graders.

- If the score data set is grouped by school type, THS show an very important anomality for math scores (25% lower), when compared with other schools.

I strungly suggest to develop another deeper analysis to understand this relevant finding.
