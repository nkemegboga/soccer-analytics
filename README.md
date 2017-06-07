# soccer-analytics
This project is aimed at using machine learning algorithms to improve soccer strategies.

## Description:
There's a lot of uncertainty in soccer. The home team wins 46% of the time and the bookmakers are right 53% of the time. However, I believe analyzing games from a tactical perspective will help explain some of these uncertainties. For example in England, recently, West Ham beat Tottenham. Tottenham were 2nd and had lost only 3 games this season, while West Ham were 12th and had lost 17 games this season, so naturally, Tottenham were expected to win. So what happened? If we just look at quality of players and form, any model would have predicted a Tottenham win. However, if in addition to player quality and form, the model includes tactical perspectives such as formations being played, and features that qualify style of passing, style of attack, style of defending etc, I believe we would have had a much better prediction for the game.

This can be helpful to soccer teams as before a game, the model can be run to determine how likely the team is to win, given the way a given opponent plays on average. The team can then change parts of their tactics until the model predicts a high chance of winning.

Additionally, given historical betting odds data, a threshold that maximizes returns on bets from the model's predictions will be determined.

## Problem being solved:
Uncertainty in soccer; tactical setups in soccer, given a specific opponent.

## Data that will be used:
Data that quantifies/qualifies the home and away team's style of attack.

Style of attack: long ball %, short pass %, through ball %, crosses sent in %, average pass streak, % pass success, number of passes, possession %, % shots in 6 yard box, % of shots in 18 yard box, % of shots from outside the box, shots per game, % of chances from counter attacks, # of successful dribbles, % of attacks through the middle

Style of defending: % aerial duels won, # of successful tackles, # of interceptions, # of clearances, average position of defensive line

General stats: Formation, league, average player rating before game

Target: (Home score - away score)

## Presentation:
Slides with results of tactical analysis

Web app that allows users put in 2 teams before a game and predicts the likely outcome and determines if it's a good bet given the odds on the game.

## Data sources:
Web scrape data from whoscored.com on 15,000 games across the English, Spanish, French, German and Italian leagues from the 2009/2010 season to today.

## Next step:
I have populated my database with 15,000 games.
 
Fit and tuned an XG Boost model with test set accuracy of 68%
 
Clustered data to define 12 different game strategies
 
Working on analysis and developing web app
