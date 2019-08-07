The first few sentences should give a quick overview of the entire project. Then, elaborate with a description of the problem that will be solved, a brief history (with citations) of how the problem came about, why it's important/interesting, and any other interesting facts you'd like to talk about. You should address and explain where the problem data is coming from (research? the internet? synthetically generated?) Also give an outline of the rest of the report.

This section should be 300-600 words long, and should be accessible to a general audience (don't assume your reader has taken the class!). Feel free to include images if you think it'll be helpful:

# Introduction

This report seeks to design optimization models around selecting NBA players for an NBA team. Since the 1940s, NBA teams have used specialized tools, statistics, and models to develop an optimal roster. As mentioned by [nbastuffer.com](https://www.nbastuffer.com/analytics101/nba-teams-that-have-analytics-department/), every team in the NBA has an analytics dept, stressing the importance of player statistics. Popular games, such as the NBA 2K to ESPN's Fantasy Basketball League have grown in popularity over the past decade, giving fans the ability to design their own teams. In this report, we will examine two models one can use in helping them select an optimal NBA basketball team. An example of what one could expect is listed below.


In our first model, we look to maximize a team's winning percentage by selecting players they would want. By using a player's offense rating and defense rating, plus the player's salary (provided by [basketball-reference.com](https://www.basketball-reference.com/contracts/)) we are able to provide various lineups for team's. In creating this model, we used Mixed Integer Linear Programming. Whereas linear programming maximizes (or minimizes) a linear objective function (subject to one or more constraints), mixed integer programming adds one additional condition that at least one of the variables can only take on integer values. Thus, giving us the decision to whether or not to choose a specific player based around other statistics. Here, we assumed each team consisted of 5 starters and 5 bench players, assigning two of them to each position. We then place our variables in the given objective function, which all data was taken from the 2018-2019 season (provided by [NBAstatstuffer.com](https://www.nbastuffer.com/2018-2019-nba-player-stats/)). 

| Player                | Position | Off % | Def % |
|-----------------------|----------|-------|-------|
| Rudy Gobert           | C        | 133.8 | 96.7  |
| Giannis Antetokounmpo | F        | 121.6 | 93.9  |
| Derrick Favors        | F        | 124.5 | 98.1  |
| James Harden          | G        | 118.6 | 103.5 |
| Eric Bledsoe          | G        | 115.8 | 101.0 |

**Win Percentage: 69.4%**


In the second model, we seek to maximize the sweet spot of each team by using tradeoff.
Here, the data was sythetically generated.

In both of these models, we first provide the mathematical models and present the corresponding code. Then, we examine the results, provide data interpretation, remarks and limitations on the models, and any possible improvements that could be made on our models.
