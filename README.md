# AmazonReview_Text_Classification

### Introduction

The introduction of anonymity has led to increase in number of reviews but on the other hand the quality of reviews has gone down on the interent forums. Different websites have tried different methods for extracting more useful comments. Amazon came up with their own helpfulness rating system.

### Problem:

But still poor quality comments seem to be at the top of their review forms.The reason for the failure is that the part of the algorithm that determines the order of reviews relies on how recently the review was posted.

For example the following review was at the top of an app called “Friday Night at Freddies 4”

“I love this game so much but at first I though it was lame but when I go in the game I can't beat the first night because cause I put it to full volume and I can't here the breathing bonnie strike at 4 am Chica at 5 and plus it not lame it's better than fnaf and fnaf 2 plus get this game when u buy fnaf”

This comment, despite being at the top of the forum, is difficult to understand, a run on sentence, and full of spelling errors. The offending review was the most recent, but it’s helpfulness score was far less than previous reviews. This illustrates the difficult balance that must be struck between showing the highest rated reviews, and showing the newest reviews, to be rated by the community.

### Solution:

Use machine learning techniques to design a system that “pre-rates” new reviews on their “helpfulness” before they are given a position at the top of the forum. The proposed system will use a set of Amazon review data to train itself to predict a helpfulness classification (helpful, or not helpful) for new input data.

### Conclusion:
##### Amazon Point of View

This would help amazon put new reviews on the top if they are helpful which would enhance customer experience

##### Text Classification
Tried to find a link between ratings and helpful reviews, but since the correlation was low, we realized that Text classification would be needed to classify reviews as helpful or not.

Gathered a better understanding of the classic problem in NLP, text classification, and learned about important concepts like feature engineering(TF-IDF Vector, Count Vectors).

Understood that accuracy is not a good measure when data is imbalanced and utilized AUC-ROC Curve as a performance measure to select models

Selected Logistic regression (TF-IDF-Word Level) since it had the highest AUC score.
