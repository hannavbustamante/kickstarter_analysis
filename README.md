# Analysis of Kickstarter Campaigns
*MS Excel data analysis using advanced Excel formulas to uncover trends*

## Project Overview 
### Background
In this project I am performing data analysis for the ***Kickstarter*** crowdfunding campaigns (from the year 2009 to 2017) in order to find trends, patterns or correlations in Kickstarter dataset, and answer the following questions:
- [x] Is there a correlation between time (month of the year) and campaign outcome?
- [x] How successful are campaigns within a certain goal range?
- [ ] 
For this data analysis I am using ***MS Excel*** as a tool, including **interactive pivot tables and charts**, **conditional formatting**, **advanced filters**, **VLOOKUPs**, **COUNTIFs** and various **advanced Excel formulas**.

:heavy_check_mark: All calculations refer to spreadsheets ![Kickstarter_Challange.xlsx](Kickstarter_Challange.xlsx) and ![StarterBook.xlsx](StarterBook.xlsx) 
<kbd>
(Please download the .xlsx files to see the full analysis.)
</kbd>

### Purpose
The purpose of this analysis is to help playwright Louise with her decisions in applying for the crowdfunding campaign on Kickstarter. Her campaign is a theater play *Fever* at an estimated cost of roughly *$10,000*. She is wondering where she stands with her goal, how successful are campaigns with a similar budget and when is a good time to launch the campaign. She is interested in the US and GB theater market, specifically in plays and musicals respectively; therefore, part of this analysis focuses on those fields as well.

```In this report``` :bulb: ```symbol is used to guide Louise’s decision based on this data analysis.```

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
In this analysis, I created an interactive pivot table and a line pivot chart that can be filtered by parent category and years. The chart **Theater Outcomes Based on Launch Date** has months on x-axis and count of outcomes on y-axis. I created pivot table and chart from the selection of the entire dataset. Next, I added selected variables by dragging and dropping into chart fields and set up filters on the data that I wanted to drill-down (years and parent category).

From the chart, we can see that May and June are the best months to start the campaign. There were 111 (67%\*) and 100 (65%\*) successful campaigns, respectively. The number of successful campaigns significantly declined in December; only 37 (49%\*) successful campaigns in this month. Moreover, May and June have a higher volume of campaigns, 166 (12%\*) and 153 (11%\*) respectively, while December has the lowest volume of campaigns at 75 (5%\*). Another interesting observation is the overall success rate of theater campaigns at 61%\**.

\* Percentages are calculated from the total campaigns within the same month.

\** Percentage of theater campaigns is calculated from the total campaigns in all categories.

<p align="center">
<img src="Resources/Theater_Outcomes_vs_Launch.png" width="50%" height="50%">
</p>


:bulb: ```This data analysis can help playwright Louise decide when is a good time to start a campaign. She can plan accordingly in order to increase her chances of success.```


### Analysis of Outcomes Based on Goals
In this analysis, I created a table to count theater plays campaigns based on their outcome and goal range. For calculations, I used `COUNTIFS()` formula, which consists of three conditions `subcategory`, `range`, and `outcome`. Next, I used `SUM()` formula to calculate total projects for each goal range. Additionally, I calculated the corresponding percentages for outcomes and used cell formatting to convert numbers into % and round them to the nearest integer. 

<p align="center">
<img src="Resources/Outcomes_vs_Goals.png" width="70%" height="50%">
</p>

The table and chart **Outcomes Based on Goals** reveals which goal range has a higher % of successful campaigns. Campaigns with a goal of less than $1,000 and a goal range between $1,000 to $4,999 have a higher success rate 76% and 73% respectively, while campaigns with the goal above $50,000 have a lower success rate at 13%.


:bulb: ```Louise’s project falls in goal range between $10,000 and $15,000. The success rate in this range is 54%. However, the volume of total campaigns in this range is not very high. Only 72 (7%) campaigns are in this range. For comparison, one range below her budget ($5,000 to $9,999) has a similar success rate at 55%, and the volume at 169 (16%) total campaigns.```

### Challenges and Difficulties Encountered
I found the written part of the analysis the most challenging. I realized that takes a lot of time and effort to tell a meaningful story and to write a clear, easy-to-understand analysis report. Yet it is very rewarding at the end. I encountered some technical problems as well, but luckily the “coding” community is very active and very helpful. Searching for technical support on **@StackOverflow**, **@BSC Lessons**, and **@Slack** made this part much easier and I was able to overcome those challenges. 

