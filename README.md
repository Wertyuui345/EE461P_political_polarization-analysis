# EE461P_political_polarization-analysis
An attempt to find whether consumption of certain forms of media is a predictor of political views.

# Definitions
We are defining polarization as ideological consistency. In this case, whether Democrats are more consistently liberal and Republicans are consistently conservative
See following article. We use the questions provided as a measure of ideological consistency. https://www.pewresearch.org/politics/2014/06/12/section-1-growing-ideological-consistency/

# Reasoning
Ideally, if our model accurately predicts that, with certain features, the political party more accurately than previous years, then media is definitely a driving force behind views. However, our current model only predicts based on survey data from 2014 and does not take into account the past.

# Steps
Current goal is to isolate columns and see which columns heavily correlate with party. Do certain viewership of media impact political party? By how much? Can we map consumption of certain types of media to certain political parties.

We performed one-hot-encoding on survey data and isolated questions based on trust and distrust of certain sources of media. Additionally, we used heuristics outlined by the Pew Research Center to create a proportional features based on the number of sources trusted and distrusted. We then performed multiple logisitic regression for each prediction and mapped them onto a confusion matrix for visualization. We also determined the most important features needed to predict a survey participant's political party

# Conclusion
In sum, we found that there is an association between trust and distrust in certain media and political party. We found that trust and distrust regarding highly conservative and highly liberal media tend to have a very strong correlation with certain political parties. Furthermore, refusing to answer certain questions also were a strong indicator of political party.
