# Exploratory Analysis of RAPTOR Metrics in the Modern NBA

## Project Overview
RAPTOR (Robust Algorithm (using) Player Tracking (and) On/Off Ratings) is a modern-day plus-minus statistical analysis developed by FiveThirtyEight. This system measures the number of points a player contributes to his team’s offense/defense per 100 possessions, relative to a league-average player. Our team analyzed the `latest_RAPTOR_by_team.csv` (play-by-play metrics from the 2022-2023 NBA season) and the approximate `historical_RAPTOR_by_team.csv` charts (predictive analyses dating from 1977-2022) uncovering comparisons between both sets of data across a variety of criteria. 

## Installation and Usage Instructions of Libraries/Tools
We are utilizing two datasets within FiveThirtyEight's RAPTOR database:

- [Latest RAPTOR Analytics by Team](https://projects.fivethirtyeight.com/nba-model/2023/latest_RAPTOR_by_team.csv) 
- [Historical RAPTOR Analytics by Team](https://github.com/fivethirtyeight/data/blob/master/nba-raptor/historical_RAPTOR_by_team.csv) 

### Required Libraries:
- Pandas
- Numpy
- Matplotlin
- Scipy, stats module.
- Seaborn
- Plotly.graph_objects
- Plotly.express.
### Tool(s) required:
- Jupyter notebook,pyviz environment.
## Intro
RAPTOR (Robust Algorithm (using) Player Tracking (and) On/Off Ratings) is a modern-day plus-minus statistical analysis developed by FiveThirtyEight. The main component of this  system measures the number of points a player contributes to his team’s offense/defense per 100 possessions, relative to a league-average player.  

***Why RAPTOR?***    

RAPTOR fulfills two long-standing goals:
- First, to create a publicly available statistic that takes advantage of modern NBA data, specifically player tracking and play-by-play data that isn’t available in traditional box scores.
- Second, and relatedly,  a statistic that better reflects how modern NBA teams actually evaluate players.

## Project Goals
- Does the amount of possessions per player greatly impact that player’s overall RAPTOR ratings? Why or why not?
- Which team displayed the highest/lowest RAPTOR ratings across the 2022-23 season across all players? How does this data compare to their predictive PREDATOR model?
- How accurate are the overall results of predictive-RAPTOR, which was used for the historical data charts (1977-2013), compared to those of modern - RAPTOR’s integration (2013-Present)? 
- Is there a relationship between most minutes played and the greatest pace impact on the team compared to RAPTOR scores?
- How do these statistics line up by player in relation to the top players/teams (MVPs) of the 2022-2023 season?
- Find out relationship between different features.

## Data Cleaning
There are two separate datasets for this challenge, the historical dataset which includes data from 1977-20xx and the latest dataset which is for 2023  
The first step was to import the datasets and then merge them  
Then the datasets were checked for null values, there were some null values under historical data which was then filled and checked for duplicates, finally giving us our clean dataset to work with.
## Analysis
After merging and cleaning the datasets, we defined some functions which were used through out our notebook.   
we started our data exploration by looking at the average distribution of PREDATOR total, RAPTOR total and WAR total. ![histogram](/Visuals/histogram.png) 
Our main goal was to evaluate how different variables influence the RAPTOR scores and if there is correlation between those and to compare the RAPTOR results to actual results.![Correlation](/Visuals/Correlation.png)
The first variable we looked at was the amount of possessions per player. we did this by creating a scatter plot and a regression line, which showcased a weak but positive correlation.  
Along with the number of possessions, minutes played also play an important role in a player's performance when we compared average minutes played by a player with their RAPTOR scores we found out that there was a weak positive correlation as well.  
Lastly we wanted to compare a player's pace impact in their team with their RAPTOR scores, we uncovered a negative correlation. We can conclude that although RAPTOR scores are effected by number of possessions and the minutes played, it isn't a strong correlation.  
Now that we had covered individual RAPTOR scores, we wanted to look at the teams. We continued looking at a team's highest and lowest RAPTOR scores across 2022-2023 season and compared it to their PREDATOR scores. Atlanta Hawks ranked first and Portland Trail Blazers ranked last. For the PREDATOR top was ___ and the bottom was ___.  
Next we wanted to look at how accurate the overall PREDATOR was which was used for historical dataset when comapred to modern RAPTOR integration.  
The average RAPTOR total with the latest data shows more trends, because starting from 2013-14 player-tracking data became available online. The historical data uses a limited range of variables. With more data available, more accurate readings can be done as shown.  
Lastly we wanted to evalute How do these statistics line up by player in relation to the top players/teams (MVPs) of the 2022-2023 season  
The RAPTOR metrics used to identify the top players and teams were raptor total, raptor box total, raptor offense, raptor defense, raptor on/off total, war total, minutes played and possessions. Our statistical results line up with the top players and top teams for the 2022-2023 season. Our top player result is the NBA finals MVP and the top team result won the championship this season  
The top player for the 2022-2023 season is Nikola Jokic and the top team for the 2022-2023 season is the Denver Nuggets.

## Visuals

![Boxplot](/Visuals/Boxplot.png)

![Lebron](/Visuals/Lebron.png)
![Without Lebron](/Visuals/Lebronless.png)
![LeBron vs Kobe Line Plot](/Visuals/LeBronvsKObepng.png)


## Additional Explanations

## Major Findings
- If we look at indvidual total RAPTOR scores, John Stockton is at number 1 where as for the average RAPTOR scores it is Stanley Umude.
- For the teams, the highest RAPTOR scores is ___ and the highest average is ____
- Accuracy of RAPTOR : 
## Limitations
- Advanced metrics
- Poor performing out-of-sample variables in constructing RAPTOR are avoided for PREDATOR
## Conclusions

## References 
For dataset : [FiveThirtyEight](https://fivethirtyeight.com/features/how-our-raptor-metric-works/)  
[for importing image](https://mljar.com/blog/jupyter-notebook-insert-image/)  
[Seaborn](https://seaborn.pydata.org/)  
[Plotly](https://plotly.com/python/)  
Specific debugging and code reference are included in comments before the code.
## Team Members
- [Christopher](https://github.com/cbake105)
- [Jack](https://github.com/jackhayes21)
- [Jonathan](https://github.com/jccrock311)
- [Uzma](https://github.com/UzmaSayyeda)
- [Wipawadee](https://github.com/wnaiyakhu)