# mushroom_classification

# Capstone 2: Supervised Learning
### Mushroom Classification Model
Dataset: Mushroom records drawn from The Audubon Society Field Guide to North American Mushrooms (1981).

## Dataset & Research Question

This dataset includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family. Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. The Guide clearly states that there is no simple rule for determining the edibility of a mushroom; no rule like "leaflets three, let it be'' for Poisonous Oak and Ivy.

From this dataset we aim to determine the following:
Can mushroom samples be correctly identified as edible or poisonous based on a set of physical attributes?


## Model Specification & Results

For this analysis, five classification models were fit to the data. K-fold cross validation was used to assess the accuracy of each model. For the random forest and KNN classifiers, hyperparameter tuning was done to determine the optimal number of estimators and neighbors, respectively. The models compared for this analysis and their respective accuracies can be found below: 

![](https://github.com/jdscott782/mushroom_classification/blob/main/model%20accuracy%20results.png)


## Practical Uses & Considerations

For our purposes, the best model was the random forest classifier with an accuracy of 95.8%. Ultimately the top factor in selecting the best model was accuracy, since misidentifying a poisonous mushroom could be a fatal error.

* This model could be used by mushroom collectors to determine whether the mushrooms they encounter in the field are edible or poisonous. 
* This can mean the difference between survival and death in certain instances, so it is important that the model has the highest possible accuracy. 
* Since the model would likely not be usable out in the field, it would be less useful to survivalists and more useful for individuals collecting the mushrooms and later determining whether or not they are edible. That is, unless a portable application of the model could be created to test samples in the field.


## Weak Points & Further Analysis

This model does not have 100% accuracy so it is not a foolproof method to determine whether or not a collected mushroom is edible. Further hyperparameter tuning could be done to improve the accuracy closer to 100%, but that is beyond the scope of this analysis. For the purposes of our analysis, an accuracy of 95.8% is acceptable.

Additionally, we included all 22 categorical variables as features in the model. Further analysis could be done to determine which features could be dropped without sacrificing accuracy, in order to improve the performance of the model.

