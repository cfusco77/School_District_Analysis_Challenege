# School_District_Analysis_Challenege
## Overview of the school district analysis: Explain the purpose of this analysis.
The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked us to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Maria would like us to repeat the school district analysis and describe how these changes affected the overall analysis.

## Results
### How is the district summary affected?
Replacing the THS 9th grade test results with NaNs has little to no impact on the average math and reading scores of THS students, which change by a fraction of a percentage point, meaning the dishonest data we replaced with NaNs must have close to the averages. Had the dishonest data been significantly higher or lower than the mean, replacing it would have been more impactful to the district summary. In addition THS ninth graders only make 461 of the total 39,170 students. So we might expect that replacing their grades with NaNs would not be overwhelmingly consequential. 

#### Original District Summary 
![Original District Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/PYCity_DistrictSummary_Original.png)

#### District Summary Having replaced THS Ninth Graders grades with NaNs 
![THSEdit District Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/PyCity_DistrictSummary_THSEdit.png) 

--- 

### How is the school summary affected?
Only THS has the possibility of being impacted by this edit, all other schools metrics should remain the same. 
Initially when we calculated the school summary having replaced the THS ninth graders grades with NaNs, the % passing math, % passing reading, and overall passing percent for THS results looked suprisingly low, this is because we did not use the new student counts when calculating these metrics. We recalculated and replaced these results using only the scores of the 10th-12th graders from Thomas High School. 

#### Intitial School Summary, before replacing THS calculations
![Initial THS School Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/THS_summary_before.png)

#### After recalculating THS percentages using 10th-12th graders
![After THS recalculations](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/THS_summary_after.png)


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Replacing the ninth grader' math and reading scores did not change thomas high School's performance relative to other school. When we examine the 5 top school ranked by overall performance, Thomas high School still ranks number 2

![TopSchools](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/TopSchools.png)
---

### How does replacing the ninth-grade scores affect the following:
Average Math and Reading Scores By Grade: Looking at math and reading scores by grade grouped by school, we should see no changes from our initial analysis other than that in the 9th grade column THS shows NaNs

When reviewing our secondary analysis, if percent passing rates changed by less than 1 full percentage point I considered them unimpacted. 
* Scores by School Spending: Unimpacted 
* Scores By School Size: Unimpacted 
* Scores by School Type: Unimpacted 


###Summary  
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
