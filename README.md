# School_District_Analysis

The school district summary will be a high-level snapshot of the district's key metrics:

Total number of students
- 39,170
Total number of schools
- 15
Total budget
- $24,649,428
Average math score
- 81.87784018381414
Average reading score
- 78.98537145774827
Percentage of students who passed math
- 29,370 / 39,170 = 74.98%
Percentage of students who passed reading
- 33610 / 39170 = 85.80%
Overall passing percentage
- 65.17%





## Overview of the school district analysis:

The purpose of this jupiter notebook analysis is to present an overview of key metrics betweem student and school data. Data from two .csv files were read, cleaned, and merged using Python to create tables. The student data was matched to the school to calculate math/reading scores and provide insights about each school's size, budget, and type.

## Results
Thomas High School's ninth grade scores needed to be removed from the dataset.
- How is the district summary affected?
    - The district summary decreased from 65.17% to 64.9%
![Image of District Summary Before](/Resources/districtsummary_before.PNG)
![Image of District Summary After](/Resources/districtsummary_after.PNG)
- How is the school summary affected?
    - Since Thomas High School's ninth graders scores were removed their overal school performance decreased.
- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
    - Before including the averages from 10th-12th grade students, Thomas High School's Overall Passing Percent decreased from 90.94% to 65.07%. Once the 10th-12th grade students were recalculated back into the dataframe, the school remained the 2nd top school.
![Image of THS Before](/Resources/ThomasHighSchoolBefore.PNG)
![Image of THS After](/Resources/ThomasHighSchoolAfter.PNG)
How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
    - The average math score decreased by 0.067412%
    - The average reading score increased by 0.047152%
- Scores by school spending
    - Thomas High School has a budget of $638 per student which puts the school in the $630-$644 Spending Range. The Overall Passing Percentage saw a decrease from 62.857656% to 62.778233%.
![Image of Spending Ranges Before](/Resources/spendingranges_before.PNG)
![Image of Spending Ranges After](/Resources/spendingranges_after.PNG)
- Scores by school size
    - Thomas High School has 1635 total students, so the Medium (1000-2000) would be affected by the removal of this school's data. The column Overall Passing Percent went down for Medium School Size went down from 90.621535% to 90.557997%
![Image of School Size Before](/Resources/schoolsize_before.PNG)
![Image of School Size After](/Resources/schoolsize_after.PNG)
- Scores by school type
    - Thomas High School is a charter school so Charter school averages were affected. The Overall Passing Percent went down from 90.432244% to 90.392533%
![Image of School Type Before](/Resources/schooltype_scoresbefore.PNG)
![Image of School Type Before](/Resources/schooltype_scoresafter.PNG)
## Summary
Within the high-level overview of school and student data, Thomas High School's 9th grade student data negatively  impacted the columns regarding, Average Math Score, % Passing Math, % Passing Reading, and % Overall Passing. When using only 10th - 12th grade students, Thomas High School's Average Reading Score increased. The % changes in the combined schools' data can only be seen without formatting the relative dataframes. By not including 9th grade student grades from one school an overview of the overall performance of 9th grade students among these schools would be incomplete. Thomas High School's data can only be evaluated by the scores of it's 10th-12th grade students, but the school remains a top school.