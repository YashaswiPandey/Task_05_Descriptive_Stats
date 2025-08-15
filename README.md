# Task_05_Descriptive_Stats

This task evaluates the ability of a Large Language Model (LLM) to answer progressively complex analytical questions when provided with a compact, real-world dataset. The dataset used is the final table of the English Premier League from 1993 to 2024.

## Dataset

- The dataset can be downloaded from [Kaggle](https://www.kaggle.com/datasets/evangower/english-premier-league-standings/data/)  
- The file contains the final league table at the end of each season starting from 1992/93 to 2023/24  
- There are twelve columns that contain information such as year, team name, games played, wins, defeats, ties, goals scored, goals conceded, position, goal difference and points  
  
## LLM Responses

**1**
> which team has finished at position 1 most number of times?

ChatGPT & DeepSeek
Both calculated Manchester United with 13 times

**2**
> which team has the best goal scoring record over a period of 3 years

ChatGPT & DeepSeek
Both calculated Manchester City with 303 goals between 2017-2019

**3**
> which team conceded the least goals over a period of 3 years

ChatGPT & DeepSeek
Both calculated Chelsea with 61 goals between 2005-2008

**4**
> which team had the worst goal scoring over a period of 3 years

ChatGPT & DeepSeek
Both calculated Crystal Palace with 116 goals<br>
After verifying with code, both got this answer wrong, when  asked why, they said they did not check for only consecutive years

**5**
> which team had the worst goal conceded over a period of 3 years

ChatGPT & DeepSeek
Both calculated West Brom with 196 goals between 2017-2019<br>
After verifying with code, both got this answer wrong, when  asked why, they said they did not check for only consecutive years

**6**
> which team deteriorated the most from 2023 to 2024 but avoided relegation

ChatGPT 

Identified Brentford as the team that detoriated the most as they dropped 7 positions  

DeepSeek

Identified Chelsea and Manchester United as the team that detoriated the most, DeepSeek reasoned that since they were higher up in the table their deteoriation was worse as they are expectd to be better.


**7**
> As a coach of Brentford, if I wanted to win two more games this coming season, should I focus on offense or defense and If so, why

ChatGPT and DeepSeek both identified the defense as the issue, this is because they conceded 65 goals and since their goals scored was better than teams in the bottom half of the table.

Code shows that Brentford scored more goals on average than 5 teams just above them, but ended up conceding more goals on average when compared, thus both correctly identified that Brentford should focus on defense.


As we can see that both ChatGPT and DeepSeek can get easy calculations right but we need to use better wording when asking to solve complex problems.