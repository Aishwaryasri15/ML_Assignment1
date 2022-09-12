# ML_Assignment1
Q1 (Reproduce): Please read, understand, run the code and reproduce the model accuracies. 
Please briefly explain whether you can reproduce the classification accuracies of ‘Support 
Vector Machines', 'KNN', 'Logistic Regression’, ‘Random Forest', 'Naive Bayes', 'Perceptron', 
'Stochastic Gradient Decent', 'Linear SVC', 'Decision Tree'. (10 points)

A: Yes, I can reproduce the classification accuracies of all the above-mentioned models with the Kaggle problem set. The accuracies of the models are as mentioned below,

			Support Vector Machines	: 78.23 % accuracy
			KNN				: 83.84 % accuracy
			Logistic Regression		: 80.36 % accuracy
			Random Forest		: 86.76 % accuracy
			Naïve Bayes			: 72.28% accuracy
			Perceptron			: 78.34% accuracy
			Stochastic Gradient Decent	: 77.10% accuracy
			Linear SVC			: 79.01% accuracy
			Decision Tree			: 86.76% accuracy	

Some of the models were producing different results compared to the Kaggle problem set. Out of all the models, Random Forest and the Decision Tree models have produced the highest accuracies of the 86.76%. This means if we are giving an input data of the passenger in the Titanic ship, these models will produce the result with the 86.76% accuracy whether the passenger is going to survive or not. And the Naïve Bayes is the model that produces the lease accuracy of 72.28%.








 
Q2 (Improve): Is the data preprocessing process proposed in the Kaggle post the best preprocessing solution? If yes, please explain why. If not, can you leverage what you learned in the class and your previous experiences to improve data processing, to obtain better accuracies for all these classification models? Describe what is your improved data preprocessing, and what are your improved accuracies?  (16 points)  


No, the dataset proposed in the Kaggle doesn’t produce the best preprocessing solution. The best preprocessing solution can be provided by removing some of the additional preprocessing steps like removing the columns Age Band, creating new features combining existing features such as Parch and SibSp. These steps increase the multicollinearity between the columns and make the accuracy go down.

The second step for improving the accuracy of the models is to normalize the age column since it has a large impact on the model where small age group people, women are having higher survival rates, and adult men and old age group people are having lesser survival rates.

The accuracies of the model with the above implemented preprocessing techniques are:

Support Vector Machines	: 83.39 % accuracy
			KNN				: 87.54 % accuracy
			Logistic Regression		: 81.26 % accuracy
			Random Forest		: 94.95 % accuracy
			Naïve Bayes			: 80.02 % accuracy
			Perceptron			: 64.31% accuracy
			Stochastic Gradient Decent	: 79.69% accuracy
			Linear SVC			: 81.14% accuracy
	Decision Tree			: 94.95% accuracy
 	 
This means if we are giving input data of the passenger in the Titanic ship, the Decision Tree, and Random Forest models will produce the result with 94.95% accuracy whether the passenger is going to survive or not. And I feel that these models has bit of overfitting as well.
 
![image](https://user-images.githubusercontent.com/53164418/189568205-62fd0883-b775-414c-8580-3eac8f447993.png)
