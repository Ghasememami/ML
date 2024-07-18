# 📕 Mini project 1



## Question 1
### Introduction
This question contains the implementation of a linear classifier model training and evaluation process. The tasks involve generating a dataset, training the model, evaluating its performance, and visualizing the decision boundaries.

### Table of Contents
Task 1: Block Diagram of Training and Evaluation Process
Task 2: Dataset Generation and Visualization
Task 3: Training and Evaluating Linear Classifiers
Task 4: Decision Boundary Visualization
Task 5: Repeating the Process with Custom Dataset


### Task 1: Block Diagram of Training and Evaluation Process
Description
Create a block diagram illustrating the process of training and evaluating a linear classifier model. Explain the various components of the block diagram. Indicate which part of the block diagram changes when transitioning from binary classification to multi-class classification.

### Diagram
Insert Block Diagram Image Here

### Explanation
1- Data Collection: Collect and preprocess the data.
2- Feature Selection: Select relevant features for training the model.
3- Model Selection: Choose an appropriate linear classifier model.
4- Training: Train the model using the training dataset.
5- Evaluation: Evaluate the model using the testing dataset.
6- Prediction: Use the trained model to make predictions on new data.
7- Feedback Loop: Use evaluation metrics to tune the model and improve performance.
8- Multi-Class Classification
9- In multi-class classification, the model selection and training components need adjustments to handle multiple classes. This often involves using techniques like One-vs-Rest (OvR) or Softmax for multi-class support.

### Task 2: Dataset Generation and Visualization
Description
Generate a dataset with 1000 samples, 4 classes, and 3 features using sklearn.datasets. Visualize the dataset and discuss its complexity. Suggest ways to make the dataset more challenging.

### Task 3: Training and Evaluating Linear Classifiers
Description
Use at least two linear classifiers from sklearn.linear_model with appropriate hyperparameters to distinguish between the four classes in the dataset. Explain the process of selecting hyperparameters and display the training and evaluation accuracy.

Hyperparameter Selection
The hyperparameters for each classifier were chosen based on common practices and adjusted using cross-validation to optimize performance.

### Task 4: Decision Boundary Visualization
Description
Visualize the decision boundaries of the trained model along with the dataset samples. Highlight misclassified samples with different shapes and colors.


## Question 2
This questiom explores fault detection using the CWRU Bearing dataset. The CWRU Bearing dataset is widely used for diagnosing faults in bearings using machine learning techniques. This README provides an overview of the dataset, steps to preprocess the data, extract features, and build machine learning models for fault detection.

Dataset Overview
The CWRU Bearing dataset consists of vibration signals from bearings under different conditions:

Normal Condition (Normal_X): Data from bearings operating under normal conditions.
Fault Condition (IR007_X): Data from bearings with inner race faults (IR) in state 007.
Objectives
The main objective of this dataset is to classify the health status of bearings based on vibration signals. This helps in early detection of faults and preventive maintenance.

Steps to Form the Dataset
Step 1: Data Acquisition
Download data from the respective pages:
Normal Condition Data
Fault Condition Data
Step 2: Data Preprocessing
Separate M samples of length N from each class (M >= 100, N >= 200).
Formulate an M × N matrix for both classes along with their respective labels.
Step 3: Feature Extraction
Extract at least 8 features from the dataset using the formulas mentioned in Table 1:


| Feature            | Formula                                                   |
|--------------------|-----------------------------------------------------------|
| Standard Deviation | \( x_{std} = \sqrt{\frac{\sum_{i=1}^N (x_i - \bar{x})^2}{N}} \) |
| Peak               | \( x_p = \max |x_i| \)                                    |
| Skewness           | \( x_{ske} = \frac{1}{N} \sum_{i=1}^N \frac{(x_i - \bar{x})^3}{x_{std}^3} \) |
| Kurtosis           | \( x_{kur} = \frac{1}{N} \sum_{i=1}^N \frac{(x_i - \bar{x})^4}{x_{std}^4} \) |
| Mean               | \( \text{Mean} = \frac{1}{n} \sum_{i=1}^n x_i \)           |
| Absolute Mean      | \( \text{Abs Mean} = \frac{1}{n} \sum_{i=1}^n |x_i| \)     |
| Root Mean Square   | \( \text{RMS} = \sqrt{\frac{1}{n} \sum_{i=1}^n x_i^2} \)   |
| Peak to Peak       | \(\text{Maximum} - \text{Minimum}\)                       |


Step 4: Importance of Feature Extraction
Feature extraction reduces dimensionality and improves model accuracy by capturing essential information from raw data.

Step 5: Data Mixing and Splitting
Mix data if possible and divide it into reasonable training and evaluation ratios.

Step 6: Data Normalization
Normalize data to ensure consistent scaling of features. Choose one of the following normalization methods:

Min-Max Scaling: Scales data to a range of 0 to 1.
Standardization: Scales data to have a mean of 0 and variance of 1.
Conclusion
This repository aims to provide a comprehensive guide on using the CWRU Bearing dataset for fault detection. By following the steps outlined above, you can preprocess the dataset, extract relevant features, and normalize data for training machine learning models effectively.



You can find used dataset for question number 2 in link below.
### [Dataset 1](https://engineering.case.edu/bearingdatacenter/download-data-file)


## Question 3


You can find used dataset for question number 3 in link below.
### [Dataset 2](https://www.kaggle.com/datasets/budincsevity/szeged-weather/data)




