# Business Understanding
This company provides insights into NBA player performance by analyzing statistical data to identify star players. Those with exceptional skill, impact, and/or potential. It goes beyond surface-level data such as points, rebounds, and assists, by also analyzing advanced metrics such as BPM.
# Data Lifecycle


![datacucle](https://github.com/user-attachments/assets/0d24a472-dfdc-44d8-8661-6cd940d11605)

## Business Problem
### Question: How can someone identify a "Star" in the NBA?
I'm approaching this question by looking at various honors that are awarded at the end of each season based on a player's statistics, both in the regular season and the playoffs. I want to make a note that once a person is considered a "star" one season, it is very hard for them to lose that title. It often takes multiple seasons of poor production. Some of the "stars" identified may be on a downward slope, and on the contrary, we may be able to predict who is going to be a "star" in the near future, along with recognizing current "stars". 

## Data Collection
The datasets that my business collects are statistics the box scores of NBA games. It also can go deeper into calculated statistics from the NBA websites, and other non-NBA affliated cites such as basketball-reference.com and statmuse.com.
## Data Processing
To process the data, we must extract the statistics that matter and make sure that every player qualifies for what we're looking for. For an example if a player plays for 1 minute and scores 3 points, their stats per 36 minute would be 108 points. Statistics like that give a false impression of players performance and may interfere with the true objective of this analysis.
## Data Analysis
The Most Valuable Player (MVP) award is rewarded to the most outstanding players who have the biggest impact on their team and are the most dominant. Due to the definition of the award, this is what I used to determine the standards of a star. It is important to note, just because someone has not been an MVP candidate does not mean that they are not a star. Some factors that may prevent a star from being an MVP candidate are how the media perceives them and their teams overrall success. There are cases of the media considering someone a star solely off their swagger and how they act. An example of someone with exceptional stats who wasn't considered an MVP candidate, but is most definitely a star, is Trae Young. In the 2021-2022 season, Trae Young led the league in points and assist, but was not even close the being considered MVP due to his team's poor record. The most important statistic I found while researching was Box Plus Minus(BPM). Box Plus Minus is an advanced statistic that calculates a player's contribution to their team's performance on the court, measured in points per 100 possessions. It is based only on the information in the traditional basketball box score. It is a purely rate stat and is adjusted according to position. The league average is defined as 0.0. 
To give a scale from basketball-reference.com:
- -2.0 is a bench player
- 0.0 is a starter
- +2.0 is a good starter
- +4.0 is an all-star candidate
- +6.0 is an all-NBA candidate
- +8.0 is an MVP candidate
- +10.0 is an all-time season 

## Data Presentation
<img width="460" alt="Screenshot 2025-05-08 at 11 00 59 AM" src="https://github.com/user-attachments/assets/60130551-99b9-498a-852b-9c027d4e9fe1" />

This is a graph of the top 9 MVP candidates from the 2023-2024 season (listed in order from 1-9, left-right) vs. their BPM. The graph lists the top candidate (Nikola Jokic) on the left and the bottom candidate (Kevin Durant) on the right. As you can see, this graph shows the decline between BPM and ranking as an MVP candidate. There are a few outliers in this graph, but that can be explained by the other statistics and overrall team success.

# Step 1: Data Analysis + Processing in Excel
There are currently 78 seasons in the National Basketball Association(NBA). I filtered out the last 10 complete seasons and sorted them in a table chronologically, and then removed unnecessary rows and sorted the players by points scored in the season. After sorting, I highlighted the regular season MVPs and added the highest Box Plus Minus(BPM) per season. 
<img width="1261" alt="Screenshot 2025-05-08 at 1 10 06 PM" src="https://github.com/user-attachments/assets/53fa0ca5-baf5-41b5-a76c-484a67c21460" />
###### Ex. 2023-2024 Regular Season

After adding the highest BPM, I went to the playoffs for the last 10 seasons, and highlighted the Eastern Conference Final MVP in a light green, and the Western Conference Final MVP in a light yellow. There are only 3 of each award because the award was introduced 3 years ago. Finally, I bolded the Finals MVP. Again, I want to make a note that the data on Finals MVP must be analyzed very carefully for these reasons:
- The Finals MVP can only be between the two teams that made it NBA Finals
- It is only based on the 4 - 7 game series of the Finals, not the entire playoffs, meaning it's a very small sample size
- It is often rewarded to the best player on the team that wins the finals, meaning it is more dependent on others, which isn't exactly what we're analyzing
- It is a vote by 11 media panelists
  -   Since it is a vote, it can often be skewed by the media or the popularity of a player.
  -   Since it is a vote, it's technically an opinion.
<img width="1365" alt="Screenshot 2025-05-08 at 1 10 25 PM" src="https://github.com/user-attachments/assets/377490a6-6202-4b1f-9c56-5bceb4b53403" />

###### Ex. 2021-2022 Playoffs

# Step 2: Data Analysis + Processing in Python
In addition to analyzing the data in Excel, I also used a Python notebook (.ipun) to process and analyze my data. I imported the CSV module and then opened the last 10 complete Regular Seasons and the last 10 complete Playoffs. First, to get a grasp of the CSV functions, I opened the regular season CSV as a readable file, and printed the headers and the first 5 rows of data. Upon doing that, I noticed that there was also unnecessary data in this set. Appropriately, the next step was to open the regular season file, then rewrite only the data columns the were crucial to analyze the data. After removing the 4 nonessential columns, I used a basic for loop to print the adjusted CSV into a new file, and repeated the same steps for the Playoffs Data.

This is a fictitious scenario created by the GitHub author for academic purposes only.
