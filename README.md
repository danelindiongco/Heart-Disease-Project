# Heart-Disease-Project

Heart disease is the number one cause of death globally, taking an estimated 17.9 million lives each year. This project aims to produce a classification model, using machine learning, to detect individuals with heart disease early.
The classification model is trained using a dataset with 11 features that can be used to predict the possibility of an individual with heart disease. The dataset can be found here:

https://www.kaggle.com/fedesoriano/heart-failure-prediction

#### The project is split into 4 steps:
1. Data Cleaning
2. Exploratory Data Analysis
3. Training the Machine Learning Models
4. Choosing and Evaluating the Classification Model

### Data Cleaning
This process involves cleaning the dataset to be able to conduct Exploratory Data Analysis and eventually Train the Machine Learning models. It involves the following steps:
- Remove Unnecessary Values or Columns
- Correct Datatypes
- Handle Missing Values
- Remove Outliers

### Exploratory Data Analysis
To explore the dataset before any modelling is done. Also spots any patterns and also any obvious errors in the data. The graphs also confirms that the results of the model are valid.

Here are the observations:
- As age increases in the dataset, the likelihood of having heart disease increases
- The proportion of Men with heart disease are greater than the proportion of Women with heart disease suggesting Men are more likely to have heart disease in this sample distribution
- A flat st slope is a strong indicator of the presence of heart disease
- Asymptomatic chest pain type is a strong indicator of the presence of heart disease
- Old peak (ST value), when greater than zero, is a strong indicator of the presence of heart disease

### Training the Machine Learning Models
This step first begins with preprocessing the data using one-hot encoding to transform categorical data into numerical features.

3 different models were trained using different Machine Learning algorithms. The goal was to identify the model with the highest effectiveness in spotting heart disease using the features of the dataset. The 3 algorithms used to train the model were Logistic Regression, Random Forest and SVM. The models were trained using Scikit-Learn, with Random Forest and SVM further optimised using GridSearch.


### Choosing and Evaluating the Classification Model
By analysing the accuracy, precision and recall figures of the 3 models, the Logistic Regression model was chosen. The model had an accuracy of 86% but more importantly, it had the highest recall with 86%. Recall takes into account false negatives which we have the least amount of tolerance for. This is because we would not want to turn away a patient with heart disease and leave it untreated as it can be dangerous or even fatal.

Evaluating the model's parameters ....
