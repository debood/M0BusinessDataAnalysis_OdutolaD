# Business Understanding

# Data Lifecycle


![datacucle](https://github.com/user-attachments/assets/0d24a472-dfdc-44d8-8661-6cd940d11605)

## Business Problem
### Question: How can someone identify a "Star" in the NBA?
I'm approaching this question by looking at various honors that are awarded at the end of each season based on a player's statistics, both in the regular season and the playoffs. I want to make a note that once a person is considered a "star" one season, it is very hard for them to lose that title. It often takes multiple seasons of poor production. Some of the "stars" identified may be on a downward slope, and on the contrary, we may be able to predict who is going to be a "star" in the near future, along with recognizing current "stars". 

## Data Collection
The datasets that my business collects are statistics the box scores of NBA games. It also can go deeper into calculated statistics from the NBA websites, and other non-NBA affliated cites such as basketball-reference.com and statmuse.com.
## Data Processing
To process the data, we must extract the statistics that matter and make sure that every player qualifies for what we're looking for. For an example if a player plays for 1 minute and scores 3 points, their stats per 36 minute would be 108 points. Statistics like that give a false impression of players performance and may 
## Data Analysis
## Data Presentation

## Step 1: Data analysis and processing in Excel
There are currently 78 seasons in the National Basketball Association(NBA). I filtered out the last 10 complete seasons and sorted them in a table chronologically, and then removed unnecessary rows and sorted the players by points scored in the season. After sorting, I highlighted the regular season MVPs and added the highest Box Plus Minus(BPM) per season. Box Plus Minus is an advanced statistic that calculates a player's contribution to their team's performance on the court, measured in points per 100 possessions. It is based only on the information in the traditional basketball box score. It is a purely rate stat. The league average is defined as 0.0. 
To give a scale from basketball-reference.com:
-2.0 is a bench player
0.0 is a starter
+2.0 is a good starter
+4.0 is an all-star candidate
+6.0 is an all-NBA candidate
+8.0 is an MVP candidate
+10.0 is an all-time season

After adding the highest BPM, I went to the playoffs for the last 10 seasons, and highlighted the Eastern Conference Final MVP in a light green, and the Western Conference Final MVP in a light yellow. There are only 3 of each award because the award was introduced 3 years ago. Finally, I bolded the Finals MVP. Again, I want to make a note that the data on Finals MVP must be analyzed very carefully for these reasons:
- The Finals MVP can only be between the two teams that made it NBA Finals
- It is only based on the 4 - 7 game series of the Finals, not the entire playoffs, meaning it's a very small sample size
- It is often rewarded to the best player on the team that wins the finals, meaning it is more dependent on others, which isn't exactly what we're analyzing
- It is a vote by 11 media panelists
  -   Since it is a vote, it can often be skewed by the media or the popularity of a player.
  -   Since it is a vote, it's technically an opinion.




This is a fictitious scenario created by the GitHub author for academic purposes only.
