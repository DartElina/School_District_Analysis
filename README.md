# School_District_Analysis
## Overview of the school district analysis: Explain the purpose of this analysis.

The school board has notified our team that the students_complete.csv file shows evidence of tampering after we had completed a district analysis. It seems that the ninth graders of Thomas High School's grades have been altered. We have been asked to replace the math and reading scores for Thomas High School ninth graders with NaNs while keeping the rest of the data intact. Once we’ve replaced the math and reading scores with NaNs we repeated the school district analysis that produced the following report to describe how these changes affected the overall analysis.

We created a code that would replace the grades in the math and reading scores with null values so that the potentially tampered grades did not skew our analysis. The code identified the grades of 461 students and replaced them with null values. Image of resulting list of students iwth null grades:

![image](https://github.com/DartElina/School_District_Analysis/blob/213f1d799f720d4d50678c3f2897aafc405e4e86/Resources/code%20example%20null%20values%209%20AND%20Thomas.png)


## Results: 

### How is the district summary affected?

- Our analysis was completed before we removed the allegedly tampered grades. The district results looked like this:

![i](https://github.com/DartElina/School_District_Analysis/blob/213f1d799f720d4d50678c3f2897aafc405e4e86/Resources/District%20Results%20w%20Tampered%20Grades.png)

- Once tampering was identified we needed to analyze the district results with out the tampered grades potentially skewing the results. Here are the district results after removing potentially tampered grades:

![i](https://github.com/DartElina/School_District_Analysis/blob/213f1d799f720d4d50678c3f2897aafc405e4e86/Resources/District%20Summary%20After%20NaNs.png)

- The results shows that in a district of 39,170 students, removing the grades of 461 ninth grades has lowered the percentages of the district. "% Overall Passing" reduced .3% Additional analysis must be done to measure the significance of this shift. 

### How is the school summary affected?
- ThomasHS results including tampered grades:

![i](https://github.com/DartElina/School_District_Analysis/blob/213f1d799f720d4d50678c3f2897aafc405e4e86/Resources/Thomas%20Stats%20with%20tampered%20Grades.png)

- ThomasHS after ninth grader grades nulled and analysis was completed again not including the 461 students with null grades:

![i](https://github.com/DartElina/School_District_Analysis/blob/135a4bcc940b05e64c36c98e8ec8143e8a475639/Resources/Thomas%20After.png)

- If we weren't careful we'd have nulled the values of the ninth graders test scores and ran the analysis and the result could have been averaging the nulls into the school data and that looked like this, until we corrected the values for the chart. 

![i](https://github.com/DartElina/School_District_Analysis/blob/4c855bb6048ca981450b22b16b6e29ee227af0b1/Resources/THS%20with%20NaN%20calculated%20into%20school%20average.png)

- Further Analysis:

  - How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
      
      Before (with tampered grades)
![before](https://github.com/DartElina/School_District_Analysis/blob/4c855bb6048ca981450b22b16b6e29ee227af0b1/Resources/Top%205%20including%20tampered%20grades.png)
      
      After (excluding ninth grade)
![after](https://github.com/DartElina/School_District_Analysis/blob/4c855bb6048ca981450b22b16b6e29ee227af0b1/Resources/Top%205%20after%20tampered%20grades%20removed.png)

  - Before and after these analysises Thomas High School is in second place of the Top 5 in the district. There was no significant change in THS standing among the other schools.

- How does replacing the ninth-grade scores affect the following:

  - Math and reading scores by grade
     - Math and Reading score charts show NaN in the Thomas High School Row, 9th grade column. 
  
![math](https://github.com/DartElina/School_District_Analysis/blob/4c855bb6048ca981450b22b16b6e29ee227af0b1/Resources/Math%20Scores%20with%20NaN.png)
![reading](https://github.com/DartElina/School_District_Analysis/blob/4c855bb6048ca981450b22b16b6e29ee227af0b1/Resources/reading%20scores%20with%20NaN.png)
   
  - Scores by school spending: Thomas High School spends $638 per student. Results are unchanged. 
  
![spend before](https://github.com/DartElina/School_District_Analysis/blob/7e1c1e0ef71ee7d67dea80a99016bddb82861ecb/Resources/spending%20before%20.png)
![spend after](https://github.com/DartElina/School_District_Analysis/blob/7e1c1e0ef71ee7d67dea80a99016bddb82861ecb/Resources/spending%20after%20.png)

  - Scores by school size: Thomas High School has 1635 students. Results are unchanged. 
  
![size before](https://github.com/DartElina/School_District_Analysis/blob/7e1c1e0ef71ee7d67dea80a99016bddb82861ecb/Resources/size%20before.png)
![size after](https://github.com/DartElina/School_District_Analysis/blob/7e1c1e0ef71ee7d67dea80a99016bddb82861ecb/Resources/size%20after.png)

  - Scores by school type: Thomas High School is a charter school. Results are unchanged. 
  
![type before](https://github.com/DartElina/School_District_Analysis/blob/7e1c1e0ef71ee7d67dea80a99016bddb82861ecb/Resources/type%20before%20.png)
![tpe after](https://github.com/DartElina/School_District_Analysis/blob/7e1c1e0ef71ee7d67dea80a99016bddb82861ecb/Resources/type%20after%20.png)


## Summary: 

Our analysis is not meant to prove whether or not there was tampering with the ninth grader's grades. Maria has requested us to complete this analysis to be sure that results are not skewed by the tampering. 

Notable changes are 
1. the .3% reduction in % overall passing at the school level at Thomas High School. 
2. the .3% reduction in % passing reading scores at the school level at Thomas High School. 
3. On the district level we see a a reduction of % Overall Passing by .3% as well. 
4. Also notable that there was NO change in the scores by school spending, school size, or school type. 

I believe more analysis should be done to confirm there is no tampering with other grades at THS or other schools that could be continuing to affect the analysis.
 
