# :dart: Scoring Model
Use historical loan application data to predict whether or not an applicant will be able to repay a loan.

**Expected output**: a probability of default prediction, between 0 and 1.

# :card_index_dividers: Dataset
The dataset is provided by [Home Credit](https://www.kaggle.com/c/home-credit-default-risk)

# :scroll: Tasks
- :heavy_check_mark: Exploratory Data Analysis (EDA);
- :heavy_check_mark: Data cleaning;
- :heavy_check_mark: Feature engineering;
- :heavy_check_mark: Imbalanced classes management;
- :heavy_check_mark: Model training: Naïve Bayes, Logistic Regression, Stochastic Gradient Descent, Random Forest, LightGBM
- :heavy_check_mark: Model evaluation: AUC (Area Under the Curve), Recall, F1-Score
- :heavy_check_mark: Hyperparameters optimization;
- :heavy_check_mark: Evaluation of variable importance with SHAP (Shapley Additive exPlanations).

## Distribution of the classes
<img src=".\pictures\imbalanced_classes_distribution.png">

## Performance of lightGBM
<img src=".\pictures\roc_auc_lightgbm.png">

## Global explanation with SHAP
<img src=".\pictures\shap_global_explanation.png">

# :computer: Dependencies
scikit-learn, LightGBM, SHAP

# :pushpin: References 
- [Start here a gentle introduction - Will Koehrsen on Kaggle](https://www.kaggle.com/willkoehrsen/start-here-a-gentle-introduction/notebook)
- [Collection of useful functions - Ann Antonova on Kaggle](https://www.kaggle.com/aantonova/collection-of-useful-functions-and-simple-baseline)
- [Introduction to Imbalanced Classification - Jason Brownlee (machinelearningmastery.com)](https://machinelearningmastery.com/what-is-imbalanced-classification/)
- [Reduce memory usage on large datasets with datatype conversion](https://www.kaggle.com/c/champs-scalar-coupling/discussion/96655)
- Baseline: [scikit-learn - Naive Bayes (Gaussian)](https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html)
- Linear models: [scikit-learn - Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html); [scikit-learn - Stochastic Gradient Descent (SGD)](https://scikit-learn.org/stable/modules/sgd.html)
- Non Linear models : [Random Forest Classifier (ensemble method)](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html); [LightGBM (Gradient Boosting Machine) documentation](https://lightgbm.readthedocs.io/en/latest/index.html)
- [Cross-validation: evaluating estimator performance](https://scikit-learn.org/stable/modules/cross_validation.html); [cross_validate](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_validate.html)
- Evaluation metrics : [Evaluation of models with scikit-learn](https://scikit-learn.org/stable/modules/model_evaluation.html)
- [Tuning the hyperparameters of an estimator](https://scikit-learn.org/stable/modules/grid_search.html); [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)
- [Interpretable Machine Learning with SHAP](https://shap.readthedocs.io/en/latest/index.html)

# :arrow_forward: Further reading
- [Threshold moving for Imbalanced Classification - Jason Brownlee (machinelearningmastery.com)](https://machinelearningmastery.com/threshold-moving-for-imbalanced-classification/)
- [Imbalanced Data in NLP and Computer Vision - Analytics Vidhya](https://www.analyticsvidhya.com/blog/2020/11/handling-imbalanced-data-machine-learning-computer-vision-and-nlp/)
- [Bayesian Optimization- Jason Brownlee (machinelearningmastery.com)](https://machinelearningmastery.com/what-is-bayesian-optimization/)