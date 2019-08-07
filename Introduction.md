The first few sentences should give a quick overview of the entire project. Then, elaborate with a description of the problem that will be solved, a brief history (with citations) of how the problem came about, why it's important/interesting, and any other interesting facts you'd like to talk about. You should address and explain where the problem data is coming from (research? the internet? synthetically generated?) Also give an outline of the rest of the report.

This section should be 300-600 words long, and should be accessible to a general audience (don't assume your reader has taken the class!). Feel free to include images if you think it'll be helpful:

# Introduction

This report seeks to design optimization models around selecting NBA players for an NBA team. Since the 1940s, NBA teams have used specialized tools, statistics, and models to design optimal rosters. Popular games, such as the NBA 2K basketball video game series, to ESPN Fantasy Basketball have grown in popularity over the past decade, giving hardcore fans the ability to design their own teams. In this report, we will examine two models one can use in helping them select an optimzal NBA basketball team.

In our first model, we look to maximize a team's winning percentage by selecting players they would want. By using a player's offense and defense ratings, plus the player's salary provided by [basketball-reference.com](https://www.basketball-reference.com/contracts/). In creating this model, we used Mixed Integer Linear Programming. Here, we assumed each team consisted of 5 starters and 5 bench players, assigning two of them to each position. We then place our variables in the given objective function, which all data was taken from the 2018-2019 season (provided by [NBAstatstuffer.com](https://www.nbastuffer.com/2018-2019-nba-player-stats/)). 


In the second model uses tradeoff to The second one is based on maximizing the sweet spot of each team.

In both of these models, we first provide the mathematical model we are using, then present the code. Finally, we provide additional results and remarks on how the model interprets the data, plus where the model could be improved.
