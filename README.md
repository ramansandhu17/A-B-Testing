# A/B Test: Email Subject Line Optimization

## Objective
To improve email open rates by testing two subject lines using a controlled A/B test.
Project Statement: We will compare open rates between 2 email subject lines
Metric: We will decide on open rate  which one has more open rate
Group A: Control group; Group B: Test Group
Test: Two proportion z-test
Internal Notes: Two Proportion z-test is a statistical test that checks whether the difference between two proportoms is statistically significant 


## Summary
- Subject Line A: "Following up on our last conversation"
- Subject Line B: "Fresh flavors just arrived"
- 100 emails sent per group
- Open rates: A = 24%, B = 31%

## Statistical Test
- Z-score: -1.1085306154508543
    
- P-value: 0.26763272469108135
- Result: Not statistically significant

- ### How to Interpret This:
- The **Z-score** tells us how many standard deviations the observed difference is from the expected difference (which is 0 under the null hypothesis). How far away are our results from what we would expect
- if there was no differenece at all. Negative Z- score = test group was better but in our case not by a lot
- A **p-value of 0.268** means there's a 26.8% chance of seeing this difference (or more extreme) if there were actually **no real difference** between the subject lines.
-   5 year old version - this is not a wa
- Since the p-value is **greater than the common threshold of 0.05**, we **fail to reject the null hypothesis**.

## Conclusion
Although Subject Line B had a higher open rate, we cannot conclude it performs better with statistical confidence. The difference may be due to chance.

## Tools Used
- Python (pandas, numpy statsmodels)
- Jupyter Notebook
- Simulated email data
