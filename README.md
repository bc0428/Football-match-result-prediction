# Football-match-result-prediction

feature engineering.ipynb: <br>data preprocessing <br><br>
match results prediction.ipynb: <br>dimension reduction, model building and evaluation, model performance visualisation 
<br><br>

<h2>Football match result prediction using betting odds only</h2>
<br>data retrieved from (https://www.football-data.co.uk)<br><br>

Raw data consists of betting odds of Home, Draw and Away, over and under 2.5 goals. It is then further augmented with probability and odds for match result, i.e. probability and odds of Home/Away win or Draw. Then, principal component analysis were done to reduce dimension, and it explains for over 99% of variance.<br>


Reduced data were experimented with K-Nearest Neighbor classifier, Random forest classifier, Support Vector classifier, XGBoost and logistic regression. For base models, K-Nearest neighbour and ensemble algorithms (random forest / XGboost) perform relatively better on dimension reduced data <br>

Final model is a voting classifier, composed of XGBoost, K-Nearest Neighbor classifier and Logistic regression, which achieved F1 score = 0.816
