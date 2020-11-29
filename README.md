# Titanic Dataset Prediction

This notebook was created mainly to show the influence of feature selection and principal component analysis (PCA) on a dataset.

## Dataset

The data used in this study is the Titanic Survivors Dataset obtained from [Kaggle](https://www.kaggle.com/c/titanic).

## The Analysis

### Import Data

Load data into a pandas dataframe.

### Engineer Features

Drop useless features and reformat the existing ones in such a way to avoid overfitting.

### Encode Data

Transform non-numerical features to numerical, making out data more flexible for the machine learning algorithms.

### Machine Learning

#### Split Data to Train/Test Sets

Split data into train and test data sets and use cross validation.

#### Evaluate Algorithms

Test and evaluate 5 algorithms:

1. Naive Bayes
2. Support Vector Machines
3. K Nearest Neighbors
4. Random Forest
5. AdaBoost

#### Validate

Measure the effectiveness of the algorithms with `KFold`. Compare the algorithms based on accuracy score and training time.

#### Influence of Feature Selection & PCA

Investigate if Feature Selection and PCA can improve the performance of Adaboost. Plot the results to depict the comparison of the dimensionality reduction techniques.

#### Tune

Optimise the hyperparameters with `GridSearchCV`. Evaluate with multiple metrics such as accuracy, precision, and recall.

#### Predict the Actual Test Data

Make the predictions and export them to a csv file.

## Credits

Most of the preprocessing code such as data cleaning, encoding and transformation was adapted from the [Scikit-Learn ML from Start to Finish](https://www.kaggle.com/jeffd23/scikit-learn-ml-from-start-to-finish) work by [Jeff Delaney](https://www.kaggle.com/jeffd23).
