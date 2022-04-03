# Intersteller-Titanic-Analysis
New Interstellar Titanic competition on Kaggle to predict whether the passenger will be transported in another dimension or not. 

There were several steps followed before just using a Machine Learning algorithm to predict whether the passenger will be transported or not successfully. The following steps were taken in completion of the analysis:

File1: Intersteller_Titanic_Kaggle.ipynb:

1. Importing necessary Libraries.
2. Loading the competition train dataset.
3. Dealing with missing values.
4. Exploratory Data Analysis.
5. Encoding the Categorical columns.
6. Scaling the continuous columns.
7. Splitting the dataset.
8. Training the base model to compare with (Logistic Regression) using GridSearch CV parameters.
9. Using SVM Classifier, Naive Bayes, Random Forest with GridSearch CV parameters for their best performance.
10. Using metrics such as Confusion Matrix, Classification Report, ROC curves for comparing the performances. 
11. Preprocessing the competition test set and using best model(Logistic Regression) to predict whether passenger will be transported or not. This resulted in 0.77 score over Kaggle. 

To improve this, I used different approaches in a separate file: Part2.ipynb:
1. Importing Libraries.
2. Loading the competition train dataset. 
3. Creating functions for each pre-processing step (Used different approach then previous one). 
4. Pre-processing the dataset. 
5. Splitting the dataset. 
6. Using Logistic Regression with GridSearch CV best parameters as a base model. 
7. Used another algorithm Random Forest with GridSearch CV best parameters as a model to compare with the base model. 
8. Using appropriate metric to compare the models. (Classification Report, Confusion Matrix).
9. This time Random Forest performed better then Logistic Regression so used that trained model to predict the competition test dataset Transported values which resulted in a better score of 0.7877.
10. On further improving the data pre-processing, Random Forest again did better which was used to predict the competition test dataset Transported values which resulted in the best score till now of 0.79003.
