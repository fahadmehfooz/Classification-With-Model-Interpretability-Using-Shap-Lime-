# Classification-With-Model-Interpretability-Using-Shap-Lime: Project Overview 

* We are provided with over a hundred variables describing attributes of life insurance applicants. 
* The task is to predict the "Response" variable for each Id in the test set. "Response" is an ordinal measure of risk that has 8 levels.
* Handling null values and the class imbalance.
* Built tree based models,logistic regression and stacked models.
* Doing a feature importance check for all the models. And then, interpreting the model, how every feature is pushing towards which target response.

## Resources and Tools Used
**Tools:** Jupyter Notebook

**Packages:** Pandas, NumPy, sklearn, Matplotlib, seaborn, shap, lime,mlxtend

## Data Used
**Data Source**: https://www.kaggle.com/fahadmehfoooz/classification-with-model-interpretation/data


## Data Wrangling And Visualizations
* Null values found, filling missing values using appropriate functions.
* Changing targer variable to lesser categories.
* Plotting heatmap to find the correlation between continuous features.
* Plotting displots, barplots and boxplots for the features.
* Once model has been built. Plotting feature importance plots and tree explainer plots using shap.
* Some of the visualizations are shown here:

![alt text](https://github.com/fahadmehfooz/Classification_With_Model_Interpretability/blob/master/images/Shap%20results.png)
![alt text](https://github.com/fahadmehfooz/Classification_With_Model_Interpretability/blob/master/images/lime.png)


## Model Building 

* I took a split on the data with training data as 80% and test data as 20%. 
* I took a split on the data with training data as 80% and test data as 20%. Built base level models for Logistic Regression, Random Forest,Gradient Boosting, Voting Classifier and stacked model.
* After building base model, I tuned the hyperparameters using grid search with 2 cross validations.
* Scoring metric used ROC-AUC.

## Metrics Used For Evaluation
* ROC-AUC
* Accuracy
* Log Loss
* F-score, precision and recall.

## Model performance

**Results:**

![alt text](https://github.com/fahadmehfooz/Classification_With_Model_Interpretability/blob/master/images/scores.png)


* Gradient Boosting, Voting Classifier and Stacked models are performing really well. Their train and test errors and also the roc scores and f scores are really close and good.
