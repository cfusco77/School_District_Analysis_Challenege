## Project Overview
Maria a data scientist for a city school district was asked to perform an analysis on school performance, namely math and reading scores. This analysis will aid in the determination of sachool funding so its imperative that the analysis by thorough and without bias. 

The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked us to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Maria would like us to repeat the school district analysis and describe how these changes affected the overall analysis.

Below I have provided Marias's initial analysis compared to a secondardy analsyis having replaced THS ninth graders' grades with NaNs. 

## Results

### District Summary 
Replacing the THS 9th grade test results with NaNs has little to no impact on the average math and reading scores of THS students, which change by a fraction of a percentage point, meaning the dishonest data we replaced with NaNs must have been close to the averages. Had the dishonest data been significantly higher or lower than the mean, replacing it would have been more impactful to the district summary. In addition THS ninth graders only make 461 of the total 39,170 students. So we might expect that replacing their grades with NaNs would not be overwhelmingly consequential. 
##### Original District Summary
![Original District Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/PYCity_DistrictSummary_Original.png)
##### District Summary Having replaced THS Ninth Graders grades with NaNs 
![THSEdit District Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/PyCity_DistrictSummary_THSEdit.png) 

--- 

### School Summary 
Only THS has the possibility of being impacted by this edit, all other schools metrics should remain the same. 
Initially when we calculated the school summary having replaced the THS ninth graders grades with NaNs, the % passing math, % passing reading, and overall passing percent for THS results looked suprisingly low, this is because we did not use the new student counts when calculating these metrics. We recalculated and replaced these results using only the scores of the 10th-12th graders from Thomas High School.
#### Original School Summary 
![Original School Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/Original%20School%20summary%20.png) 
#### Having replaced THS grades with Nans but having not yet adjusted the student count in percent calculations
![Initial THS School Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/THS_summary_before.png)
#### After recalculating THS percentages using 10th-12th graders
![After THS recalculations](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/THS_summary_after.png)

---

### School Rankings
Replacing the ninth grader' math and reading scores did not change Thomas High School's performance relative to other schools. When we examine the 5 top schools ranked by overall performance, Thomas high School still ranks number 2. 
#### Original Top School Rankings
![Original top 5](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/Original%20Top%205%20Schools.png) 
#### After Replacing THS Ninth Graders' Grades with NaNs 
![TopSchools](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/TopSchools.png)

---

### Math and Reading Scores by Grade 
All average grades across 9th - 12th remained the same for every school with the exception of THS where we replaced the ninth grade scores with NaNs because we believe the data to be compromised. 

---

### Scores by School Spending 
THS belongs to the $630 - $644 bin which, after having performed the secondary analsyis, sees no statisitically signifcant change to the percent passing math, reading or overall. 
#### Original School Spending 
![Original School spending](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/Original%20Spending%20Ranges%20.png) 
#### After Replacing THS Ninth Graders' Grades with  NaNs 
![After School Spending](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/New%20Spending%20summary%20.png) 

---

### Scores by School Size 
THS belongs to the medium sized school bin which, after having performed secondary analysis, sees no statstitically significant change to the percent passing math, reading or overall. 
#### Original School Size Summary 
![Original school size summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/Original%20Size%20Summary.png)
#### After Replacing THS Ninth Graders' Grades with NaNs 
![New School Size Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/New%20Size%20Summary%20.png) 

---

### Scores by School Type 
THS belongsa to the type charter which, after having performed secondardy analysis, sees no statistically significant change to the percent passing math, reading, or overall. 
#### Orginal School Type Summary 
![Original Type summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/Original%20District%20summary%20.png) 
#### After Replacing THS Ninth Graders' Grades with NaNs 
![New Type Summary](https://github.com/cfusco77/School_District_Analysis_Challenege/blob/main/Resources/New%20District%20Summary.png)



### Summary
There were very minimal changes to replacing the Thomas High School ninth graders' grades with NaNs, however a worth while excercise in an effort to protect data integrity. Adjusting the grades did reduce the number of students used in our calculations from 39,170 to 38,709. We saw in some areas such as the district summary average math scores a decrease by a fraction of a pecentage point. Almost all discrepancies were so small that when we applied the formatting requested by the sachool district the results were identical. 
