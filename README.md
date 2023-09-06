# FM22_Hungerford_TableauPublic_trial

https://public.tableau.com/shared/XGM3P99QC?:display_count=n&:origin=viz_share_link

The FM22 Tableau Public trial was an experiment using a large dataset from the computer game Football Manager 22. Simply, the game is a simulator, where to take control of a club football (soccer) team, and build a team of individuals capable of winning in both the short and long term. The game rates player skills on a scale of 1-20, and also tracks player performance metrics, among many other things. This data is used to inform player and team decisions and easily accessed in game.

https://youtu.be/yqIXVjCdYks?si=ZMS_mLTPbFU3NHmu

With help from several other players, popular youtube personality and FM streamer, Zealand (Zealand Shannon), published a video that demonstrated how individuals could extract in-game data into a large Excel file. Using this file players could sort player performance data and identify the best performing players. This style of game play was dubbed "Moneyball" saves, after the popular Brad Pitt film, and Michael Lewis book. 

After realizing that this type of game style utilized Mircosoft Excel, it became clear that one could save the Excel workbook as a "CSV UTF-8" file and be properly cleaned using Python. To create a more organized data cleaning process, Jupyter Notebooks were utilized. Once the data was effectively cleaned, the ultimate goal was to open the cleaned data file in Tableau to create a number of visualizations that could animate the in-game player performance data.

Some notes about the cleaned data:
  - Height and Weight were changed from english to metric units of measurements. (The change makes the data more aligned with how the larger world measures player physical traits, and easier to clean.)
  - Most punctuation had to be eliminated from idividual columns in order to change data types.
  - Most numeric data types were changed from object to float.
  - The data set only includes player performance data from 3 leagues. This is because performance and player data is based on the scouting range that is available to your team in game.
  - The data only represents the current season performance up until that point. I.E. to get a data set that is representative of the entire season you would have to play through the entire season, first.

Observations based of Tableau Visualizations:
  - Goal scoring performance is most correlated to the amount of shots a team takes.
  - Height is better indicator of aerial performance than weight.
  - Defensive performance is more closely correlated with clearances and interceptions, but that fewer defensive actions correlate to fewer goals conceded. This means that the more a team retains possesion of the ball, the less likely they are to concede goals.
  - GK performance is more closely correlated to a ratio of conceded goals vs starts. There is not correlation between GK performance and individual GK performance metrics.
