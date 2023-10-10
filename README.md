# PARKINSON_DISEASE_PREDICTION
Pakinson Disease Classificaton model.

AIM: Parkinsons Disease Prediction.

Data Set Characteristics: Multivariate

Number of Instances: 197

Area: Life

Attribute Characteristics: Real

Number of Attributes: 23

Associated Tasks: Classification

Missing Values? N/A

Attribute Information:

Matrix column entries (attributes):

name - ASCII subject name and recording number

MDVP:Fo(Hz) - Average vocal fundamental frequency

MDVP:Fhi(Hz) - Maximum vocal fundamental frequency

MDVP:Flo(Hz) - Minimum vocal fundamental frequency

MDVP:Jitter(%),MDVP:Jitter(Abs),MDVP:RAP,MDVP:PPQ,Jitter:DDP - Several 

measures of variation in fundamental frequency

MDVP:Shimmer,MDVP:Shimmer(dB),Shimmer:APQ3,Shimmer:APQ5,MDVP:APQ,Shimmer:DDA - Several measures of variation in amplitude

NHR,HNR - Two measures of ratio of noise to tonal components in the voice

status - Health status of the subject (one) - Parkinson's, (zero) - healthy

RPDE,D2 - Two nonlinear dynamical complexity measures

DFA - Signal fractal scaling exponent

spread1,spread2,PPE - Three nonlinear measures of fundamental frequency variation 

EVALUATION:
We find that LogisticRegression, SupportVectorMachine, DecisionTree algorithms show an accuracy score of around 86-88%. K-NearestNeighbors algorithm performs really well on the train set with an accuracy of 95%.
Decision-tree and Random Forest overfit the train set so we had to apply cross validation method.RandomForest is the best performing algorithm with an accuracy score of 93% on test data.

Conclusion:
I performed EDA, Data preprocessing steps including finding out the counts of each status type, numerical description of features, standardiztion of input variable after splitting the features on the basis of input and output variables. Status is most correlated to the PPE feature. We split the train and test data where 30% of the data was kept for testing. While performing Machine Learning we found that Decision Tree and Random Forest algorithms were overfitting the train dataset so we appliied cross validation on both. We found that RandomForestClassifier was the best performing model with test accuracy of 93% and overall accuracy of 97%.



