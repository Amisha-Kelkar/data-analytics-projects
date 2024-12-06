## Executive Summary
**Introduction**<br>
This report performs various analyses using the *nhtsa_traffic_fatalities* dataset to provide recommendations to various U.S. government stakeholders that could help prevent and improve the response to fatal traffic accidents.
The dataset was sourced from the National Highway Traffic Safety Administration (NHTSA). From this dataset, we were able to provide detailed analyses on fatal crashes from 2017-2020 regarding:
* Demographic factors
* Date and time
* Relation between crashes and driving conditions
* Crash Involvement characteristics (Vehicle and collision type)
* Weather conditions
* People involved in crashes
While the analyses only utilize four years of data, the resulting insights provide a reliable foundation for implementing crash-prevention and response measures. This reliability will only be improved by continuously adding newly available data.


**Methodology & Process**<br>
All project data work and analyses were conducted using SQL within a Jupyter notebook. Visualizations were created using Tableau.
1. Cleaning
	* The largest challenge with this dataset was choosing the most relevant of the 143 total tables spread across six different years. Multiple hours were spent on establishing the target outcome and the desired approach that allowed the team to key in on the final list of 21 tables used in this report
	* The dataset’s cleanliness and workability was assured through the following steps:
		1. Counting records across all tables used for each year as a sanity check to ensure their completeness and that their lengths were feasible in comparison to the other years
		2. From there, all tables (Including the created “population” table) were checked for “null” values, and none were found in any table
2. Merging Tables
To perform desired analyses, the merging of different table types was necessary to execute integral queries. The tables merged were as follows:
  * accident, vevent & drimpair tables for the years 2017-2020
  * accident 2017-2020 & population of states for years 2017-2020
3. Analysis & Observations
	* The project’s analysis process for the six categories listed in the introduction took place in a two-tiered process:
		1. Exploration: The team started their analysis by building on the narratives found in the project's first iteration. This included experimenting with scaled versions of queries from the first iteration (i.e., bringing in the years 2017-2019 and adding additional columns) and looking at interesting trends that manifested in the first iteration
		2. Insight Targeting: After finishing the exploration process, the team digested the query outputs and decided which areas would be most relevant to target stakeholders. From there, these chosen query outputs were optimized for stakeholder presentation (Converted to a palatable format for visualization) and synthesized in writing to explain their relevance
4. Visualization & Report Preparation
	* Selected query data was imported into Tableau to better to convey the project’s key insights and use cases. In Tableau, two dashboards were created:
		1. High-level findings for broad applications
		2. Tailored findings centering on specific conditions and circumstances

**Key Findings**<br>
*  Demographic factors
	1. The high population States of California, Florida, Texas, New York, and Georgia report the most accidents of any states. California is at the top with 4,881 fatal accidents from 2017-2020
	2. The states of North Dakota, Vermont, and Wyoming have the fewest accidents at often less than 50 per year. This is relfective of their lower populations and traffic density
	3. The rural states of Wyoming and Montana face elevated fatal accident rates relative to their populations (Despite having low absolute accident counts) due to factors such as limited emergency services, harsh weather, and extensive rural road networks
	4. The urbanized states of New York and Massachusetts have low fatal accident rates relative to their populations due to having safer roads through extensive public transportation, better infrastructure, and effective urban design.
* Date and time
	1. An interactive tool was created in Tableau that allows stakeholders to understand when fatal crashes most frequently happen historically by year (2017- 2020 individually and combined), day, hour, and 10-minute block within that hour. For example, “On Sundays from 2017-2020, crashes between 12:00 am and 1:00 am occurred most frequently between 12:00 am and 12:10 am”
	2. Higher crash counts in 2020 compared to 2017-2019 (+5.06%) suggest that abnormal situations related to a greater number of drivers on the road lead to more crashes
	3. Fatal crashes follow a highly predictable pattern across years, where they are at their peak in the warmer months (June-October) and decrease from there to their lowest numbers in the middle of winter (January & February) before increasing again
* Relation Between Crashes and Driving Conditions
	1. Roadway departures, vehicle rollovers, and motor vehicle collisions are consistently the top causes of crashes from 2017-2020. These trends are often amplified by driver impairment due to alcohol or drugs
	2. Weekends account for the majority of drunk driving deaths, where Saturday has the most, followed by Sunday and Friday. This trend aligns with peak social drinking nights, and overall death numbers are in line with increased drunk driving accidents
*  Crash involvement characteristics (Vehicle and collision type)
	1. Parked or stopped vehicles contribute significantly to fatal crashes, and this number has increased over time. This challenges the assumption that most crashes occur between moving vehicles
* Weather conditions
	1.  Cloudy and rainy weather conditions contribute the most to crashes in both urban and rural settings
	2. Less frequent conditions such as fog and smog contribute to crashes at a higher rate in urban settings
	3. Accidents occur more frequently in the daylight hours due to a higher traffic volume, while many nighttime crashes occur in poorly lit rural areas
* People involved in crashes
	1. Most traffic fatalities occur within the 45-60 age group
	2. The under-18 age group experiences the smallest number of traffic fatalities
	3. Males account for the majority of fatalities across all age groups


**Recommendations**<br>
* Assign more funding to traffic safety and road infrastructure in states with high accident rates relative to population
* Emergency services should utilize the “Top Crash Times by Day & Hour (2017-2020)” tool to optimize staffing and road placement to prevent and better repsond to car crashes
* Increase staffing and road placement of emergency services when factors that increase traffic volume are present
* Implement strategies to counteract the seasonal increase in fatal crashes during the warmer months, including increased emergency services staffing, higher fines for poor driving, and enhanced driver’s education programs
* Increase awareness of driving under the influence and increase the severity of punishments for such offenses
* Promote road safety awareness, and improve road design with construction projects
* Promote and implement vehicle stability technologies
* Enforce stricter parking regulations and raise awareness surrounding the dangers presented by parked vehicles
* Heighten alertness and emergency services availability during adverse weather conditions such as rain, snow, fog, and smog
* Improve infrastructure to reduce the negative impacts of poor lighting conditions in traffic accidents


**Conclusion**<br>
Overall, in conducting extensive analyses on the 2017-2020 fatal traffic data, the team was able to identify trends in the various conditions, factors, and characteristics of fatal traffic accidents. From this, the team was able to supply a list of key findings and associated recommendations that can help to prevent and improve the response to traffic accidents. While these findings will benefit from additional data in the future, this project has served to provide government stakeholders with foundational insights that can allow them to improve traffic safety, and decrease traffic fatalities.
