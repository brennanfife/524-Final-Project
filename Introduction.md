# Introduction

This report seeks to design optimization models around selecting NBA players for an NBA team. Ever since the 1940s, NBA teams have dished out millions to people who use specialized tools and statistics to calculate the optimal roster, all in the hopes of bringing their respective city an NBA championship. Popular online games, ranging from basketball video games to fantasy basketball have grown in popularity over the past decade, giving fans the ability to design their own team given specific scenarios. In this report we will examine two models one can use in helping them select and optimzie a NBA basketball team.

In our first model, we look to maximize the winning percentage of a team. In creating this model, we used Mixed Integer Linear Programming. Here, we assumed each team consisted of 5 starters and 5 bench players, assigning two of them to each position. We then place our variables in the given objective function, which all data was taken from the 2018-2019 season. The second one is based on maximizing the sweet spot of each team.

#### Variables
| Variables        | Descriptions            |Type   |
|------------------|:------------------------|------:|
| $p_i$            |player $i$               |binary |
| $ofr_i$          |Off rating of player $i$ |Real   |
| $dfr_i$          |Def rating of player $i$ |Real   |
| $s_i$            |Salary of player $i$     |Real   |
| $SC$             |Salary Cap               |Real   |


In the second model uses tradeoff to 

In both of these models, we first provide the mathematical model we are using, then present the code. Finally, we provide additional results and remarks on how the model interprets the data, plus where the model could be improved.
