# Kickstarter Campaign Analysis with Excel

## Overview of Project
Louise launched a kickstarter campaign to fund the production of a play she wrote.  Her kickstarter nearly reached its funding goal shortly after launching and based on the provided dataset, she wants to learn more about the effect time of year and the lenghth of time the kickstarter runs on whether the campaign reaches its fundraising goal.
### Purpose
The purpose of this project is to analyze the kickstarter campaign data to arm Louise with the best actionable analysis based on prior kickstarter campaign trends to enable her to carry out a successful kickstarter campaign.
## Analysis and Challenges
The analysis consists of two main elements: a pivot chart evaluating the campaign outcomes based on its launch date and a line chart analyzing the campaign outcomes based on the fundraising goals. 
### Analysis of Outcomes Based on Launch Date
For the Outcomes Based on Launch Date analysis, first a Years column had to be added to the data using the [YEAR()](https://support.microsoft.com/en-us/office/year-function-c64f017a-1354-490d-981f-578e8ec8d3b9) function.  Then a pivot table of the data displaying the outcomes of kickstarters based on what month they launched, with a parent category and year filter was created to show a count of how many kickstarters succeeded, failed, and were canceled sorted by year.  By selecting the theater filter, only theater kickstarters are displayed in the pivot table.  Then a pivot chart depicting the data was created, visually displaying the data.  

![pivot_chart](https://github.com/mewers2/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png) 
### Analysis of Outcomes Based on Goals
In a new sheet, using the [COUNTIFS()](https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842) function, the data is displayed in separate columns indicating the number of kickstarter plays which succeeded, failed, and were canceled and sorted by different dollar-amount ranges of the project goals.  The total amount of projects within each dollar-amount range is also displayed, along with the percentage of projects within each dollar-amount range that succeeded, failed, and were canceled.  Lastly, the data is displayed visually on a line chart illustrating two lines, one for percentage of the play kickstarter projects that succeeded and one line for the percentage that failed, with a point on the lines for each different dollar-amount range.

![line_chart](https://github.com/mewers2/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png) 
### Challenges and Difficulties Encountered
One challenge I encountered dealt with setting the exact columns of data for the line chart and getting them to display as desired.  The documentation [here](https://support.microsoft.com/en-us/topic/present-your-data-in-a-scatter-chart-or-a-line-chart-4570a80f-599a-4d6b-a155-104a9018b86e#:~:text=Click%20the%20Insert%20tab%2C%20and%20then%20click%20Insert%20Line%20or,style%20you%20want%20to%20use.) can provide assistance with creating a line chart.
## Results

- Looking at the Outcomes based on Launch Date chart, two conclusions can be drawn: first, the best time to launch a play kickstarter campaign is in either May or June.  May and June are the two months when the highest number of successful campaigns were started. The second conclusion that can be drawn from the Outcomes based on Launch Date chart is that December is the worst time of year to launch a play kickstarter campaign.  In December, the number of successful campaigns is at its lowest and the number of succesful campaigns is nearly equal to the number of failed campaigns.

- The Outcomes based on Goals chart quite strikingly indicates that the goal amounts with the best chances for success are either $5000 and below, or $35000 to $45000.  Keeping a production small (under $5000) shows approximately a 75% success rate with the lowest failure rate of 27% or less. If the production needs to be larger, launching a campaign with a goal amount of $35000 to $45000 is the next best solution with a 67% success rate and a failure rate that is below 40%.  

- A few limitations of this dataset are worth noting.  First, the age of this data.  The most recent lines within this dataset within the play subcategory are from 2017, five years ago and the earliest data in this set is from 2009, over ten years old.  There may be some new factors that might influence the performance of a kickstarter campaign in 2022.  Moreover, the dataset gives no account for the experience-level of the playwright, director, and production management.  This key factor could shed light on Louise's production and could guide her decisionmaking on critical roles where experience may be most helpful.

- Perhaps a chart could be created to display an evaluation of a campaign's length influences the outcome, or perhaps a chart displaying a campaign's length and the campaign's goal.
