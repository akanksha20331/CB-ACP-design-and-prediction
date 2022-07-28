Project OOPD CB: ACP design and prediction

Name:- Aman Srivastava (MT20333) Akanksha jarwal (MT20331) Amaithi Priya
Himanshi Garg

Problem Statement:- To implement different machine learning algorithms
to predict anticancer peptides.

Libraries used:- 1. Numpy. 2. Pandas. 3. MatPlotLib.pyplot 4. sklearn 5.
keras 6. Tensorflow. 7. Seaborn 8. MYSQL.

Classes:- 1:-DB\_Conn 2:-DB\_Manager 3:-Data\_Preprocessor
4:-DecisionTreeClassifierModel 5:-RandomForestModel. 6:- Conf\_metrix.
7:- DB\_Load

Database Used:- MYSQL local Database.

Input Files :- FASTA format.

Step1:- Creating a Server Connection.

Step2:- Creating a Database.

Step 3:- Creating Connection to the Database.

Step 4:- Creating a Table in the SQL Database.

Step 5:- Pre processing our Data, both positive datasets and negative
datasets and loading it in the Table.

Step 6:- Retrieving the data from the Database in the form of a
Database.

Step 7:- Performed p-Feature analysis on our Data and preprocessing
using Standard Scaler.

Step 8:- Performed feature Selection using Variance Threshold.

Step 9 :- Split the Dataset using train\_test\_split in training set=
70% and testing set = 30%

Step 10:- Prepared Decision Tree Classifier model and running data on
it.

Step 11:- Prepared Random Forest model and running data on it.

Step 12:- Calculated Accuracy and F1 score of Output.

Step 13:- Plotted the Confusion Matrix and also plotting the ROC curve.

Step 14:- Built class Confusion Metrices and calculated values of
Sensitivity, Specificity etc.

Step 15:- Saving the results to the Database in Table named Results.

Model:-

Model 1:- Decision Tree Classifier with Random State set to 15.

Model.fit is then done to fit the model using the X\_train and Y\_train
values. The accuracy and F1-Score are below:-

Accuracy of Decision Tree: 0.674074074074074 f1\_score of Decision Tree:
0.6986301369863014

Model 2:- Random Forest Model:

Random forest model is built in which the random state is set to 18 with
max\_depth=2,max\_features='auto'and n\_estimators=3.

Model.fit is then done to fit the model using the X\_train and Y\_train
values. The accuracy and F1-Score are below:-

Accuracy of Random Forest: 0.7851851851851852 f1\_score of Random
Forest: 0.6986301369863014.

Plotting:- Plotting a Confusion Matrix of Our result.

Confusion matrix \[\[52 20\]. \[ 9 54\]\]

Also Calculated the AUC score using the FPR and TPR values: AUC:-
0.8656305114638447.

Plotted the ROC curve and also calculated the scores: Below they are
mentioned:-

True Positives: 54 True Negatives: 52 False Positives: 20 False
Negatives: 9 --------------------------------------------------
Accuracy: 0.79 Mis-Classification: 0.21 Sensitivity: 0.86 Specificity:
0.72 Precision: 0.72 f\_1 Score: 0.78

Finally saved the values to the Database after processing and used
DB\_Load class to load the classes to the Database.

Thanks
