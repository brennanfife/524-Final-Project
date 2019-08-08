# Introduction
Since the 1940s, NBA teams have utilized specialized tools, statistics, and models to assist them in constructing optimal lineups. As listed by [nbastuffer.com](https://www.nbastuffer.com/analytics101/nba-teams-that-have-analytics-department/), every NBA team currently has an analytics department, supplying their organizations with knowledge of how to best match current rosters with offseason transactions. Even popular games such as the NBA 2K series to ESPN's Fantasy Basketball League, have given hardcore fans the chance to craft a fantasized lineup for their favorite clubs. With such demand, we will examine two models one can take to assist them in selecting for an optimal, fantasized NBA lineup. 

**In our first model**, we look to maximize a team's winning percentage by selecting players around their offensive and defensive efficiency rating from the 2018-2019 NBA season (provided by [NBAstatstuffer.com]((https://www.nbastuffer.com/2018-2019-nba-player-stats/))), salaries (provided by [basketball-reference.com](https://www.basketball-reference.com/contracts/players.html)) salary caps, and weighted experience. This model takes advantage of Mixed Integer Linear Programming. Whereas linear programming maximizes (or minimizes) a linear objective function (subject to one or more constraints), mixed integer programming adds one additional condition that at least one of the variables can only take on integer values. Thus, we get a decisive decision on who to select and not to select. An example would appear as such...

| Player                | Position | Off % | Def % |
|-----------------------|----------|-------|-------|
| Rudy Gobert           | C        | 133.8 | 96.7  |
| Giannis Antetokounmpo | F        | 121.6 | 93.9  |
| Derrick Favors        | F        | 124.5 | 98.1  |
| James Harden          | G        | 118.6 | 103.5 |
| Eric Bledsoe          | G        | 115.8 | 101.0 |

**Win Percentage: 69.4%**

**In the second model**, rather than using efficiency ratings, we apply a player's shooting 'sweet spot'. By utilizing tradeoff between the sweet spot distribution vs. the total sweet, we can calculate the optimal lineup a team can have on the court. In this model, we synthetically generated x, y coordinates, corresponding to halfcourt, accounted for a player's abilities (e.g., stars, rookies), and their positions (e.g., centers shoot near the rim, whereas guards shoot 3-pointers). From thirty players, we pick a lineup of 5 (two guards, two forwards, and a center). 

[PICTURE OF NBA COURT AND/OR AN EXAMPLE OF THE CORRESPONDING TABLE FOR MODEL 2 (LIKE ABOVE) HERE]

In both of these sets, we first provide the mathematical model and the corresponding code, we examine results, offer our interpretations of the data, any limitations we experienced, and possible improvements that could be made for future use.
