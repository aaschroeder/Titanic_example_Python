# Titanic_example

This repository contains files I created, using Python 2 and Jupyter Notebook, to predict survivors of the sinking of the Titanic (https://www.kaggle.com/c/titanic). The datasets required to run the file are included. There are seven scripts, each of which appears in the three following formats:

* .ipynb - Python Notebook file, which includes some very basic commenting and markdown formatting
* .html  - HTML outbook of Python notebook
* .py    - Raw Python script, without markdown coding

The seven scripts are as follows:

* Titanic_data_exploration_MASTER - Inputs training data, performs some basic feature preprocessing that will be used among all algorithms, and outputs a cleaned dataset. It then uses the execfile() command to call and execute the other scripts
* Final_setup_Random_Forest - Performs Random Forest algorithm, scanning across parameters in a forward-searching order to determine a high-quality fit
* Final_setup_GBoost - Performs Gradient Boosting Algorithm, scanning across parameters in a forward-searching order to determine a high-quality fit (As an aside, there are few moments that made me wish I used a Mac as much as trying to install XGBoost on a Windows system)
* Final_setup_SVM - Implements a Support Vector Machine, after creation of additional interaction variables from cleaned dataset. Uses the pipeline feature in Python to streamline code
* Final_setup_Logit - Implements Logit Classifier, in a manner similar to that of the SVM
* Final_setup_NB - Implements Naive Bayes Classifier
* Final_ensemble - Inputs predictions from the 5 base learning algorithms on an extra test set (extracted from the initial input training set), implements a Gradient Boosting Classifier on these predictions, and uses the results to produce a final prediction for the test set submitted to Kaggle.
