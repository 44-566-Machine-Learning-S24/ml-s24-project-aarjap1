[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/7lKBcjfN)
# 44-566 machine-learning project
Repo for all project documents

Please find the README_Final Project if you are looking for the final project submission with links to raw_data, data, analysis and conclusion.

README ( This read me was to keep track of milestones. The Final Project readme is in the notebook README_Final Project.ipynb )

My project is a classification problem which predicts the parental level of education on 4 categories Bachelor's degree, Master's degree and associate's degree using features such as race, gender and student's score. My initial goal at the beginning was to predict the Parental level of education using other features present in the dataset which I sticked with throughout the project because I thought the co-relation between the features in the dataset would be interesting.

I acquired my dataset from kaggle. I went through multiple datasets but choose to go with this one because I thought it would interesting and fun to predict Parental Level of education by looking through features such as Student's grade in different exams, their gender and race as well. The name of my dataset is "Student Performance In Exams". 
KAGGLE DATASET LINK : https://www.kaggle.com/code/spscientist/student-performance-in-exams/input

Initial exploration link : http://localhost:8890/lab/tree/Machine%20Learning%20Repos/ml-s24-project-aarjap1/initial_exploration.ipynb
For my intial exploration my target was to predict the parental level of education using the scores provided in the dataset which consisted of reading, writing and math score. Instead of using reading, writing and math score individually I thought I would use a new feature called Total Score which would combine the three score to predict parental level of education. Since the parental level of education was a non-numeric type I convert the feature to a numeric type with a mapping "bachelor's degree": 1, 'some college': 2, "master's degree": 3, and "associate's degree": 4.

After getting to milestone 1 I have also introduced two new features gender and race which also non-numeric type which I have converted to numerical type as well. I introduced them since I though it would help predict the parental level of education better.

New features included starting classification modeling (SVM and Decision Tree classifier can found on this link): http://localhost:8890/lab/tree/Machine%20Learning%20Repos/ml-s24-project-aarjap1/classification.ipynb

After doing the model on Decision tree classifier and SVM, compared to the linear regression model my dataset does overall better looking at the metrics value such as the R-squared value and the root mean squared error. In the previous milestone the linear regression model score for the r-squared was 0.00030304875264952624 which indicated the model is not effectively explaining the variability in the data and is likely not a good fit for the given dataset. Hence I learned my dataset which is a classification problem does not do to well in Linear regression model. Since it is a classification problem it should better in a classification model

In the decision tree classifier training accuracy and precison I got was 0.89 and 0.90 which suggested my model did really good. But in the test set the model performed poorly with acccuray and precision of only 0.28 and 0.32 respectively. So looking at the metrics value for training and testing set for decision tree classifier we can see the huge gap in the value of metrics which suggests that the model looks to be overfitting. Hence I learned my dataset has a overfitting problem due to the huge gap in metrics score between training and testing set.

The SVM model in the training set had accuracy and precison of 0.37 and 0.54 respectively and in testing set had accuracy and precison of 0.34 and 0.49 respectively which overall again does better than the Linear regression model and Decision tree classifier since the decision tree model was overfitting by a lot. Even though SVM model did not do to well it still performed better than the Linear regression and Decision tree model in perdiciting the Parental Level of education. But overall none of the model was able to accurately predict the parental level of education so far.

In conclusion comparing the SVM and decision tree classifier, the decision tree classifier does better than the SVM model in the testing set whereas in the training set the SVM does better than the decision tree classfier. But overall SVM model is better as it's metrics are more consistent compared to that of decision tree classifier.

I have did the Linear kernel classifier which does overall well with training accuracy and precision value of 0.404 and 0.28 in training set and in testing set with accuracy and precision of 0.312 and 0.24 respectively but compared to SVM RBF classifier the SVM RBF is still prefered as it is more consistent with it's accuracy and precision accross both the training and testing set.

Coming to milestone 3, I applied dimension reduction to my dataset and did the Random Forest classifier model. The model had an weighted average for the all the performance metrics(precision, recall, f1-score) we got was 0.87 which was extremely well. With neural nets model also my dataset did really well. Almost to well with 100% accuracy across all performance metrics which are precision, recall and f1-score. There is a high possibility of overfitting looking at the confusion matrix. Hence I learned my dataset classification problem does really well on Random Forest and also on neural nets but with a sign of overfitting.

After doing the classification modeling I learned that my dataset did overall very well in SVM, SVM linear kernel, Random Forest and Decision tree model as my dataset is a classification problem compared to regression models. Even though the classification models were not able to accurately predict the parental level of education I felt like it was more of a dataset problem of not having enough features. The features I used to predict parental level of education were Total students score, Gender and Race. I felt like the Gender and Race were not much of help in predicting the parental level of education. And the other features in the dataset were not much of help either which I could use because the features were Lunch which wouldn't be of a much help in predicting the parental level of education so I left those features out.

If I were to have more features I would ask the person who made the dataset to add features like Parent's job, Student's previous semster GPA's, study hours and so on which could play a huge factor in prediciting the outcome.

Overall, my main findings were that the best model was the SVM and Random Forest classifier model for my classification dataset to predict Parental level of education using the three features race, gender and student's score. 
SVM Link : http://localhost:8890/lab/tree/Machine%20Learning%20Repos/ml-s24-project-aarjap1/classification.ipynb
Random forest Link : http://localhost:8890/lab/tree/Machine%20Learning%20Repos/ml-s24-project-aarjap1/milestone_3.ipynb

My conclusion to why my dataset did not do extremely well in most of the models is because I feel like the features provided in the dataset is not extremely helpful in predicting parental level of education. Like the features Lunch, Gender and Race in my thinking is not very well co-related to predicting the Parental Level of Education. I mentioned in my analysis if we had features like the Parental's job, Student's previous semester GPA's etc could maybe have provided more insight or be more helpful in predicting Parental Level Of Education which would help the model do better.