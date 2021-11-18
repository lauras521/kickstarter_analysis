# Kickstarting with Excel
## Overview of Project
### Purpose
Louise's play, *Fever* came close to its fundraising goal quickly.  She now wants to understand how different Kickstarter campaigns faired in relation to their launch dates and their funding goals.  Reviewing data for different theater Kickstarter outcomes based on launch date and Kickstarter outcomes based on goal will help Louise see her Kickstarter fate.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
Below outlines the process taken to complete the analysis of outcomes based on launch date. 

A pivot table from all data on the Kickstarter tab was created.  The fields used can be seen in the image below:

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/ddbe1460dbe198404d2e1ab3d7159d8744adfd9c/Resources/Theater_Outcomes_by_Launch_Date_pivottable_fields.PNG>
</p>
    
Theater was filtered to only see outcomes in the same Parent Category as Louise's Kickstarter.  And columns were also filtered.  The theater filter and column filter location are highlighted in the image below:

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/main/Resources/Theater_Outcomes_by_Launch_Date_pivottable_filters_highlighted.PNG>
</p>

The columns were highlighted to only show completed Kickstarter campaigns and were ordered to show them in descending order.  The locations for column filters are highlighted in the image below:

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/main/Resources/Theater_Outcomes_by_Launch_Date_pivottable_columnfilters_highlighted.PNG>
</p>

A Pivot Line Chart with Makers was added and a title was added to the chart before saving.  An image for how to create this chart is shown below:

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/main/Resources/Theater_Outcomes_by_Launch_Date_how_to_insert_pivot_chart.PNG>
</p>

The final chart outcome is below:

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png>
</p>

#### Challenges and Difficulties Encountered
The one challenge I encountered was initially I sorted "Row Labels" in Descending order which reordered the months instead of sorting Column Labels.  This change carried over to the PivotChart which made it not intuitive to read.  This was corrected by sorting the Column labels.  This display makes more sense as people are familiar reading dates in order from January - December (vs. alphabetical order).

### Analysis of Outcomes Based on Goals
Text was added to get the correct columns and goals.  Columns were extended to be able to see all text.  Then COUNTIFS was used to calculate successful, unsuccessful, and cancelled "play" Kickstarters in predetermined dollar ranges.  The following formulas were used:

* =COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<5000")
* =SUM(B2:D2)
* =B2/E2  (used Percentage Number Format)

Chart for Outcomes Based on Goals Formula View:

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/main/Resources/Outcomes_Based_On_Goals_FormulaView.PNG>
</p>

The percentage columns were highlighted and a line graph was created and titled outcomes based on goal.

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/main/Resources/Outcomes_vs_Goals_GeneratingLineChart.PNG>
</p>

The final chart outcome is below:

<p align="center">
  <img src = https://github.com/lauras521/kickstarter_analysis/blob/main/Resources/Outcomes_vs_Goals.png>
</p>

#### Challenges and Difficulties Encountered
One challenge I encountered was initially I tried to capture the <= and > in one criteria with an AND statement  nested in the COUNTIFS statement vs. using it as 2 criteria.  An error was generated and it became clear they should be separated into 2 criteria and the AND piece was implied in the formula.  The other challenge was I highlighted all data to create the chart and had to delete 4 Legend Entries (Series) for "Number Successful," "Number Failed," "Number Canceled," and "Total Projects."  I could have just highlighted the 4 columns needed for the graph to avoid this step.

## Results
### What are two conclusions you can draw about the Outcomes based on Launch Date?
### What can you conclude about the Outcomes based on Goals?
### What are some limitations of this dataset?
### What are some other possible tables and/or graphs that we could create?








# An Analysis of Kickstarter Campaigns
## Louise wants to fund a play Fever via kickstarter.  The play has a $10,000+ budget.  Analysis of previous kickstarter campaigns was completed to determine factors in a successful kickstarter.
![KickstarterProjectOutcomesBasedonLaunchDate](path/to/image_name.png)
![USKickstarterProjectResultsbyParentCategoryChartPicture](path/to/image_name.png)
[data-1-1-3-StarterBook](path/to/filename.xlxs)
## Recommendations and Conclusions:
* Launch kickcstarter in May for highest success rate
* 60% of theater kickstarers are successful globally
* 72% of theater kickstarters are successful in GB
* 56% of theaeter kickstarters are successful in the US
* 91% of all kickstarters for theater are in GB or the US
* launch kickstarter in GB or US
* The theater parent category has the 2nd highest kickstarter success rate globally.  2nd to music.
* Within the theater parent category plays has the most kickstarters (vs. musicals and spaces) and plays has a 65% success rate.
* Of the play subcategory kickstarters in the US the mean goal of successful kickstarters was ~$5,000 vs. the mean goal of unsucessful kickstarters was ~$10,000.



