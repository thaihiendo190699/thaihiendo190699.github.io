## Building dashboard for daily monitoring of the operational performance of a FMCG retail chain

**Project description:** 

Context: The Operational Department needs to monitor daily data on the operation throughout its company system to ensure that over 1700 retail stores have adequate stocks to serve customers. In addition, they must take action as quickly as possible to solve any arisen problems, usually within a day or several days.

Problem: There are too many separate reports from the company system, completely in Excel sheet format, which causes difficulty and time-wasting for the employees in getting relevant data to control the complex operation. As a result, problem-solving actions are often delayed or not well-informed by data, and the workload of employees is often overloaded.

Solution: Building an automatic dashboard that has all relevant information to boost work efficiency for the whole team.


### 1. Data preparation:

#### 1.1 Data downloading automatically from company report systems by Python

As company policy about data security, data analysts do not have permissions to query data from the database directly, so I need to download Excel-formated data separately from the system built by IT department.

I used selenium library in Python to execute the tasks and Task Scheduler to automate them on a daily basis.

[Python code sample](https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/POS-downloader-HIE.ipynb?short_path=d160d63)

#### 1.2. Data processing by Python

- Converted data to feather form for easy processing.
- Processed data
+ Cleaned, transformed, mapped, aggregated data
+ Exported the dataset as a parquet file to import to Power BI.

[Python code sample](https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/code_BI.ipynb)

#### 2. Dashboard building by Power BI

I used Power BI to create a multiple-sheet dashboard and share it for the department by Power BI service.

The sample of my dashboard: 

1) Key metric - Lostsale (how many percentage of goods are lacking compared to demand)

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/BI1.png?raw=true"/>

2) Inventory change (how inventory is imported and exported at the stores)

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/BI2.png?raw=true"/>

4) Cause of lost sales detecting (detect causes that can create high lost sales index)

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/BI3.png?raw=true"/>

For example, from this report, it can be seen that a small group of stores belonging to a specific hub has a high lost sales rate (7.5%). The reason can be seen that in stage 4 in the Funnel chart, the quantity of goods is significantly reduced compared to the previous stage (almost half) and is smaller than the minimum demand (the first stage). Therefore, the person in charge will review the conditions in this step and take action as quickly as possible.


