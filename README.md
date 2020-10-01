# NFL-Score-Predicter

For this project we will be looking at prediciting NFL Scores based on a database given to us. The database is from fivethirtyeight and can be accessed here https://github.com/fivethirtyeight/nfl-elo-game. This database contains the date a game was played, the season, the elo rating for both teams, the elo probability, the team tags, whether it was a playoff game, whether it was played at a nuetral area or not, the scores of the games and the results. I think it would be useful to have the average points allowed and points scored for each team, but the average should be a rolling average from the more recent games. Since the goal is to predict future games, the scores and results will not be included in the training data since this will not be given for any games that haven't been played yet. However, I think it could be useful to train a classifier to predict the winner before hand and then have that prediction be used to train the regression model that predicts the scores of each game.

To get predictions on a game just call getPredicitons(filename) where filename is the name of the dataset to be used. This will return a dataframe containing all the predictions. to see the predictions call the printWinners(dataset) where dataset is the dataframe with predictions in it.
