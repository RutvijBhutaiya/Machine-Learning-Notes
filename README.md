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

5.
