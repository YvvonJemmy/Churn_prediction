# CHURN PREDICTIONS
The code predicts churn
# Requirements
- Have python installed 
# Libraries used
- numpy and pandas are used for data manipulation and analysis.
- seaborn and matplotlib.pyplot are used for data visualization.
- train_test_split is used from sklearn.model_selection to split data into training and testing sets.
- KFold is used for model evaluation
- cross_val_score is used to perform cross validation and return the score
- A standerd scaler is used to scale the data
- Models used here are KNearestNeighbor, Decision Tree and Logistic Regression for classification.
- A classification report and confusion matrix were used to show the evaluation of the models.
- train_test_split is again used from sklearn.model_selection to split data into training and testing sets.

# The dataset
The dataset is in the form of one csv file.
# models used
 3 models have been used
- K nearest neighbor model
- Decision Tree model
- logistic regression
# Sanity checks
- sanity checks were performed on the dataset. It was found to have duplicates which were removed
# working on the dataset
The train dataset has 3150 rows and the test dataset has 14 columns
# EDA on the target variable
- EDA was performed on the churn column
- A histogram was drawn and the count of unique values in the column was done
# Model building
The y variable was defined
The train dataset was the divided into the train set and the validation set
The data was scaled using standard scaler
### defining the models
All the three models were defined in one dictionary
A for loop was then created to apply cross validation through the 3 models.
A kfold object with 10 splits was used.
The models were fitted on the train data and tested on the test data.
The results were appended to a list then plotted using boxplots
The best performing model so far was was knearestneighbor(knn)
### Accuracy of the models
The accuracy of the models was calculated:
- The accuracy of the knn model is: 0.9470899470899471
- The accuracy of the  logistic regression model is: 0.8846560846560847
- The accuracy of the decision tree model is: 0.9439153439153439
The knn model has the highest accuracy
### Making predictions on the model
Predictions on the test data were made by all the models.
A confusion matrix and a classification report was generated for all the models.
The logistic regression model had low f1 score and recall score on class 1 of the target variable.

# OVERVIEW
The best performing model was the knn model.





