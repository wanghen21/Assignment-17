# Assignment-17
## Credit Risk Analysis-ML Learning

Credit risk is difficult to determine; most of the financial institutions have established similar modeling methods to determine credit worthiness. 
#Purpose
In this challege, we are investigating the file "loan_stats csv" to predict whether someone is low or high risk status. One of the most common way to determine creditworthiness is creating a model and then evaluate and train the models that they create. We are using imbalanced-learn and scikit-learn libraries to build models and evalute them using a resampling method. In the first couple of models we oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm. In the remaining models we used a combination approach to over and undersample the data using smoteenn. Finally, the two machine learning models were compared to minimize bias, balancedrandomforestclassifier and easyensembleclassifier.

#NaiveBalanced
![NaiveBalanced](https://user-images.githubusercontent.com/80020446/126086235-b6cbe738-2281-4aa8-8e8a-339317c4322d.PNG)
#Smote Oversampling
![Smote](https://user-images.githubusercontent.com/80020446/126086276-7ffaa7fd-8642-4c95-b170-c3160d244073.PNG)
#Under Sampling
![UnderSampling](https://user-images.githubusercontent.com/80020446/126086332-19a180dd-fdf4-4867-8291-51d105a06193.PNG)
#Combined/Over and Under sampling
![CombinedSampling](https://user-images.githubusercontent.com/80020446/126086374-932d263b-2943-403e-9038-a02700787b56.PNG)
#Balanced Random Forester Learner
![BalancedRandomForester](https://user-images.githubusercontent.com/80020446/126086452-74f59084-d433-468c-96c1-de1a1bc968d1.PNG)
#Easy Ensemble Learner
![EasyEnsemble](https://user-images.githubusercontent.com/80020446/126086453-04434429-ef38-4a14-8d6a-a08868adacee.PNG)
#Summary
In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
