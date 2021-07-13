# School_District_Analysis_Challenege
## Overview of the school district analysis: Explain the purpose of this analysis.
The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked us to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Maria would like us to repeat the school district analysis and describe how these changes affected the overall analysis.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.
### How is the district summary affected?
Replacing the THS 9th grade test results with NaNs has little to no impact on the average math and reading scores, which change by a fraction of a percentage point, meaning the dishonest data we replaced with NaNs must have close to the averages. Had the dishonest data been significantly higher or lower than the mean, replacing it would have been more consequential to the district summary. 

### How is the school summary affected?
Initially when we calculated the school summary, the % passing math, % passing reading, and overall passing pcercent results looked suprisingly low. We recalculated and replaced these results using only the scores of the 10th-12th graders from Thomas High School. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Replacing the ninth grader' math and reading scores did not change thomas high School's performance relative to other school. When we examine the 5 top school ranked by overall performance, Thomas high School still ranks number 2

### How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type
Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
