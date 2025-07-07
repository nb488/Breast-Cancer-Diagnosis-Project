Trial Log: 


7/3/2025

!!!this try: 

keep only worst and mean
discard radius + perimeter
discard compactness + concavity

based on correlation to y, heatmap and random forest importance features.

Result: linear model doing very well 96.5% on test data (+ not overfitting) at C=100, catboost doing the best of the ensembles still (~93%)


7/4/2025

!!!Try adding back the _se features, because I'm worried that I made the data to simple/general and that is why random forest and gradient boosting are overfitting.
keep discarding radius and perimeter
keep discarding compactness + concavity

Result: linear model whent down to 94% while catboost whent down to 93%. The rest on the ensembles are overfitting

Using just the mean data is consistently doing not as good, so I am going to drop this

!!!It looks like texture_mean and texture_worst are very correlated (heatmap)
Try and remove texture_mean (texture_worst is more correlated to the target value)
keep _se features out
discard radius + perimeter
discard compactness + concavity

Result: linear model at 95, catboost at 93


7/6/2025

!!!Move onto hyperparamter optimization

achieved good results in catboost and SVM RBF, specifically 94% and 96% without overfitting

!!!Made a shap plot and used the best model (Logistic regression) on the test data. To analyze next day


7/7/2025

!!! Added comments, cleaning up code and added some descriptions 