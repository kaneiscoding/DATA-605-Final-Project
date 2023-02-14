# League of Legends eSports
### By [Kane Smith](https://github.com/kaneiscoding)
### Data 605: Actionable Visualization & Analytics

<img src="assets\logo.png" alt="League of Legends Logo" width="650"/>

<br> <br> 

## Table of Contents
- [Introduction](README.md#introduction)
- [Guiding Questions](README.md#guiding-questions)
- [Dataset](README.md#dataset)
- [Methodology](README.md#methodology)
- [Tools](README.md#tools-used)
- [Q1: What team has been the best in their region?](README.md#question-1-what-team-has-been-the-best-in-their-region)
- [Q2: What team has been the best internationally?](README.md#question-2-what-team-has-been-the-best-internationally)
- [Q3: Who has been the best in their respective role?](README.md#question-3-who-has-been-the-best-in-their-respective-role)
- [Q4: What are the most important factor in winning a game?](README.md#question-4-what-are-most-important-factors-in-winning-a-game)
- [Q5: What Champions Have Been the Best Throughout the Years?](README.md#question-5-what-champions-have-been-the-best-throughout-the-years)
- [Final Thoughts](README.md#final-thoughts)
- [References](README.md#references)

<br> <br> 

## Introduction 

Traditional sports has become dominated by data and analytics. From the decisions made by a team such as what players to aqurire, how to play, etc. to the debate between fans of who is better than who by comparing their statistics. The same can be said for an much newer, emerging sport known as eSports where people compete against each other virtually. One of the most popular eSports games for the past decade has been League of Legends. I will bring the data-driven debate to the virtual domain to see if some of the age old questions can be answered.

### What is League of Legends?

League of Legends (sometimes refered to as LoL) is a multiplayer online battle arena game where two teams of five players each battle against each other with the goal of destroying the enemy team's base (called the Nexus) while defending their own. Players choose from a roster of over 150 unique champions with different abilities and play styles to strategically coordinate attacks and defenses in real-time combat. 

The arena has 4 main sections. Top lane, Middle lane, Bottom lane, and the area between each lanes are called the Jungle.

Each team's players are assigned to a different position:
- Top: This player will spend most of the game in the top lane.
- Middle: This player will spend most of the game in the top lane.
- Jungle: This player will spend most of the game in the Jungle moving between all ofthe lanes to help their teammates.
- Damage and Support: Both of these players spend most of the game in the bottom lane together.

<img src="https://github.com/kaneiscoding/DATA-605-Final-Project/blob/main/Graphics/roles-map-mobafire.png"  alt="Roles" width="900">
(Credit: Mobafire)

### What is League of Legends E-sports?
Now that we understand the basics of the game, what does the competitve scene look like?

There are 4 main regions (leagues):
- South Korea (LCK)
- China (LPL)
- Europe (LEC)
- North America (LCS)

The teams in each region compete against each other throughout the season, broken up into two splits (Spring and Summer). At the end of spring and summer, a team is crowned the champion of their respective region. In between the spring and summer, the top teams of each region are invited to an international tournament called the Mid Season Invitational (MSI) to compete against each other to see who is the best in the world. At the end of the season, the best teams for each region qualify for the World Championship where all teams compete to see who is the best in League of Legends for that season. 

Visually, a League of Legends season will look like this:

<img src="\Graphics\season-schedule.png"  alt="Schedule" width="450">
<br>

## Guiding Questions

To formate my guiding questions, I refrenced common debates in traditional sports, such as who is the best team?, who is the best player? etc. However, unlike like traditional sports league like the NBA and NFL, League of Legends has a domestic component and an international component, so these questions had to be analyzed through both lens.

Throughout this article we will aim to answer 5 main questions:
1. What team has been the best in their region?
2. What team has been the best internationally?
3. Who has been the best in their respective role?
4. What are the most important factors in winning a game?
5. What Champions Have Been the Best Throughout the Years?

<br>

## Dataset

The dataset was collected by Tim Sevenhuysen from [Oracles Elixir](https://oracleselixir.com/). It contains data for every professional match played from 2014 up until now. He collected this data by scraping it from the official League of Legends eSports website, the League of Legends wiki, and Riot's eSports API and aggregating it together using Python. Many professional coaches, anaylsts and caster use his data to gain deeper understanding of the game. 

For our analysis, years 2014-2017 have been left out, as during this time the eSports scene was very volatile with many players having short careers along with teams coming in and out of the scene frequently. In 2018, Riot, the developers of League of Legends decided to franchise their leagues, giving stability and an injection of money to the teams and players making it more like a traditional sports league.

<br>

## Methodology

During my analysis I used the following methodology:

1. Define the question
2. Clean and wrangle the data
3. Data analysis
4. Data Visualization
5. Conclusion

<br>

## Tools Used:
- Microsoft Excel and Python to clean the data
  - Python packages used: [Matplotlib](https://matplotlib.org/), [Numpy](https://numpy.org/), [Pandas](https://pandas.pydata.org/)
- [Tableau](https://www.tableau.com/) to create visualizations
- GitHub for version control and GitHub Pages to create this blog 

<br>

## Question 1: What team has been the best in their region?

To begin my analysis, I want to know which team has performed the best in their respective region (North America, China, Korea, and EU) between 2018-2022. 

<img src="/Graphics/Q1%Annotated.png"  alt="Question 1" width="900">

We can see from the visualization above that Gen.G has performed the best in the LCK (Korea), however not by much when compared to the other top 4 teams. In North America (LCS), Cloud9 has clearly been the best team in terms of win percentage. They have qualified for the World Championship every year since their inception in 2014. In Europe (LEC) we see similar parity as in Korea with G2 Esports being the best and Fnatic following closely behind. Interestingly, between 2015 and 2020 only G2 or Fnatic had won the domestic title. In China (LPL), there is a clear best being Top Esports.

All of these teams are considered the best and are considered staples in their respective regions, often being the regulars in playoffs and international tournments.

<br>

## Question 2: What team has been the best internationally?

We've seen who performs the best in their region, but what about internationally. The international tournaments are considered the most prestigous as that's when you compete again all of the best teams in the world. These tournaments also pose a different challenge as along with the extra pressure, you are facing against teams you haven't played all year.

<img src="https://github.com/kaneiscoding/DATA-605-Final-Project/blob/main/Graphics/Q2%20Annotated.png"  alt="Question 2" width="900">

The above visualization shows the top 20 teams in terms of international tournament win percentage. Gold teams have won an international tournament while the blue teams have not. We see a concentration of gold at the top with a few more gold teams scattered throughout. The most interesting thing is that the top 14 teams in the graph are from either China or Korea. These regions are condisered the best in the world and have historically dominated international tournmanets.

<br>

## Question 3: Who has been the best in their respective role?

Now that we have analyzed the teams, let's take a closer look at the players. As mentioned before, there are 5 different roles in League of Legends, so it's important to compared apples to apples. Let's see who has been the most successful in terms of winning in each role.

<img src="https://github.com/kaneiscoding/DATA-605-Final-Project/blob/main/Graphics/Q3%20P1%20Annotated.png"  alt="Question 3a" width="900">

Top: We see that Zeus has the best win percentage by a significant margin. Also interstingly 4 of the top 5 players are Chinese, with only Khan being from Korea.

Support: Wolf from Korea tops the support role with a fellow Canadian, Vulcan, coming in at 5th!

Midlane: The Koreans dominate the midlane role with 5 out of the top 5 being from the region. Faker who is at the top, is often considered by fans to the best player in history with 3 world championships.

Jungle: Once again we see domination from the Asian regions in the jungle role with Oner topping the list with a signicant margin.

Bottom: In the bottom role we see 3 world champions top the list with 2 North Americans (and my personal favorite player, Sneaky) following behind.

However, maybe looking just at win percentage doesn't tell the whole story. Perhaps their are some talented players who are stuck on lower tier teams that don't win as much. A good metric to see how impactful you are during a game is how much damage you have inflicted to the enemy. That is what the below visualization captures. Note that the support role is excluded as their role is not focused around doing damage.

<img src="https://github.com/kaneiscoding/DATA-605-Final-Project/blob/main/Graphics/Q3%20P2%20Annotated.png"  alt="Question 3b" width="900">

We see a player, TheShy show up at the top of the top laner role who was not present in the win percentage graph. Not only are they at the top, but they eclipse everyone else by a large margin which is very impressive when compared to the other positions where the damage / min. numbers are much closer between players.

<br>

## Question 4: What are the most important factors in winning a game?

Next, let's see how some game metrics differ between the losing team and the winning team. It's important to understand two concepts XP and gold. XP is used to level up your character which makes them stronger as the game goes on. It is aquire by killing monsters in the jungle and the enemy characters. Gold is used to by items for your character which also increases their power; it is aquired in the same way as XP but all players also earn a constant amount of gold passively.

Now that we understand XP and gold, we can analyze the following visualization:

<img src="https://github.com/kaneiscoding/DATA-605-Final-Project/blob/main/Graphics/Q4%20Annotated.png"  alt="Question 4" width="900">

We see that the winning team does 418 more damage to the enemy on average compared to the losing team. This makes sense because as a team begins to pull ahead, they will have more gold and XP and therefore be stronger. 

The intersting metrics are XP and gold at 15 minutes into the game. The winning team will be up 1880 XP and 2812 gold on average 15 minutes into the game. It's important to know that the teams themselves are not aware of these metrics while they are playing the game, but a viewer would be. 

<br>

## Question 5: What Champions Have Been the Best Throughout the Years?

One aspect of the game we have not touched yet is the champions. These are the characters that the players choose at the beginning of the game. Each have their own traits and abilities and this is where a lot of the strategy related to League of Legends comes in to play, creating "metas" within the game. What champions have been the most successful in competitive play?

<img src="https://github.com/kaneiscoding/DATA-605-Final-Project/blob/main/Graphics/Q5%20P1%20Annotated.png"  alt="Question 5a" width="900">

We see the best champions having between a 70-75% win rate with one support chamption, Braum, having an impressive 78% win rate.

Sometimes the most successful champions are not the most popular though. That's because before the game, each team can ban 5 champions that cannot be played during the game. The strategy is to ban the most powerful champions, the champions they believe the other team is best at, or champions they do not want to play against. 

<img src="https://github.com/kaneiscoding/DATA-605-Final-Project/blob/main/Graphics/Q5%20P2%20Annotated.png"  alt="Question 5b" width="900">

We see different champions appear at the top of pick percentage for each role. There are large difference in the top of the middle, jungle and bottom roles with Azir being picked about 9% of games for midlane, Lee Sin being picked 7% of games for jungle and Ezreal being picked about 9% in bottom lane.

<br>

## Final Thoughts 

One type of data I would have loved to analyze is player contracts/salary. Unlike traditional sports, these contracts are not publicly known for most players. It would be interesting to see if the most successful teams spend significantly more than the lower tier teams. Currently in League of Legends eSports there is no salary cap, so teams can spend as much as they can/want.

When discussing the classic questions such as "what is the best team?" and "who is the best player?" there often isn't one obvious answer. Especially in the realm of League of Legends eSports where teams compete against their native region for most of the year and then compete against the rest of the teams internationally. However, I think the visualizations used to answer the guiding questions give a good idea of who is at the top of the sport. 

<br>

## Refrences

-Mobafire (November 18, 2021). Understanding League of Legends. Obtained from Mobafire: https://www.mobafire.com/league-of-legends/build/understanding-league-of-legends-beginners-guide-600269

-Sevenhuysen, T. (2023). Esports Match Data. Obtained from Oracles Elixir: https://oracleselixir.com/

<br>
