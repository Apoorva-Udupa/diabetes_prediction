
# Diabetes Prediction

View this project [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Lc47x2eHPQkzAZhDxdGmp0FMXJkE6uhB?usp=sharing)

## About
Diabetes is a chronic illness affecting many people and is characterized by the presence of high blood sugar levels. Early detection is important since diabetes detected in early stages can be controlled by lifestyle changes and/or minimal medication. Diabetes prediction serves as a useful reference for doctors because they can order further tests to detect diabetes early. 

## Dataset
In this project, we are going to train the model to predict whether the patient has diabetes or not. To train the model the dataset used is PIMA Indian Dataset. This dataset describes the medical records for Pima Indians
and whether or not each patient will have an onset of diabetes within next 10-20 years.

*Fields description of the dataset is as follows:*

- preg = Number of times pregnant

- plas = Plasma glucose concentration a 2 hours in an oral glucose tolerance test

- pres = Diastolic blood pressure (mm Hg)

- skin = Triceps skin fold thickness (mm)

- test = 2-Hour serum insulin (mu U/ml)

- mass = Body mass index (weight in kg/(height in m)^2)

- pedi = Diabetes pedigree function

- age = Age (years)

- class = Class variable (1:tested positive for diabetes, 0: tested negative for diabetes)

## Statistical Model Used 

The model used for diabetes prediction is **Support Vector Machine**.  SVMs are one of the most robust prediction methods, being based on statistical learning frameworks or VC theory. Given a set of training examples, each marked as belonging to one of two categories, an SVM training algorithm builds a model that assigns new examples to one category or the other, making it a non-probabilistic binary linear classifier. SVM maps training examples to points in space so as to maximise the width of the gap between the two categories. New examples are then mapped into that same space and predicted to belong to a category based on which side of the gap they fall.


## Installation of libraries for this project

- **Numpy** - for array computation

```bash
  pip install numpy

```
- **Pandas** - for data manipulation in csv files
```bash
  pip install pandas
```
- **Scikit-Learn** - for importing statistical model like Linear SVM
```bash
  pip install scikit-learn
```

## How it Works?
![work_flow](https://github.com/ChandanaGiridhar/diabetes_prediction/blob/main/work_flow.png)

After installing the dependencies, the dataset is loaded from the csv file. Before training the model it is necessary to perform data preprocessing. After preprocessing of the data, the dataset is grouped for training and testing the model. The training dataset is used to train the linear SVM. The trained model is then used for testing on the test dataset. Using the Accuracy score (from Scikit-learn package) we can determine the accuracy of the trained model and tested model and the accuracy scores are compared.


## Acknowledgements

 - [PIMA Dataset](https://www.kaggle.com/datasets/kumargh/pimaindiansdiabetescsv)
 - [Diabetes Prediction](https://www.sisense.com/blog/diabetes-prediction-using-support-vector-machines/)
 - [SVM for diabetes Prediction](https://www.youtube.com/watch?v=xUE7SjVx9bQ&list=PLfFghEzKVmjvuSA67LszN1dZ-Dd_pkus6&index=2)
