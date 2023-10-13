# Voting-model
Voting model using (Logistic Regression , Gaussian NB , Random Forest Classifier , K Neighbors Classifier)

this notebook explains how to apply many models on same dataset by using voting models
Loosely speaking that is the main idea of ensemble learning. We train a number of predictors on the same data set, or on smaller data sets that are samples from the same larger data set, and then we combine the predictions of all the predictors in order to choose the most appropriate prediction. There are a number of approaches for implementing this idea. In this tutorial, we focus on voting classifiers.

The idea of the voting classifiers is very simple. We train different classifiers on the same data set. Classifiers can be of completely different types, such as for example support vector machine, logistic regression, decision trees, random forests, etc., classifiers. Also, the classifiers can be of the same type, however, the parameters of the classifiers can be different. For example, we can train a series of decision trees with different parameters. After we train the classifiers, we predict the class label by using the majority vote strategy or the soft voting strategy. In this tutorial, we focus on the majority vote strategy since it is simple and easy-to understand.

Every classifier can predict either the class 1 or the class 2. The majority vote classifier will then select the class 1 because three classifiers predict this class, and two classifiers predict the class 2. That is the basic idea of the majority vote classifier. In the sequel, we explain how to implement the voting classifier in Python. As the result, of our implementation, we will be able to generate the classification results shown below (this graph will be explained in the next section).

for basic code (https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.VotingClassifier.html)
