[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/7lKBcjfN)
# 44-566 machine-learning project
Repo for all project documents

After doing the model on Decision tree classifier and SVM, compared to the linear regression model my dataset does overall better looking at the metrics value such as the R-squared value and the root mean squared error. In the previous milestone the linear regression model score for the r-squared was 0.00030304875264952624 which indicated the model is not effectively explaining the variability in the data and is likely not a good fit for the given dataset.

Whereas in the decision tree classifier the r-squared value for the training set and testing set was 0.894 and 0.312 respectively which means the decision tree classifier model does overall better compared to the Linear regression model. However looking at the r-squared value for training and testing set for decision tree classifier we can see the huge gap in the value of r-squared which suggests that the model looks to be overfitting

The SVM model in the training set and testing set had a R-squared value of 0.37 and 0.336 respectively which overall again does better than the Linear regression model.

If comparing the SVM and decision tree classifier, the decision tree classifier does better than the SVM model in the testing set whereas in the training set the SVM does better than the decision tree classfier. But overall SVM model is better as it's metrics are more consistent compared to that of decision tree classifier.