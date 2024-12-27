# Data Analyst Portfolio

Welcome to my Data Analyst Portfolio!

I have included a variety of projects that highlight my data analytics skills. These projects feature links to dashboards and reports I’ve created using tools such as Power BI, Excel and SQL. They demonstrate my ability to analyse and present data in a clear, visually engaging manner that resonates with diverse stakeholders. Through these projects, I have gained valuable experience and enhanced my ability to present actionable insights effectively. I am eager to continue learning and growing in the data analytics field, continually refining my skills to uncover meaningful data-driven solutions.


Feel free to explore my work and get a glimpse into how I transform raw data into meaningful insights!


## Power Bi Projects

### Call Centre Analysis Project

#### Code: [Cell Centre Metrics Analysis.pbix](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/Cell%20Centre%20Metrics%20Analysis.pbix)



**Project Goal**
Analyse and build reports around identifying key performance indicators (KPIs) such as average wait times, call resolution rates, agent performance and interval analysis to uncover deeper insights from the dataset.

**Key Steps**

** 1.Data Exploration**

**Goals achieved in this step:**

The main objective of the call centre analysis is to enhance operational efficiency, improve customer satisfaction, and optimise resource allocation. The analysis is broken down into three main components to address different aspects of performance:
* General KPIs: Metrics such as call volume, average handle time (AHT), first call resolution (FCR), and call forecasts
* Interval Analysis: Metrics tracked across specific time intervals, including call volume by hour, peak periods, and trends in wait times
* Agent Performance: To evaluate individual and team-level agent performance looking at NPS and CSAT scores for targeted improvements

** 2. Data Preparation **

#### Goal: Prepare the data for an effective data model for analysis.

#### Key steps taken:

#### In Power Query:
* Identify and delete duplicate entries and making sure each column in the dataset has its appropriate data type
* Created a dedicated calendar and intervals table for time intelligence analysis

#### In Power BI Desktop:
* Built calculated column to identify and classify the different call-handling metrics (Wait Time, Hold Time, and After-Call Work) by their duration in minutes
* Built a customer satisfaction indicator calculated column for satisfaction rate calculation
* Built a calculated table, obtaining the highest and lowest CSAT and NPS scores per agent using DAX functions like MAXX and FILTER
* Implemented a measure to dynamically display the last N months based on user slicer selection

#### 3. Data Modelling

* Designed the data model using a star schema, with a central fact table linked to dimension tables.
* Implemented snowflake schema where appropriate, normalizing dimension tables for better storage efficiency
* With the previous steps and preparations, the data model can be established for dashboard building.

#### 4. Logical Considerations While Building the Dashboard

* Incorporated target/benchmark values that are based on industry standards, using them as reference points rather than actual dataset targets (i.e AHT target was set to 635)
* Average Handling Time (AHT) was calculated as the sum of hold time, after-work time, and talk time, some industries, only talk time or a different combination of times may be used to calculate AHT
* CSAT score calculation was adjusted to include both positive and neutral surveys, while acknowledging that in some industries, only positive surveys are counted towards the score

#### 5. Recommendations 

* Encourage a stronger focus on gathering detailed customer feedback post-interaction (through surveys or follow-ups) to identify specific pain points that may be impacting CSAT and NPS scores
* Based on my interval analysis, there should be an increase staffing during peak hours, particularly in the afternoon and evening, consider using flexible shifts or more part-time staff members
* Offer multiple survey methods (e.g., SMS, email, IVR) to increase participation, also implement follow-up reminders to customers who have not responded to the initial survey request
* Dive deeper into the specific reasons for high AHT later in the day. Communicate with staffing as to why, are calls becoming more complex, or is it related to agent fatigue or training gaps, offering additional training or implementing strategies to manage more complex calls could help reduce AHT


![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/Dashboards/1.PNG)

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/Dashboards/2.PNG)

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/Dashboards/3.PNG)

## Excel Projects

### Melbourne House Prices Analysis 

#### Code: [MelbourneHousePricesAnalysis.xlsm](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/Melbourne%20House%20Prices%20Analysis.xlsm)

#### Project Goal
Analyse and build a report to identify key seasonal trends in Melbourne house prices, focusing on top-performing suburbs and different market dynamics in different metropolitan regions

#### Key Steps

#### 1. Data Exploration

#### Goals achieved in this step:
The main objective of this analysis is to uncover seasonal fluctuations, identify high-performing suburbs, and explore the dynamics of different regions within Melbourne’s housing market.

* Seasonal Price Trends: Investigating price fluctuations throughout the year to uncover seasonal patterns and their impact on house prices.
* Suburb Performance: Analysing which suburbs have experienced the highest price growth, focusing on emerging and established areas.
* Regional Differences: Exploring price disparities between various metropolitan regions, understanding how location influences pricing trends.

#### 2. Data Preparation

#### Key steps taken:

* Cleaned the dataset by identifying and removing duplicates, filling missing values, and ensuring the accuracy of price data.
* Created a dynamic chart with slicers to visualise seasonal trends and allow filtering by suburb, price range, or time period.
* Created pivot tables to aggregate and analyse data by key dimensions, such as suburb, property type, and time period
* Implemented a simple macro that allows users to switch between different parts of the dashboard such as refreshing and returning to the home menu

#### 3. Interpretation & Insights

* House prices tend to peak during the spring/summer months and drop during the winter months. This seasonal fluctuation is likely driven by market activity, with more buyers entering the market in warmer months. As seen in the visual, there is a noticeable dip in property prices during the colder months (especially in April and July), suggesting a reduction in buyer activity and less competition for properties
* The average unit price has remained relatively stable throughout the year, whereas house prices fluctuate more significantly during specific months
* Prices in the inner-city suburbs are consistently higher compared to the outer suburbs, likely due to their proximity to business hubs and amenities
* Some outer suburbs, however, show a higher growth rate in recent years, likely driven by increasing demand from first-time homebuyers and investors looking for more affordable properties
* Areas like Bayside and Boroondara have higher average house prices, while more affordable regions such as Hume are showing promising growth trends in recent years



![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/Dashboards/4.PNG)


## SQL Projects

###  Running Carnival Database Design

#### Code: [RunningCarnivalDatabaseDesign.zip](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/Running%20Carnival%20Database%20Design.zip)

#### Goal:
Design and implement a relational database to manage event data, race results, and participant information for a fictitious carnival, ensuring data consistency and efficient querying.

#### Description:
This project involved creating a relational database for a carnival event using Oracle SQL. The database was designed to handle tables for event details, race results, and participant information. It included setting up constraints to maintain data integrity, as well as writing advanced SQL queries involving joins, subqueries, and aggregation functions to manipulate the data. Transaction handling was also implemented to ensure the database maintained consistency during updates.

#### Skills:

* Database design and implementation
* Oracle SQL (creating and altering tables, defining constraints)
* Advanced SQL querying (joins, subqueries, aggregation functions)
* Transaction management and data consistency

#### Results:
Successfully created a fully functional relational database for carnival data management. The use of advanced SQL queries enabled efficient data retrieval and manipulation, ensuring that event and race data was consistently updated and accurate. The project demonstrated an effective approach to database design and management while maintaining the integrity of the data.







