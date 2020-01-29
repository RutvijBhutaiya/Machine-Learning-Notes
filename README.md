# Machine-Learning-Notes
#### Few notes on basic concepts of Machine Learning. 


1. Ensemble: Ensemble idea is to train multi model using same learning algorithm. Main cause of error are noise, bias and variance. Ensemble minimizes it. And it uses to stabilize the learning model. 

2. Bagging vs. Boosting: (https://quantdare.com/what-is-the-difference-between-bagging-and-boosting/)

- Bagging is also knwn as Bootstrap aggregation. 
- Based on training data set, both techniques create n classifier (random new datasets). 

- Bagging each model build independently. Like for example there are 10 new random datasets. So, the 10 models based on each data would be independent to each other. 

- Boosting each model build in sequence. Means model 1 build based on dataset 1. Then model 2 build based on model 1 (previous classifier success) but uses dataset 2. 

- Hence, in bagging, classifier is an average (regression) or max vote (classification). However, in boosting is based on weightage average. 
- Bagging is train and keep AND boosting is train and evaluate. 
- Boosting uses certain weights to next classification stage e.g. Adaboost, XGBoost.
- Bagging may solve overfitting problem. Boosting can increase overfitting. Because, Boosting gives more weights to good performance and removes bad performers from the model. 

3. 
