# Text Classification

Sample Jupyter Notebooks for Tensorflow Models used to classify text

## Current Notebooks

1. Multi Label Text Classification
2. Binary Classification for Fake News Detection

### text_classification_RELU.ipynb

This notebook uses a custom multi layer perceptron model on the news20 category dataset 
already present in scikit.

Currently classifies under 4 categories. Further categories can be added and trained upon by adding to global variables in notebook

Activation function :RELU
Loss function : Softmax Cross Entropy
Optimizer: Adam Optimizer

Current accuracy is 81% on 70-30 split

### bag_of_perceptron.ipynb

This notebook uses a custom tensorflow estimator on the DBPedia dataset.
This has no hidden layer . Only single forward feed input layer

Activation function : Not required since single layer
Loss function : Softmax Cross Entropy
Optimizer: Adam Optimizer

Current accuracy is 88% on 70-30 split

Query sentences can be modified in queries.txt and thereafter can be inferred

### multi_layered_perceptron.ipynb

This notebook uses a custom tensorflow estimator on the DBPedia dataset.
This is one hidden layer of embedded word2vec encodings

Activation function : Softmax Classifier with RELU
Loss function : Softmax Cross Entropy
Optimizer: Adam Optimizer

Current accuracy is 92% on 70-30 split

Query sentences can be modified in queries.txt and thereafter can be inferred

### fake_news_perceptron.ipynb

This notebook uses a premade tensorflow estimator on the Kaggle Fake news Dataset.

Following estimator functions have been added:
1. Linear Estimator : Acc - 88% ROC - 88%
2. DNNEstimator: Acc - 91% ROC - 95%
3. DNNLinearClassifierEstimator Acc - 95% ROC - 95%

Activation function : RELU
Loss function : Softmax Cross Entropy
Optimizer: Adam Optimizer

Sample query sentence has been added in the notebook which can be tweaked