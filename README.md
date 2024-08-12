# STA 141B Group Project: College Scorecard Data Analysis

We are interested in analyzing the overall value of an undergraduate degree and whether attending college is a worthwhile investment in the long run for all students, especially ones that require students to take out loans to pay for their college tuition. With that, we developed functions to query financial variables from the College Scorecard web API to perform a comprehensive analysis of the value of college to answer the following questions:

* How have student debt and post-graduate income changed over the past 10 years?
* Is there any correlation between median projected income, completion rate, and cost of tuition?
* Is there a significant difference in median earnings (10 years after graduation) and student debt in public vs. private institutions?

:robot: Tools & Libraries: Python, requests, matplotlib, scipy, seaborn, numpy, pandas

:robot: Data Source: College Scorecard, an online database maintained by the United States Department of Education

## Data Analysis
### Student Loan Debt vs College Graduate Income

While student loan debt and college graduate income have seen substantial increases over the past 10 years, student loan debt has increased by nearly 30% since 2011 while post-graduate income has only increased by 20%. This finding indicates that college is getting more expensive with time, and while college graduates are earning more year-by-year, the relationship between these factors is not one-to-one as college debt is increasing at a more rapid rate.

### Completion Rate vs Income vs Cost of College

The cost of tuition and completion rate are significantly positively correlated, a percent increase in tuition increases the completion percentage by about a percent. Next, cost and income are significantly positively correlated, $1,000 increase in tuition increases the expected income by about $420. We also see that completion rate and income are significantly positively correlated, a percent increase in completion rate increases the expected income by 350 dollars. T-tests for the correlation coefficient were used to test if the variables above were linearly correlated, we rejected null hypothesis of non-correlation for all three results.
 
Additionally, we observe a positive correlation between higher percentage of engineering students at the college and income, and a negative correlation between higher percentage of humanities students at the college and income.

### Income and Debt in Public vs Private Institutions

Students that graduated from public schools have average median earnings of $50663.65 which is only slightly lower than the earnings of students graduated from private schools, $51259.33. We used the independent T-test to test for a statistically significant difference in the means between public and private institutions. The independent T-test shows that there is no statistically significant difference in the average median earnings between public and private institutions as the p-value > 0.05.

However, the independent T-test shows that there is a statistically significant difference in the average student loan debt between public and private institutions.

## Conclusion

In conclusion, despite the significant increase in student debt and post-graduation income over the years analyzed, it is still worth attending college. Our analysis found a positive correlation between post-graduation income, completion rate, and the cost of college. It is possible to find lower-costing, high-income colleges, especially in nursing and engineering-based STEM programs. Attending these colleges gives the highest income with the lowest debt.

Furthermore, we found that while median income does not differ much between public and private institutions, student debt is significantly higher in private institutions. However, it is possible to graduate from a private institution with low student debt.

Therefore, finding a balance between the amount of debt you incur and the amount you will make largely depends on the type of college you attend and the degree you choose to graduate with. It is important to research before attending college to ensure that you make an informed decision about your future financial stability. Overall, college is still worth it, and with careful planning and consideration, students can find success both academically and financially after graduation.
