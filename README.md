# car_insurance_prediction

This report is about predicting "ISBOUND" for car insurance, which means the person who asked for the car insurance quote took out the insurance policy. To predict the prices two data sets were used, one is Cooperators_Quotes_Dataset_Training.xlsx and another one is Cooperators_Quotes_Dataset_Testing.xlsx.

Imagine you have a dataset of car insurance policy information such as car model, maker, driver name, occupation, ownership type, etc., and you want to predict if the person can get insurance for their car. The goal is to build a model that makes accurate predictions considering the core features as the maximum potential of information.

Here's what the code does:

It starts by loading the insurance policy information data and finding the major features undergoing different steps of data pre-processing such as finding columns that have missing values and replacing those applying mean and mode methods, mapping mismatched vehicle data, mapping qualitative categorical data to numerical data, etc.

Then, it splits the data into two parts: the "training" set and the "validation" set. The training set teaches the model how to make predictions, and the validation set is used to check how well the model is doing.

In this code, two different methods were used for predicting the outcome. One is the Naive Bayes method and another is the Logistic Regression.

It trains the model using the training data, so the model learns from the features of the insurance data and their actual "ISBOUND" values.

After training, the model makes predictions on the validation set and calculates how accurate those predictions are. For both methods Receiver operating characteristic Curve (ROC) and Area under the ROC Curve (AUC) were calculated and plotted in the graph.

Finally, the roc curve for both Logistic Regression and the Naive Bayes method were compared to check the better result.

Final Result:

Naive Bayes:
AUC = 0.5024
Accuracy = 78%

Logistic Regression:
AUC = 0.50
Accuracy = 78%

 
