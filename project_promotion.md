## FMCG Promotion Analyst

**Project description:** 

Context: The Toothpaste Category Department tried to boost their sales through promotions. They ran a lot of promotions throughout the year, mainly based on their experience and some assumptions. 

Problem: They realized there aren't always good promotions and the one can be good or bad in different stores. They want to know more details about their promotion results and find the best practices to focus their resources on as well as confirm by data some of their assumptions.

**Question 1: What features do successful promotions have in common?**

**Question 2: For a specific item/type of item/area, how should they run the promotion?**

**Question 3: How promotion of an item/ a group of items affect sales of the whole category?**

### 1. Analytical approach

**1. Method of analysis:** descriptive analysis, using K-mean to cluster promotions based on their results. Each datapoint for clustering is a promotion for a specific product in a store.

**2. Benchmark (agreed by stakeholders):** a successfull promotion program need to achieve at least 120% sales compared to the normal sales within the last 30 days and no loss of profits.
- Drawback: some other factors affect sales during the promotion period. Based on stakeholders' expertise, some promotions which were carried out in holidays, and special events had been excluded from the analysis.

**3. Data scope:** all promotions in 1 year of all toothpaste products throughout 1700 retail stores.
Dataset has all relevant information describe the promotions (time, type, place of display, discount rate, discount value), their result (the rate of comparation of sales between before and after the period), items (types, sizes, brand, price segment), store (place, size of store, income level of surrounding residents).
- For categorical data, I encoded it by one-hot to be compatible with K-mean approach.

**4. Tools:** clean, process, apply k-mean by Python, visualize by Power BI 

**5. Duration:** 1 month.

### 2. Sample of the reports and some of the insights:

**Question 1: What features do successful promotions have in common?**
7 days period

**Question 2: For a specific item/type of item/area, how should they run the promotion?**
Brand X should be "discount about 30% - 35%"
Brand Y should be "buy 2 get 1 free", customers seem willing to stock Y products whenever they are on sale, different from brand X.

**Question 3: How promotion of an item/ a group of items affect sales of the whole category?**


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
