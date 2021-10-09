# Pandas---Challenge
# PyCitySchool
# Intro
This is an analysis of district-wide standardized test results. The  school board and mayor are looking to this analysis to make strategic decisions regarding future school budgets and priorities.  This report will aggregate the data and analyze trends in school performances.
 
# Overview Data
Two csv files were used for analysis. One was a  high school statistics file.  It had school enrollment numbers, the budget, and whether the school was a charter school or distict school (public). The second file was a students statistics file. It had students name, gender, grade, which school they attended and their math and reading scores.


# Methodology
The two csv files were combined into one dataframe with a left join based on the school name. The District Summary required a totalling of the number of schools, number of students, total overall budget, the average math and reading scores by school. The percentage of students passing math and reading was calculated, as well as the overall percentage of students passing both.  The second part of the analysis looked at the same criteria broke down by school.


# Analysis
Total Schools | Total Students | Total Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing
--------------|----------------|--------------|--------------------|-----------------------|----------------|-------------------|------------------
 | 15 | 39170 | $24,649,428.00 | 78.99 | 81.88 | %74.98 | %84.64 | %64.29

The overall passing percentage is below standards.


**Summary of all High Schools**

School Name | School Type | Total Students | Total School Budget | Budget Per Student | Average Math Score | Average Reading Score | % Passing Math | % Passing Math | % Overall Passing
------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | -------
Bailey High School | District | 4976.0 | $3,124,928.00 | $628.00 | 77.05 | 81.03 | %66.68 | %81.93 | %54.64
Cabrera High School | Charter | 1858.0 | $1,081,356.00 | $582.00 | 83.06 | 83.98 | %94.13 | %97.04 | %91.33
Figueroa High School | District | 2949.0 | $1,884,411.00 | $639.00 | 76.71 | 81.16 | %65.99 | %80.74 | %53.20
Ford High School | District | 2739.0 | $1,763,916.00 | $644.00 | 77.10 | 80.75 | %68.31 | %79.30 | %54.29
Griffin High School | Charter | 1468.0 | $917,500.00 | $625.00 | 83.35 | 83.82 | %93.39 | %97.14 | %90.60
Hernandez High School | District | 4635.0 | $3,022,020.00 | $652.00 | 77.29 | 80.93 | %66.75 | %80.86 | %53.53
Holden High School | Charter | 427.0 | $248,087.00 | $581.00 | 83.80 | 83.81 | %92.51 | %96.25 | %89.23
Huang High School | District | 2917.0 | $1,910,635.00 | $655.00 | 76.63 | 81.18 | %65.68 | %81.32 | %53.51
Johnson High School | District | 4761.0 | $3,094,650.00 | $650.00 | 77.07 | 80.97 | %66.06 | %81.22 | %53.54
Pena High School | Charter | 962.0 | $585,858.00 | $609.00 | 83.84 | 84.04 | %94.59 | %95.95 | %90.54
Rodriguez High School | District | 3999.0 | $2,547,363.00 | $637.00 | 76.84 | 80.74 | %66.37 | %80.22 | %52.99
Shelton High School | Charter | 1761.0 | $1,056,600.00 | $600.00 | 83.36 | 83.73 | %93.87 | %95.85 | %89.89
Thomas High School | Charter | 1635.0 | $1,043,130.00 | $638.00 | 83.42 | 83.85 | %93.27 | %97.31 | %90.95
Wilson High School | Charter | 2283.0 | $1,319,574.00 | $578.00 | 83.27 | 83.99 | %93.87 | %96.54 | %90.58
Wright High School | Charter | 1800.0 | $1,049,400.00 | $583.00 | 83.68 | 83.95 | %93.33 | %96.61 | %90.33


**The Top Performing Schools - By % Overall Passing**

