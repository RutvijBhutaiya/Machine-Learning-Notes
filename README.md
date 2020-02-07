# Machine-Learning-Notes
#### Few notes on basic concepts of Machine Learning. 


1. Ensemble: Ensemble idea is to train multi model using same learning algorithm. Main cause of error are noise, bias and variance. Ensemble minimizes it. And it uses to stabilize the learning model. 

2. Bagging vs. Boosting: (https://quantdare.com/what-is-the-difference-between-bagging-and-boosting/)

- Bagging is also knwn as Bootstrap aggregation. 
- Based on training data set, both techniques create n classifier (random new datasets). 

- Bagging each model build independently. Like for example there are 10 new random datasets. So, the 10 models based on each data would be independent to each other. 

- Boosting each model build in sequence. Means model 1 build based on dataset 1. Then model 2 build based on model 1 (previous classifier success) but uses dataset 2. This minimises the errors from previous models and increases influence of high performing model.

- Hence, in bagging, classifier is an average (regression) or max vote (classification). However, in boosting is based on weightage average. 
- Bagging is train and keep AND boosting is train and evaluate. 
- Boosting uses certain weights to next classification stage e.g. Adaboost, XGBoost.
- Bagging may solve overfitting problem. Boosting can increase overfitting. Because, Boosting gives more weights to good performance and removes bad performers from the model. 

3. ML Principles: (https://towardsdatascience.com/machine-learning-from-first-principles-51a5e75a3c47)

-	Main math in ML is algebra. 
-	Humans do every day: learn, process language (listen), talk (speech), move (robotics), plan (optimize), see (vision).
-	Data Science: Produce insights 
-	Machine Learning: Produce Predictions
-	Artificial Intelligence: Produce actions
-	Humans process data from 5 senses, eyes, nose, ear, tongue, and then brain interprets data. 
-	Humans learns which decision leads to good and bad results – unsupervised learning. Parent teach child how to cycle is feeding data and child is learning by trial and error (fall stand and cycle) is example of supervised learning. 
-	In Math this trial and error is known as Gradient descent.

-	Machine learns from 3 things, Model, Parameters, Learners. Model is based on predictions from data, parameters are the signals and factors or variables that model uses. And learners are adjustments or tuning done on parameters for best fit

-	Step 1: Based on data everything starts with model, the predictions that ML will use. Called as Hypothesis
-	Step 2: ML model creates formula the relationship with data / variables. 
-	Step 3: It gives margin of error (Standard error) 
-	Step 4: Model adjusts according to margin of error (and system runs again! Based on previous learner) 
-	And this is how Machine learns till absolute precision (like child learns cycling): Method is gradient decent (boosting principle)

4.	Best way to Say Classification and Regression (don’t say class 0 and 1 and regg has continuous vars) - Classification: grouping of like objects based on a defined characteristic. Regression: dependent variable(s) associated with independent variable(s).

5. Supervised Learning (SML): (Human supervisor) (labelled data)

-	4 main processes in SML: Data preparation, Training, testing, Tuning
-	Data preparation: good engineer does 3 imp things, 1. Skewness (check visually) 2. Data distribution (follow normal distribution) 3. Mean/medium/mode 
-	Important concept 1 is Variance: measure of how sensitive the models is to new data.  
-	Important concept 2 is Bias: bias is errors from erroneous assumptions (predictions). Bias is difference between average expected results from different runs of the model and the true value. Bias is accuracy of our prediction. High bias means prediction will be inaccurate. 
-	UNDERFIT: low variance / high bias: Data is good but formula is bad (dumb model)
-	OVERFIT: high variance / low bias:  Data is bad (skew) 

<p align="Left"><img width=60% src=https://user-images.githubusercontent.com/44467789/73653604-8f8fab80-46af-11ea-8b06-6a44d14d64aa.png>
  
 <br>
  
  6.	Unsupervised Learning: (minimal Human involvement) (unlabelled data)
-	Mainly used in e-commerce for cross selling
-	So if you had a dataset that had a result that showed a bunch of diverse people (diversity defined as age, race, education, income, geographic area, etc.) and you knew how much money they were spending per month on products you would group said people according to how much they spent per month regardless of those other factors.
-	Next, you could sell them more products that other people in their same spending cluster had purchased. 

7.	In predictions don’t only focus in prediction results. Try and check what is the variance in the predicted results. Specially how you evaluate the prediction score. E.g there is 80% probability for person A and B to commit crime. But for A has variance of 40% and B has variance of 5% from mean. Then your views will change, and you’ll arrest person B first and may be put A on hold. 

8.	Stable variance > Accuracy 

9.	Linear models (linear regression / logistic regression) = stable variance 

10.	When to use non-linear models (like Random Forest) – 1. more features, 2. No direct relationship between vars. 3. Structure pheromone 

11.	Variance can be different for e.g size of company, 10 million and 20 billion, company both has significant different of variance in profit/loss. And hence may deviate the results (someone says it outliers).

12. Cross Validation:
-	A statistical technique to test machine learning model performance.
-	Steps: 1. Divide data into train and test 2. Train model 3. Test data for evaluation 4. Repeat steps 1 to 3 on different sets.
-	Helps to avoid over fitting
-	Method:
##### 1. Holdout: Simple 70:30 train and test dataset. Dis-adv prone to selection bias
##### 2. K-fold: e.g if k = 10, then data is split into 10 sub dataset, not one by one, train data on 9 sub-datasets and test on 1 sub-dataset.  Repeat 10 times with different combination of sub-datasets. Advantage, less prone to selection bias. Disadvantage very expensive. 
-	Repeated random sun-sampling: Similar to K-fold, but in this method, the sub-datasets are not equally sized. Dis-adv is that some points are never be selected by randomness. 


