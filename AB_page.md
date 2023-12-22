## Statistical testing for A/B testing results

**Project description:** 

Context: The Marketing Department ran an A/B experiment to test if their new technique would help increase views and clicks for their advertisement.

Questions: Did the average views and clicks results improve in the tested group? Are these results due to chance?


### 1. Data

Data contains aggregated data on the results of the experiment (user_id), treatment type (group: control and test) and key user metrics(number of views and number of clicks)

### 2. Approach

I used Python to compare the average number of views and the number between the two groups and used the Permutation technique to check if the differences are statistically significant or not with confidence level = 95% or p-value = 0.05

### 2. Results

Conclusion: the test helped increase the average clicks per user but no conclusion on the effect of the test on the average views.

Python code in details 
