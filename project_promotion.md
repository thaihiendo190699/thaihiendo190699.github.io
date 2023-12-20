## FMCG Promotion Analyst

**Project description:** 

Context: The Toothpaste Category Department tried to boost their sales through promotions. They ran a lot of promotions throughout the year, mainly based on their experience and some assumptions. 

Problem: They realized there aren't always good promotions and the one can be good or bad in different stores. They want to know more details about their promotion results and find the best practices to focus their resources on as well as confirm by data some of their assumptions.

**Question 1: What features do successful promotions have in common?**

**Question 2: For a specific item/type of item/area, how should they run the promotion?**

**Question 3: How about the period of after promotions?**

### 1. Analytical approach

**1. Method of analysis:** descriptive analysis, using K-mean to cluster promotions based on their results. Each datapoint for clustering is a promotion for a specific product in a store.

**2. Benchmark:** a successful promotion program need to achieve at least 120% sales compared to the normal sales within the last 30 days and no loss of profits.
- Drawback: some other factors affect sales during the promotion period. Based on stakeholders' expertise, some promotions which were carried out in holidays, and special events had been excluded from the analysis.

**3. Data scope:** 300 promotions in 1 year of 60 toothpaste products throughout 1700 retail stores.
Dataset has relevant information describing the promotions (time, type, place of display, discount rate, discount value), their result (the rate of comparation of sales between before and after the period - score), items (types, sizes, brand, price segment), store (place, size of store, income level of surrounding residents).
- For categorical data, I encoded it by one-hot to be compatible with K-mean approach.

**4. Tools:** clean, process, apply k-mean by Python, visualize by Power BI 

**5. Duration:** 1 month.

### 2. Sample of the reports and some of the insights:

**Question 1: What features do successful promotions have in common?**
<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/data.2023-1.png?raw=true"/>

**Question 2: For a specific item/type of item/area, how should they run the promotion?**
<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/data.2023-22.png?raw=true"/>

**Question 3: How about the period of after promotions?**
<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/data.2023-3.png?raw=true"/>

