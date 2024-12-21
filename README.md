# Data-Analyst-Portfolio

Hi there and welcome to my data analyst portfolio!

I have included a variety of projects that highlight my data analytics skills. These projects feature links to dashboards and reports I’ve created using tools like Power BI, Excel and SQL. They demonstrate my ability to analyse and present data in a clear, visually engaging manner that resonates with diverse stakeholders. Through these projects, I have gained valuable experience and enhanced my ability to present actionable insights effectively. I am eager to continue learning and growing in this field, continually refining my skills to uncover meaningful data-driven solutions.


Feel free to explore my work and get a glimpse into how I transform raw data into meaningful insights!


# Portfolio Projects

## Call Centre Analysis Project

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/1.PNG)

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/2.PNG)

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/3.PNG)

#### About this project
##### Project Goal
Analyse and build reports around identifying key performance indicators (KPIs) such as average wait times, call resolution rates, agent performance and interval analysis to uncover deeper insights from the dataset.

Key Steps
1. Data Exploration

Goals achieved in this step:

Broke down the analysis into non-admission encounters, Admission and Readmission encounters, and Procedures.
Identified key metrics and attributes for each analysis section:
Attributes from patient information, including key demographics such as Gender, Age, Age Group, Race, and Marital Status.
Attributes from encounters and procedures, including encounter class, encounter description, procedure description, and procedure reasons.
General metrics for encounters and procedures, including counts, costs, rates, Length of Stay (LOS), and averages.
Special metrics for analyzing readmissions and mortalities, including the admission range, dates between the current visit and previous discharge, and dates between death and each admission.
2. Data Preparation

Goal: Prepare the data for an effective data model for analysis.

Key steps taken:

In Power Query:
Built dimension tables, including encounter class, age, age group, and date.
Merged encounter and patient tables to get the age at encounter and the date differences between death and each encounter.
Extracted the hour of each encounter visit.
Grouped procedure table to get procedure line cost totals for each encounter, then merged this into the encounter table.
In Power BI Desktop:
Built a calculated table from the encounters table for admissions and readmissions, obtaining the previous discharge date for each admission record using the Offset function in DAX.
Calculated LOS by minutes for non-admission encounters, and by days for admission encounters. Then built LOS bins for different minute ranges.
Built an admission type calculated column to identify initial admissions and readmissions.
Built a mortality indicator calculated column for mortality rate calculation.
Built all parameter tables for dynamic analysis.
3. Data Model

With the previous steps and preparations, the data model can be established for dashboard building.

Special consideration was given to the procedures table. Although there are possible links to dimension tables, the only relationship set is to the encounter table to ensure the correct linkage between encounters and procedures.

4. Logical Considerations While Building the Dashboard

Two major considerations were made when building the logic into the analysis:

Year range selection:
The dashboard is using fiscal year as the years range instead of calendar year.

Admissions:
By definition, only the Inpatient class includes overnight visits, which should be identified as admissions. However, data showed that visits under different encounter classes also had overnight stays, with some showing hundreds of days of stay. Thus, admissions and non-admissions were built by looking at the days stayed in the hospital rather than only the encounter classes.

Initial Admissions and Readmissions:
For readmission rate calculation, initial admissions and readmissions need to be identified. Initially, only these two types were considered based on visit dates. However, many visits were regular daily visits over consecutive days and should not be counted as initial admissions or readmissions. After careful review, these were categorized as a single admission for readmission rate calculation, while still counted as individual visits in the general admission settings.

![Alt Text](https://github.com/wilsonquach99/Data-Analyst-Portfolio/blob/main/4.PNG)
