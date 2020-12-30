# Analysis of data Kickstarting campaign 

## Overview of project
Louise has been trying to identify trends that will help her implement better practices to determine her targets in a more reliable way. This project presents diverse data related to different crowdfunding campaigns organized by her from 2014 to 2017.  Therefore, through this analysis, Louise will be able to find out any hidden trends. 

### Purpose
The purpose of this project is to visualize the campaign outcomes based on launch dates and funding goals. This part of the project will only base our analysis on two categories: Theater and Plays. 

## Analysis and Challenges
### Analysis of Outcomes based on Launched date
For the purpose of this analysis, we took into consideration the Parent Category "Theater." To make this evaluation, we considered the number of outcomes (Successful, Failed, Canceled) based on the launched date per month for the campaign (2014 – 2017). 
With the data shown in Chart 1 (see below), Louise will be able to identify the following:
- During May, June, and July, there is a tendency to have many successful events based on her launched dates. The data for these three months also shows that there is a slightly linear behavior of numbers of failed events, which means that the targets established for these three months were coherent.
- The number of successful vs. failed events follows a similar tendency between the months of January to April, and September to November. That means that Louise needs to revaluate her targets for both outcomes. Overall, in order to increase the number of successful events and reduce the number of failed events, she needs to reduce the target goals for the months aforementioned. 
- Another critical point to highlight is that the number of successful and failed events is significantly similar during December, which means that the successful events' goals should be re-assessed for future events during this month.
- Lately, the number of canceled events is insignificant given the population's size shown in the data set and represents a linear behavior along the year. One point to consider is that in October, no events were canceled.
---
Chart 1

![](https://github.com/Marietas/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.PNG)


### Analysis of Outcomes based on Goals
For the purpose of this analysis, we took into consideration the Parent Category "Theater" and subcategory "Plays." To make this evaluation, we considered the number of outcomes (Successful, Failed, Canceled) on a different dollar-amount range, which allowed us to organize the events on their specific goal amount for the campaign (2014 – 2017). 
With the data shown in Chart 2 (see below), Louise will be able to identify the following:
-	The percentage of successful events is higher than 50% between the ranges of $0 to $19,999 and between $35,000 to $44,999. Especially in this last range, the percentage of successful events is close to the 67% mark. 
-	On the dollar-range of $20,000 to $34,999, the number of failed events is significantly higher (up to 80%) compare to the successful ones.  
-	100% of the events failed in the dollar range of $45,000 to $49,999.
-	There is an 80% probability of failed, for events with goals greater than $50,000.
The results of the "Outcomes based on goals" show that any events from $0 to $4,999 and $35,000 to $44,999 are events with a strong probability of success. Events with goals between dollar-ranges of $25,000 to $34,999 and greater than $45,000 should be re-assed, as they have a really low  chance of being successful (less than 25%). 
---
Chart 2

![](https://github.com/Marietas/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.PNG)

### Challenges and Difficulties Encountered

-	During the Analysis of Outcomes based on Launched date, the main challenge was how to convert the month represented by number to a month represented by a text to display it in the right format in the pivot table. Example: how to convert 06 to June. To overcome this challenge, I used the function TEXT (value, "format_text"). To use this function, I added the column "U" and applied the following formula =TEXT(S2,"mmmm"). Please refer to Colum U on the master data tab.
-	During the Analysis of Outcomes based on Goals, the main challenge was that I missed adding the outcome filter to the nested formula. Therefore, the numbers were not accurate. To overcome this challenge, I performed an audit against the master data to confirm the accuracy of the results and then added the segment of the outcome filter to the nested formula. 

## Results
1. What are two conclusions you can draw about the Outcomes based on Launch Date?
Regarding the data of the Outcomes based on Launch Date analysis, the following conclusions can be drawn:
-	There are coherent target goals based on the Launch Date for May, June, and July. To support this conclusion, the data for these months show a slightly linear behavior of numbers of failed events. 
-	Louise needs to revaluate her targets for both outcomes (successful and failed events) from January to April and September to November. Overall, the results show that by reducing the target goals, she will increase the number of successful events and reduce the number of failed events.
-	The number of successful and failed events are significantly similar during December, and therefore, the goals for the successful events should be re-assessed for future events during this month.

2.	What can you conclude about the Outcomes based on Goals?
According to the analysis performed to the Outcomes based on Goals, the following conclusions are considered:
-	The results of the "Outcomes based on goals" show that any events from $0 to $4,999 and $35,000 to $44,999 are events with a strong probability of success. 
-	Events with goals between dollar-ranges of $25,000 to $34,999 and greater than $45,000 should be re-assed, as they have a really low chance of being successful (less than 25%). 

3.	What are some limitations of this dataset?
-	There is not enough information on the criteria used by Louis to establish the goals. The goals could be defined as a percentage of the budget per event, which in this case, the information is missing. 
-	There is no definition of the data in columns K/L/M (Staff_pick, backers_count, and spotlight) mean. This missing information could potentially add value to the analysis.  
-	Another data set that could add value to the analysis would be the target audience (family, kids, adults, etc.). For example, this information could conclude why the number of successful events increased during the summer months. 

4.	What are some other possible tables and/or graphs that we could create?
-	Outcomes (successful, failed, canceled) per month per year. This chart will provide an idea of the behavior of the outcomes through the years and reveal if it is consistent or not.
-	Outcomes based on goals and launched dates per country. This graph will help us understand which country is most likely to have a higher number of successful events. We could also add the month to this analysis to understand the audience's behavior in each country against the time zone difference. 
-	On the outcome based on goals analysis, the dollar-range of equal to $50,000 was not required to be shown in the analysis/chart. Louise could use these missing records to have a different perspective on the evaluation. 

