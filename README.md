# mushroom_classification
Mushroom classification model

## Dataset & research question

This dataset includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family. Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. The Guide clearly states that there is no simple rule for determining the edibility of a mushroom; no rule like "leaflets three, let it be'' for Poisonous Oak and Ivy.

From this dataset we aim to determine the following:
Can mushroom samples be correctly identified as edible or poisonous based on a set of physical attributes?


## Model specification & results

For this analysis, five classification models were fit to the data. K-fold cross validation was used to assess the accuracy of each model. For the random forest and KNN classifiers, hyperparameter tuning was done to determine the optimal number of estimators and neighbors, respectively. The models compared for this analysis and their respective accuracies can be found below: 

!(https://github.com/jdscott782/mushroom_classification/blob/main/model%20accuracy%20results.png)
