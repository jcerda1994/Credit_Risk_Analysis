Overview of the analysis: Explain the purpose of this analysis.
-The purpose of this analysis is to show the supervised machine learning models in order to compare between them and make a better decision of which to use, first of all i made extraction, transforming and loading of a database in order to make the ML models.


Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.
overampling: 
acurcay: 0.6547385707934685
precision (TP/(TP+FP): .01
recall (TP/(TP+FN) : .72

SMOTE oversampling:
acurcay: 0.66201409663885
precision (TP/(TP+FP): .01
recall (TP/(TP+FN) : .63

Undersampling:
acurcay: 0.5447339051023905
precision (TP/(TP+FP): .01
recall (TP/(TP+FN) : .69

Combination:
acurcay: 0.6400726134353378
precision (TP/(TP+FP): .01
recall (TP/(TP+FN) : .69


Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
In this challenge, i used many techniques to demonstrate the efficiency of each model, first of all the ETL is neccesary for getting a clean database, then i split the data into taining and testing defining each variable (X,y), as we can see i started with oversampling the data, that means duplicating data of the minority class, then i used SMOTE or synthetic oversampling, that means selecting examples that are close in feature space and then selecting a k nearest neighbor randomly to create a new set of data, finallly i used the smoteenn method which combines the two methods by choosing data from the minoirty class, calculate the distance bewtween the data and its k-nearest and then multiply the difference with a random number bewteen 0 and 1 and then adding that result to the minority class. After all the imbalance data is solved i proceed to generating a logistic regression in order to predict the model, making the decision to recommend the SMOTE oversampling due to the accuracy score.





