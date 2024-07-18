
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