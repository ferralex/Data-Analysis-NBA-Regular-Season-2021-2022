# Data-Analysis-NBA-Regular-Season-2021-2022
Data Analysis in MS Excel

*For a better formatting check [here](https://www.alessandroferrarese.com/data-analysis-nba-regular-season-2021-2022/)*

## Introduction
Basketball is one of my biggest passion. I used to be part of a team and play for 7 years.

In order to practice what I’ve recently studied about Excel and Data Analysis, I decided to analyze data about the last NBA season, the professional American basketball league.

## The Dataset
[This](https://www.kaggle.com/datasets/vivovinco/nba-player-stats) is the Dataset I used for my analysis (from Kaggle). The column descriptions are listed and explained on the Kaggle page.

The archive contains two .csv files, one with the data regarding the regular season and one with the data about the playoffs (post-season).

I will focus on the regular season.

## Ask
*What is the youngest team? What is the oldest team?*

*What’s the age average per role?*

*Who are the players with the highest minutage per game?*

*What are the stats grouped by role?*

*Which role is the best for every “task”?*

*Who is the best player for 3 point shoots?*

*Who is the best player in each “task”?*

*And more…*

## Prepare
At a first look, the dataset seems to contain duplicates.

![1](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/duplicates.jpg)

Looking at the column *Tm* (Team) I notice *“TOT“*. TOT means “Two Other Teams” meaning that a player played for two (or more) teams that season.

This might create problems when searching for insights about teams or players.

I start “trimming” and fixing the letter case of the columns containing text, I make sure that the other columns are in order as well (numbers properly formatted and no unwanted values).

In order to avoid mistakes while getting insights, I decide to work on 2 datasets: one for teams-related analysis and one for players-related analysis.

## Process
For the players’ dataset, I keep the records having TOT in the Team column in the case a player appears more than once. The statistics are already the sum or the avg of those listed in the other teams of which that player was part.

Other players’ records don’t need any modification.

![2](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/Players.jpg)

For the teams’ dataset, I remove those players with TOT listed in their team (when extracting insights about teams, the data is about a whole year, including the players who have changed teams. If I wanted to analyze the roster at the end of the season performance, I had to keep only the player’s record with their last team).

## Analyze
Let’s start extracting and analyzing some data about the players age during the season.

![3](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/age_ok-1024x468.jpg)

The average age of the NBA players is 25.7 years and the oldest active player is 41 years old, Udonis Haslem. He has double the age of 40 other players! (11 players at 19 years old + 29 players at 20 years old).

Many guys in their 20s are running and jumping on the parquet but, being over 24 is maybe not a good thing for the NBA teams? Starting from 25 years old, there is a constant drop in the number of players.

**What is the youngest team? What is the oldest team?**

![4](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/oldest_youngest_team.jpg)

**What’s the age average per role?**

![5](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/age_average_per_role.jpg)

**Who are the players with the highest minutage per game?** (considering only players who have been active for at least 41 games, half of the season)

![6](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/most_minutage.jpg)

**Who are the players who played most games?**

![7](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/most_played_games.jpg)

**What are the stats grouped by role?**

![8](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/stats_by_role.jpg)

**Which role has the highest realization percentage?**

![9](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/realization_by_role.jpg)

**Which role is the best for every “task”?**

![10](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/stats_by_role_chart.jpg)

**Who is the best player for 3 point shoots?** (considering only those players with an average of at least 5 attempts per game).

![11](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/best_3_points_shooter.jpg)

![12](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/best_3_points_player_chart.jpg)

**What’s the best team for 3 points?**

![13](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/best_3_points_team.jpg)

**Who is the best in each “task”?**

![14](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/final_stats.jpg)

## Conclusions
So many insights can be discovered from this dataset. While operating on it I wanted to find out more and more about the last NBA season!

This analysis has been an opportunity for me to learn more and understand my mistakes.

I realized how important is the preparation phase. Having everything organized, especially in your mind, can save a lot of precious time and stop you from making mistakes.

Here is what happened to me:

![15](https://www.alessandroferrarese.com/wp-content/uploads/2022/06/age_wrong-1024x441.jpg)

I started with too much enthusiasm and didn’t think about those players listed more than once (because they played in more than one team). Because of that, the above representation is wrong.

This experience was also very useful to practice Excel and pivot tables, a powerful and fundamental tool.
