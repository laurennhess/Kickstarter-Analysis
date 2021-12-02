# Kickstarting with Excel
## Module 1: Analysis on Kickstarter Data 

### Overview of Project
We are able to use the Kickstarter data to understand the successes and failures of Kickstarter Campaigns. Using the Kickstarter Analysis data, we were able to visualize a campaign outcomes based on their relationship to their launch date and funding goal.

#### Purpose
The purpose of this assignment was to see how different campaigns fared in relation to their launch dates and funding goals. We specifically looked at theater campaigns. By visualizing the outcomes of theater campaigns, we can determine which month generated the most successful campaigns. This will help future campaigners chose their launch date. Additionally, we can determine what an optimal campaign goal is depending on how many successful, failed, or canceled campaigns there were based on their funding goals. 

### Analysis and Challenges
In this analysis, I generated a pivot table with specific fields and filters, then created a line chart based off my pivot table. In the second analysis, I used the =COUNTIFS() function to fill in the ranges, then built a line chart off of that table. 

#### Analysis of Outcomes Based on Launch Date
To visualize the Outcomes of Campaigns Based on Launch Date, I created a Pivot Table that was filtered on the Parent Category, 'Theater,' as well as 'Years.' Next, I set my columns to be the outcomes - successful, failed, canceled - and changed the Row Labels to the months of the year. This is the pivot table that was generated:
<img width="492" alt="Screen Shot 2021-12-01 at 9 58 36 PM" src="https://user-images.githubusercontent.com/94096530/144366215-43955cc5-0c8c-4d58-bfd4-599e3b05bdfd.png">


Next, I created a line chart to visualize the Outcomes based on Launch Date. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/94096530/144366224-3d1558e9-e9e9-46b9-94be-f1959a347d63.png)

From this graph, we can see that the month that generated the most successful campaigns was March. The month that generated the least successful campaigns was December.

#### Analysis of Outcomes Based on Goals
In this analysis I created a new sheet with a column of different ranges for the 'Campaign Goal.' Then, I used the =COUNTIFS() function to extract data from the Kickstarter worksheet where campaigns were in the specified numeric range, were under the subcategory 'Play', and were either successful, failed, or canceled. Next, I summed the values and found the percentage. 
<img width="1369" alt="Screen Shot 2021-12-01 at 9 59 03 PM" src="https://user-images.githubusercontent.com/94096530/144366264-f8413006-79a2-4c97-a307-f53714d18b16.png">

From this table, I was able to create another line graph to show the outcome based on campaign goals. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/94096530/144366277-2134ba33-eed8-40d3-8b89-a8271d93402d.png)


### Challenges and Difficulties Encountered
One of the challenges I encountered was filtering the Row Lables in the Pivot table to be just the month. I had to delete a few labels in the rows field which autopopulated when I dragged the 'years' to it. After the rows were set as the month, the data was much easier to read. 

### Results
In conclusion, for Outcomes Based on Launch Date, we can see that the best month to launch a theater funding campaign is in May. However, there are also a high number of successful campaigns in June and July. We can also see that launching a campaign in December would yeild the lowest success rate. 

For Outcome Based on Goals, we can see that goals $1,000 or less were 75% successful, followed by goals $1,000 - $4,999 were 73% successful. Therefore, staying in the range of $0 - $4,999 range would yield the best results. However, if you wanted to take some risk, goals in the $35,000 - $44,999 yielded a 67% success rate, which is still significantly high. I would recommend not setting a goal that exceeds $44,999 because that is where the failure rate increases rapidly.

One limitation of this data set is that we are not able to see the success of the campaign over time, since we are only limited to the amount they generated on a monthly basis. If we could see the success of the campaign over multiple months, that may have changed our results from above. 

To address the limitation noted above, we could create another column for duration of campaign and see how that would affect our line graph. If we looked at campaigns over multiple months, I would have considered using an area chart to display the long term data. 
