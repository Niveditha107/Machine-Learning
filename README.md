# Machine-Learning
Telco Customer churn analysis using various ML Algorithms
Customer churn in the telecom industry describes a situation where a customer stops the services of one telecom company during the contract and switches to a competitor to obtain a better cheaper and mores satisfactory service for customer’s needs.Acquiring new customers was the important strategy for increasing revenue quickly at early stage but when telecom industry become saturated it’s focus shifted to the prevention of customer churn.
Artificial intelligence means replicating human intellectual processes through machines, especially computers.Machine learning is a subset of Artificial intelligence that provide system the ability to automatically learn and improve from experience without being explicitly programmed.Machine learning(ML) explores the study and construction of algorithms that can learn from data and make predictions on data.Based on more data, machine learning can change actions and responses which will make it more efficient and adaptable.
After reading the research articles it is finalised that the main methods or algorithms used in this project are Logistic regression , Decision tree, Random Forest, Support vector machine and few of the ensembling methods.Here by analysing the details of the customers provided by the telecom company it is to be founded that whether a new customer will churn or not and therefore every algorithms used in this project are of classification type where the target variable is categorical.That is the output have value ”YES” or ”NO”.
Logistic regression is one of the most simple and commonly used machine learning algorithms for 2 class classification.It is a statistical method to predict binary classes.Just like linear regression assumes that the data follows a linear function, in logistic regression models the data follows the sigmoid function. Output of the linear regression is discrete while output of the logistic regression is continuous.The sigmoid function also called logistic function gives an ’S’shaped curve that can take any real valued number and map it into a value between 0 and 1.
Decision Tree is a tree shaped diagram used to determine a course of action.Each branch of a tree represents a possible decision, occurrence or reaction. As it’s name suggest, it is an algorithm that has shaped like tree which helps to make certain decision by monitoring the different attributes provided.Decision tree can be used both in classification and regression problem.In classification a classified tree will determine a set of logical ”if-then” conditions to classify problems.For example discriminating between 3 types of flowers based on cer- tain features.A regression tree is used when the target variable is numerical or continuous in nature.We fit a regression model to the target variable using each of the independent variables. each split is made based on the sum of squared error.Since the decision tree does not make any assumptions about data it is also known as CART(classification and regression tree).
Random forest is an ensemble machine learning algorithm.It operates by building multiple decision tree’s.The decision of the majority of the tree is chosen by the random forest as the final decision.Decision trees are highly sensitive to the training data which could result in high variance.Random forest or Random decision forest operates by considering multiple decision trees during the training phase.Random forest work for both classification and regression problems.Regression problems have continuous or numerical valued output variable.More the no:of trees in random forest, more will be the accuracy of the prediction.
Support vector machine or SVM is one of the supervised machine learning algorithm which is used for both classification and regression.The aim of SVM is to fix a decision boundary which make an n-dimensional data into classes so that a new data point can be correctly classified.This best decision boundary is known as a hyperplane.To create a hyperplane we need to choose extreme points or vectors.For which SVM is used. SVM algorithm can be used for face detection image classification text categorization etc.
For this analysis data of a telecom company had been from kaggle website.The raw data has 7043 rows and 21 columns.Each row in the data represent a customer and each column contains customer attributes.Here the last column named ”Churn” is the target variable or the dependent variable for our model.
Before going directly to the analysis some pre-processing techniques has been done in R.Summary of this data gives the Maximum,Minimum,Mean,Median,First quartile and Third quartile of the numeric type data.In this data Tenure, Monthly charges and Total charges are the only 3 attribute which is of numeric type.And their summary is given below.
After completing the cleaning of the data we go on to the feature selection part.For selecting the features 2 algorithms Principal component analysis and boruta algorithm is used. PCA is used as a feature selection method .But since the correlation between the attributes are very less we reach in a conclusion that we need to take 17 attributes among the 20 to make the principal component a good representative of the attributes.So PCA is not a suitable feature selection method for this data.By Boruta algorithm it is found that the attribute gender is an unimportant attribute to the analysis and thus we eliminate the ”gender” from the data.
It is crucial to observe the historical behavioural patterns of customers for the churn prediction in telecom sector.This study evaluated the capability of the SVM as a base classifier for some particular data.Initially every analysis should be conducted after feature selection.It is not necessary to select every feature for the analysis.Every feature have an importance in building the model and predicting the future.The feature importance of each attribute in the data is given below.
