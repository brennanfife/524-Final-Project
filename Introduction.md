The first few sentences should give a quick overview of the entire project. Then, elaborate with a description of the problem that will be solved, a brief history (with citations) of how the problem came about, why it's important/interesting, and any other interesting facts you'd like to talk about. You should address and explain where the problem data is coming from (research? the internet? synthetically generated?) Also give an outline of the rest of the report.

This section should be 300-600 words long, and should be accessible to a general audience (don't assume your reader has taken the class!). Feel free to include images if you think it'll be helpful:

# Introduction
Since the 1940s, NBA teams have utilized specialized tools, statistics, and models to assist them in constructing optimal lineups. As listed by [nbastuffer.com](https://www.nbastuffer.com/analytics101/nba-teams-that-have-analytics-department/), every NBA team currently has an analytics department, supplying their organizations with knowledge of how to best match current rosters with offseason transactions. Even popular games such as the NBA 2K series to ESPN's Fantasy Basketball League, have given hardcore fans the chance to craft a fantasized lineup for their favorite clubs. With such demand, we will examine two models one can take to assist them in selecting for an optimal, fantasized NBA lineup. 


**In our first model**, we look to maximize a team's winning percentage by selecting players they would want. By using a player's offense rating and defense rating, plus the player's salary (provided by [basketball-reference.com](https://www.basketball-reference.com/contracts/players.html)) we are able to provide various lineups for team's. In creating this model, we used Mixed Integer Linear Programming. Whereas linear programming maximizes (or minimizes) a linear objective function (subject to one or more constraints), mixed integer programming adds one additional condition that at least one of the variables can only take on integer values. Thus, giving us the decision to whether or not to choose a specific player based around other statistics. Here, we assumed each team consisted of 5 starters and 5 bench players, assigning two of them to each position. We then place our variables in the given objective function, which all data was taken from the 2018-2019 season (provided by [NBAstatstuffer.com](https://www.nbastuffer.com/2018-2019-nba-player-stats/)). 

| Player                | Position | Off % | Def % |
|-----------------------|----------|-------|-------|
| Rudy Gobert           | C        | 133.8 | 96.7  |
| Giannis Antetokounmpo | F        | 121.6 | 93.9  |
| Derrick Favors        | F        | 124.5 | 98.1  |
| James Harden          | G        | 118.6 | 103.5 |
| Eric Bledsoe          | G        | 115.8 | 101.0 |

**Win Percentage: 69.4%**


**In the second model**, we seek to maximize the sweet spot of each team by using tradeoff to select players based on the sweet spot distribution and the total amount of sweet of a lineup. Here, the data was synthetically generated with x, y coordinate depending on the player's position (e.g. center shooting near the rim while guards shoot 3-pointers). We have thirty players and pick up 5, with each lineup consisting of two guards, two forwards, and one center. The offensive area is only focused on halfcourt (the shooting area).

In both of these models, we first provide the mathematical models and present the corresponding code. Then, we examine the results, provide data interpretation, remarks and limitations on the models, and any possible improvements that could be made on our models.