School | School Type | Total Students | Total School Budget | Budget Per Student | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing
------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | -------
Cabrera High School | Charter | 1858.0 | $1,081,356.00 | $582.00 | 83.06 | 83.98 | %94.13 | %97.04 | %91.33
Thomas High School | Charter | 1635.0 | $1,043,130.00 | $638.00 | 83.42 | 83.85 | %93.27 | %97.31 | %90.95
Griffin High School | Charter | 1468.0 | $917,500.00 | $625.00 | 83.35 | 83.82 | %93.39 | %97.14 | %90.60
Wilson High School | Charter | 2283.0 | $1,319,574.00 | $578.00 | 83.27 | 83.99 | %93.87 | %96.54 | %90.58
Pena High School | Charter | 962.0 | $585,858.00 | $609.00 | 83.84 | 84.04 | %94.59 | %95.95 | %90.54


**The Bottom Performing Schools - By % Overall Passing**

School | School Type | Total Students | Total School Budget | Budget Per Student | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing
------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | -------
Rodriguez High School | District | 3999.0 | $2,547,363.00 | $637.00 | 76.84 | 80.74 | %66.37 | %80.22 | %52.99
Figueroa High School | District | 2949.0 | $1,884,411.00 | $639.00 | 76.71 | 81.16 | %65.99 | %80.74 | %53.20
Huang High School | District | 2917.0 | $1,910,635.00 | $655.00 | 76.63 | 81.18 | %65.68 | %81.32 | %53.51
Hernandez High School | District | 4635.0 | $3,022,020.00 | $652.00 | 77.29 | 80.93 | %66.75 | %80.86 | %53.53
Johnson High School | District | 4761.0 | $3,094,650.00 | $650.00 | 77.07 | 80.97 | %66.06 | %81.22 | %53.54


**Scores by School Spending**

Spending Ranges (Per Student) | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing
------- | ------- | ------- | ------- | ------- | -------
 <$585 | 83.455399 | 83.933814 | 93.460096 | 96.610877 | 90.369459
$585-630 | 81.899826 | 83.155286 | 87.133538 | 92.718205 | 81.418596
$630-645 | 78.518855 | 81.624473 | 73.484209 | 84.391793 | 62.857656
$645-680 | 76.997210 | 81.027843 | 66.164813 | 81.133951 | 53.526855


**Scores by School Size**

School Size | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing
------- | ------- | ------- | ------- | ------- | -------
Small (<1000) | 83.821598 | 83.929843 | 93.550225 | 96.099437 | 89.883853
Medium (1000-2000) | 83.374684 | 83.864438 | 93.599695 | 96.790680 | 90.621535
Large (2000-5000) | 77.746417 | 81.344493 | 69.963361 | 82.766634 | 58.286003


**Scores by School Type**

School Type | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing
------- | ------- | ------- | ------- | ------- | -------
Charter | 83.473852 | 83.896421 | 93.620830 | 96.586489 | 90.432244
District | 76.956733 | 80.966636 | 66.548453 | 80.799062 | 53.672208


# Results
1. The top performing schools were all Charter schools averaging 1,641 students each.  The bottom performing schools were all District schools averaging 3,852 students.
2. Regarding Scores by School Spending:  Schools with passing rates of 80-90% were only spending $585 to $603 per students.  Schools that spent more than that per student, dropped into the 62% passing range.
3. Regardng Scores by School Size: found that the passing rate was about 90% until the school size went over 2,000 students.  Then the passing rate dropped to 58%.
4. Lastly Scores by School Type indicated that Charter schools had an overall passing rate of 90% compared to District schools where the rates were barely over 50%.

# Conclusion
Passing rates in are not related to money spent in the school system.  The size of the school seems to matter, smaller schools have better overall passing rates.  Possible conclusions are that smaller schools have smaller class sizes, increasing their pass rate.  Or Smaller schools might limit their access based on academics creating a student body that will do better on testing. Two possible strategies are 1. To higher more teachers in the District schools to make the class size smaller; or increase the enrollment to the charter schools, or the availabity of the charter schools to give more students a chance to attend.
