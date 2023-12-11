## Building dashboard for daily monitoring of the operational performance of a FMCG retail chain

**Project description:** 

Context: The Operational Department needs to monitor daily data on the operation throughout its company system to ensure that over 1700 retail stores have adequate stocks to serve customers. In addition, they must take action as quickly as possible to solve any arisen problems, usually within a day or several days.

Problem: There are too many separate reports from the company system, completely in Excel sheet format, which causes difficulty and time-wasting for the employees in getting relevant data to control the complex operation. As a result, problem-solving actions are often delayed or not well-informed by data, and the workload of employees is often overloaded.

Solution: Building an automatic dashboard that has all relevant information to boost work efficiency for the whole team.


### 1. Requirements

Project Requirements and Strategy Document.


### 2. Bulding automatic data flow from scratch:

#### 2.1 Auto download data form company report systems

As company policy about data security, data analysts do not have permissions to query data from the database directly, so I need to download Excel-formated data separately from the system built by IT department.

I used selenium library in Python to execute the tasks and Task Scheduler to automate them on a daily basis.

Python code sample:

#### 2.2. Processing data in Python

- Chuyển đổi data sang dạng feather để dễ dàng xử lý về sau
- Xử lý dữ liệu
+ clean, transform and map data, aggregate.
+ export data set as parquet file

Python code sample

#### 2.3. Building dashboard in Power BI



For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
