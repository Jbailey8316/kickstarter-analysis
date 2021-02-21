# kickstarter-analysis
## ***Purpose:*** Performing analysis on kickstarter data to uncover trends for theatrical plays 
---
**Analysis and Challenges:**
---
By using MS Excel to interept the kickstater data I was able to organize and extract key information on the trends of multiple kickstarters within the scope of Theaterical Plays.
Once compiled I was able to determine the most likely scenarios of a successful campaign including details like the importance of launch date and goal setting.  Once collected; this information was used to create graphs to visually track and easily interpret the trends.  This was done using excels graphing features.  The below graph details the importance of a good launch date.  
---
**Outcomes Based on Launch Date**
![Outcomes Based on Launch Date](https://github.com/Jbailey8316/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)
---
From our collected data we can assess that a launch date in May would be most likely to succeed based on the trends set by past kickstarters.
---
Furthermore, the goal set for the kickstarter seems to play a role in its success as well.  Having a good estimate of where to set the goal is crucial in attaining succesful funding for the project.  From the graph below we can estimate that projects ranging from $1000 to roughly $5000 tend to get successfully funded.
---
**Outcomes Based on Goals**
---
![Outcomes Based on Goals](https://github.com/Jbailey8316/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)
---
---
One of the challenges I came across was organizing the data based on the goal ranges.  I had some difficulty in getting the goal ranges to work within my excel formula.  For example: "=COUNTIFS(Kickstarter!$F$77:$F$4115,"successful",Kickstarter!$R$77:$R$4115,"plays",Kickstarter!$D$77:$D$4115,<1000)" would return an error.  I decided to create 2 seperate columns to set my criteria for the goal ranges under the "J" and "K" columns.  I then populated the new columns with my ranges.  For example range "J3" conatins ">=1000 and range "K3" conatins "<5000".  This altered my formula to: "=COUNTIFS(Kickstarter!$F$77:$F$4115,"successful",Kickstarter!$R$77:$R$4115,"plays",Kickstarter!$D$77:$D$4115,$J$3,Kickstarter!$D$77:$D$4115,$K$3)".  This work around fixed my error and I then decided to hide the columns for presentation.
---
**Results:**
* From the collected data we can see two key features from the launch dates of projects.  The first being that timing seems to be important for successful funding.  There are a high number of successful projects in May and June indicating that these months would likely be best to start a new project. However, October has a high rate of failure when starting a new project, indicating that this month should likely be avoided.  The second key feature would be that kickstarters for theatrical plays have a decent chance of being funded throughout the year.  There is an average of 61% success rate for all plays across the provided data set.
---
* Given the data we have, based on the goals of the kickstarter projects; we can determine that projects under $10,000 have a good chance of being successful and that projects within the $1000 and $5000 range have the most success.
---
* The limitations of this dataset would include the lack of information given on the failed projects.  While we can assume the projects failed based on launch date and or funding, we have no real evidence of the amount of exposure each kickstater received.  Had a kickstarter recieved a large following given some advertisment or incentives from the campaign the number of failures may very well have been different.  Also, there is no information given for the successful campaigns on if they offered any incentives or advertising to help ensure funding.
---
We could create additonal graphs to deatil the funding amounts against the launch dates to see if there's a correlation between the goal amount and when the project was launched.  This would combine what information we have into a single graph to determine if either of these factors influence each other.  Would a larger goal started in May be successful? or would a smaller goal started in October be successful? We could also graph the average donation against the success rate to see if the successful projects had larger donations making thier funding easier to get.
