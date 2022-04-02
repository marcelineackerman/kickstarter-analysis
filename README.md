# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of this analysis was to help a potential Kickstarter user understand how to maximize their success when launching a campaign for their new theater play. Using data from a few thousand successful, failed, canceled, and currently live Kickstarter campaigns, I organized and visualized the major factors in whether or not a Kickstarter campaign is likely to be successful. This includes outcomes based on original goals, and theater-based outcomes based on launch date.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The following line chart demonstrates the outcomes of various theater-based Kickstarters based on the month they were launched.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/100869713/161392734-f7b07208-1b2a-47d4-b6dd-129e748e497a.png)

This chart can help a potential user's campaign decide the best time of year to launch their Kickstarter, to maximize potential of successful funding. This analysis was performed using the PivotTable function in Excel to first create a table.

![image](https://user-images.githubusercontent.com/100869713/161392892-54da2c63-ce23-4a56-baed-b1a1b9494cd4.png)

Then generating a chart based on this table. The table and chart are both filtered based on only theater Kickstarters, with the total outcomes of either "Successful", "Failed" or "Canceled" as the Y axis, and the Date (specifically, the month) as the X Axis.

### Analysis of Outcomes Based on Goals
The following line chart demonstrates the percentage of outcomes (successful, failed, or canceled) based on the original goal of the Kickstarter campaign.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/100869713/161392965-e46858ca-b1ae-46c6-8eed-ae71cbaa2f63.png)

This chart can help a potential user pick a starting goal for their campaign, in order to maximize chance of successfully reaching their funding goal. This analysis was performed using the COUNTIFS function in Excel to create a table of the number of successful, failed, and canceled projects in the "theater" category, then extrapolating those amounts into percentages.

### Challenges and Difficulties Encountered

During these analyses, I ran into some difficulty understand the measures of central tendency. The meanings of these statistics terms were familiar to me, but how to actual measure their values was new information and took some additional research to understand what exactly we were measuring with "standard deviation" and "IQR". During the challenge itself, I ran into some difficulty interpreting the chart based on the percentage of outcomes based on goals, as the chart provides no visualization for the actual amount of successful outcomes. This can lead to misinterpreting the data to mean a higher goal is near-equally successful as a lower goal, while the actual sum of successful outcomes is much higher for lower goals.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The first and most obvious conclusion I can draw from the Outcomes based on Launch Date chart is that beginning a theater Kickstarter campaign in the late spring to early summer has the highest rate of success. Specifically, May and June seem to be optimal months for starting theater funding campaigns, decreasing rapidly toward September and remaining low throughout winter and early spring.

The second conclusion I can draw is that the majority of campaigns are started in the late spring and throughout the summer, with the winter months beginning the fewest amount of campaigns. This is demonstrated by both the successful and failed lines having significant dips in March and November. This could mean that the higher probability of successful campaigns in Spring/Summer is correlated with a higher amount of campaigns started in that time frame.

- What can you conclude about the Outcomes based on Goals?

From the Outcomes based on Goals chart, I can conclude that smaller goals are more likely to lead to successfully funded campaigns in US-based play fundraising campaigns, and as the goal amount increases, the likelihood of success decreases. While there is a rise in the $35000 to $39999 and $40000 to $44999 range demonstrated on the chart, this does not account for the significantly fewer amount of campaigns total with those ranges as goals, and may potentially be outliers.

- What are some limitations of this dataset?

One limitation is this dataset does not account for existing budget that can be used to publicize/advertise an existing campaign. There is a potentially large impact on success based on the ability to produce publicity materials and advertise a live campaign in progress.

A second limitation is there is no way to determine success based on the theme of a given play. All plays are simply labeled as "play", whereas other categories include more granular subcategories. Having plays labeled by genre or theme can give a potential user more information on their own potential of success based on their own play's genre or theme.

- What are some other possible tables and/or graphs that we could create?

Using the existing dataset, you could create a chart that demonstrates success vs failure rate based on the length of a campaign from launch to deadline. Do longer campaigns have a higher rate of success, or short ones? First, add a column finding the date difference between launch and deadline, then make a table of the differences between launch and deadline in categories like "1 month" "2 months" using the COUNTIFS function, then compare that against success and failure rates and plot them on a line graph.

You could also create a table and graph demonstrating if a large number of smaller backers is more successful than a smaller number of larger backers. This could help determine what incentives to offer at each backer level to incentivize larger donations. First, find the average donation and make a range for number of plays like "<10" "10-50" "50-150", then plot it on a stacked column graph demonstrating the successful, failed, and canceled campaigns for each range.

A third potential chart is to plot on a line chart the number of successful and failed campaigns based on year of campaign launch. This could demonstrate the overall tendency of the public's willingness to back a new theater play based on recent years, and if it is trending up or down. This would allow a potential user decide if this year is a prime time to launch their campaign.
