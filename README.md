# Residual Shortcut: Reproduce Degradation problem and solution
This repository is dedicated to exploring the degradation problem in deep neural networks and 
implementing the Residual Learning framework as proposed in the paper ["Deep Residual Learning for Image Recognition" by He et al](https://arxiv.org/pdf/1512.03385).


**Overview**


As neural networks become deeper, they suffer from **degradation problem**: accuracy saturates and then degrades rapidly.
This is not caused by overfitting as training error also increases with test error. This project implements:
1. Plain Networks: To observe the degradation problem where 50-layer netowork takes long time to fit or maybe overfit the `CIFAR dataset`.
2. Residual Networks (**ResNets**): To demonstrate how identity shortcut connections (F(x)+x) allow for deeper models to achieve lower training error.

# Respository contents
The project is implemented using **Jupyter Notebooks**:
- `degradation.ipynb`: Focuses on training "plain" stacked layers to visualize the optimization difficulties and the rise in training error as depth increases
- `residual.ipynb`: Implements the residual building blocks and shows how identity shortcuts address the degradation problem,
  allowing for successful training of deep architectures.