#### Written Report and Understanding Data
Writing this report was my biggest challenge. I believe communication is very important and the work I did would have very little value if I couldn’t share it with others throughout this report. I really wanted to have a good start so I devoted extra time, re-read lessons and pre-work, and looked for information in external articles. Another important part is understanding the data I was working with. 

#### Markdown Language
I wrote a report in Word document, transferred to README.md file, and hoped it will work. Soon, I learned that this is not a case. At first, I struggled with markdown language, in order to get things right and visually pleasing. After a few trials and errors, I started noticing progress. I was surprised at how much I could do with it. One thing led to another. At first, I learned how to include a picture in the text, then I wanted this picture to be in the center and then I wanted to be the right size and so on (and of course :smiley: - emojis!). With every new correction, I learned something new and that was an exciting part! I also learned that markdown language is somewhat similar to HTML that I would like to learn as well! This motivation and rewarding results had helped me overcome this challenge.

#### Sorting Pivot Chart and Table by Descending or Ascending Order
I was familiar with sorting rows in the spreadsheet but was unfamiliar with this feature in pivot tables and charts. At first, I thought that was not possible for pivot tables and charts. Thanks to the lecture I learned that I can sort pivot tables and charts and was surprised how organized and clean the visualization looked by applying this feature.

#### Conditional Formatting
I had some basic knowledge of conditional formatting, yet I learned I was doing it "long-way". If I wanted to make corrections I would go back to setting and rewrite the rules. Spending some time on conditional formatting I noticed a very convenient button `manage rules`. It can be found in Home Tab -> Conditional Formatting drop-down menu -> Manage Rules. It was a bit of a game-changer for me. Now I am able to manage conditional formatting rules more efficiently.

## Results
### Conclusions about the Theater Outcomes based on Launch Date
- [x] May and June have 111 (67%) and 100 (65%) successful campaigns respectively.
- [x] December has 37 (49%) successful campaigns.
- [x] May and June have a total of 166 (12%) and 153 (11%) campaigns, respectively.
- [x] December has a total of 75 (5%) campaigns.
- [x] Overall success rate of theater campaigns is 61%.

:heavy_check_mark: Campaigns launched in May and June has a higher success rate than campaigns launched in December.

:heavy_check_mark: More campaigns are launched in May and June than in December.

### Conclusions about the Outcomes based on Goals for Theater Plays
- [x] Campaigns with a set goal under $1,000 have a 76% success rate.
- [x] Campaigns with a set goal between $1,000 to $4999 have a 73% success rate.
- [x] Campaigns with a set goal of over $50,000 have a 13% success rate.
- [x] 96% of all campaigns are under a set goal of $25,000.
- [x] 4% of all campaigns are above a set goal of $25,000.

:heavy_check_mark: Campaigns with a set goal under $1,000 has higher success rate than campaigns with a set goal over $50,000.

:heavy_check_mark: There are significant more campaigns with a set goal under $25,000 than campaigns above $25,000.

### Limitations of the dataset
:exclamation: Excel is a great tool since doesn’t require a specific query language to retrieve data, it is widely used and easy to learn. Excel is also very versatile since covers many fields of the data pipeline: exploratory data analysis, data validation, data visualization, and data analysis. These are great aspects but have some drawbacks as well. 

:exclamation:Excel files are easy to duplicate, and it is done more than has to be, what can lead to inaccuracy and referring to outdated data. Duplicates and multiple versions of datasets are one of the biggest issues of data accuracy.

:exclamation:Multiple access problem. Excel files are inconvenient when multiple people need to work on the same excel file at the same time.

:exclamation:Not suitable for a large amount of data. Excel has limitation of 1,048,576 rows and 16,384 XFD columns.
 
If the chart is missing or lacking a descriptive title, especially when we save Pivot charts in separate directories apart from corresponding pivot tables, visualization can be misleading. 
 
### Recommendations for additional tables and graphs

:pushpin: Using data bars. 
          
Using data bars on tables gives us at-a-glance analysis and we can easily see what data stands out.

:pushpin: Pivot tables and charts with additional filters.
Adding an additional filter to a table, for example, *Theater outcome based on launch date* (see the table at the beginning of this report) would enable easy comparison of selected categories by country.

:pushpin: Additional analysis in order to find more patterns and trends, for example:
- Correlation between the length of campaigns (launched date vs. deadline to outcome) and their outcome.
- Correlation between backers count, average donation and campaign outcome.

:pushpin: Pie charts and dot charts. We could use those charts for data that contain less information (2-3 different proportions of a whole). An example for pie chart would be *theater plays outcome chart*. 
