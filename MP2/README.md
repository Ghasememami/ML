
# 📗 Mini project 2
These files are the solution of the second home work of the Machine Learning course.

## Question 1 

Classifying Points in a Triangle
This code implements a simple neural network to classify points within a triangle. The network utilizes a single neuron with different activation functions (ReLU and Sigmoid) to explore their impact on the classification task.
![alt text](1_6.png)


## Functionality:

### Data Generation: 2000 random data points are generated within a specified range.

### Network Architecture:
Each data point is represented by its x and y coordinates (2-dimensional input).
The network aims to classify points: 1 for points inside the triangle's shaded area, 0 for points outside.
A single neuron with adjustable weights and bias processes the input.

### Classification with Different Activation Functions:
ReLU (Rectified Linear Unit): y = max(0, z), where z is the weighted sum of inputs.
Sigmoid: y = 1 / (1 + exp(-z)), introducing a smooth S-shaped curve for activation.

#### Diagram of the model: 

![alt text](1_8.png)

### Visualization:
 The generated points are plotted with colors indicating their classification:
- Green: Points classified as "inside" (output 1)
- Red: Points classified as "outside" (output 0)
- Triangle outline for reference

### Experimentation:

This code allows you to experiment with both ReLU and Sigmoid activation functions and observe how they influence the classification boundary. You can easily modify the code to explore the impact of different network parameters (weights, bias) or even try more complex network architectures.

### RESULT :
![alt text](1_5.png)


## Question 2 


### Enhanced Bearing Fault Classification with Multi-Layer Perceptron
This project delves into improving fault classification accuracy on the Bearing CWRU dataset. It expands the available fault classes and leverages a Multi-Layer Perceptron (MLP) neural network for robust classification.

### Key Features:

#### Data Augmentation: 
 The dataset is enriched by incorporating additional fault classes from "X_6@007OR" in the "Fault Data in k,12" page, resulting in a total of four distinct fault categories (including the original two from Mini Project 1).
#### MLP Network Architecture:
 A versatile MLP network with two or more hidden layers is employed. Each layer comprises perceptron neurons equipped with activation functions (like ReLU) to introduce non-linearity.
#### Optimized Training Process:
 A meticulously chosen optimizer (e.g., Adam, SGD) guides weight updates during training. Additionally, a suitable loss function (e.g., Cross-entropy) measures the difference between predicted and actual labels, aiding the optimization process.

#### Comprehensive Evaluation:
 The trained model's performance is rigorously assessed on unseen testing data using metrics like accuracy, precision, recall, and F1-score for all fault classes. A confusion matrix provides a visual representation of classification performance, helping identify potential issues.

#### Detailed Analysis:
 The results are thoroughly analyzed, considering factors such as model complexity, optimizer choice, and loss function. This analysis sheds light on potential areas for improvement and furthers our understanding of MLP networks in fault classification tasks.

### Benefits:

Potentially superior fault classification accuracy compared to the baseline model in Mini Project 1.
Valuable insights into the effectiveness of MLPs for bearing fault diagnosis.
Guidance for future refinements, including model architecture adjustments, exploration of new optimizers, and data augmentation strategies.
Further Exploration:

This project encourages experimentation with different network configurations (number of layers, neuron count, activation functions) and optimization algorithms with their hyperparameters. Regularization techniques can also be investigated to enhance model generalization and prevent overfitting.

By incorporating these advancements, this project aims to elevate the performance of bearing fault classification tasks on the CWRU dataset.

### Result

![alt text](2_10.png)

#### Accuracy :

![alt text](2_11.png)