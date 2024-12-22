# Data Analyst Portfolio

Welcome to my Data Analyst Portfolio!

I have included a variety of projects that highlight my data analytics skills. These projects feature links to dashboards and reports I’ve created using tools such as Power BI, Excel and SQL. They demonstrate my ability to analyse and present data in a clear, visually engaging manner that resonates with diverse stakeholders. Through these projects, I have gained valuable experience and enhanced my ability to present actionable insights effectively. I am eager to continue learning and growing in the data analytics field, continually refining my skills to uncover meaningful data-driven solutions.


Feel free to explore my work and get a glimpse into how I transform raw data into meaningful insights!


## Power Bi Projects

### Call Centre Analysis Project

#### Project Goal
Analyse and build reports around identifying key performance indicators (KPIs) such as average wait times, call resolution rates, agent performance and interval analysis to uncover deeper insights from the dataset.

#### Key Steps

#### 1. Data Exploration

#### Goals achieved in this step:

The main objective of the call centre analysis is to enhance operational efficiency, improve customer satisfaction, and optimise resource allocation. The analysis is broken down into three main components to address different aspects of performance:
* General KPIs: Metrics such as call volume, average handle time (AHT), first call resolution (FCR), and call forecasts
* Interval Analysis: Metrics tracked across specific time intervals, including call volume by hour, peak periods, and trends in wait times
* Agent Performance: To evaluate individual and team-level agent performance looking at NPS and CSAT scores for targeted improvements

#### 2. Data Preparation

#### Goal: Prepare the data for an effective data model for analysis.

Key steps taken:

In Power Query:
* Identify and delete duplicate entries and making sure each column in the dataset has its appropriate data type
* Created a dedicated calendar and intervals table for time intelligence analysis

In Power BI Desktop:
* Built calculated column to identify and classify the different call-handling metrics (Wait Time, Hold Time, and After-Call Work) by their duration in minutes
* Built a customer satisfaction indicator calculated column for satisfaction rate calculation
* Built a calculated table, obtaining the highest and lowest CSAT and NPS scores per agent using DAX functions like MAXX and FILTER
* Implemented a measure to dynamically display the last N months based on user slicer selection

#### 3. Data Modelling

* Designed the data model using a star schema, with a central fact table linked to dimension tables.
* Implemented snowflake schema where appropriate, normalizing dimension tables for better storage efficiency
* With the previous steps and preparations, the data model can be established for dashboard building.

4. Logical Considerations While Building the Dashboard

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/1.PNG)

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/2.PNG)

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/3.PNG)

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/4.PNG)
