# Dry Bean Classification
<p align="center">
  <img width="1000" src="https://github.com/user-attachments/assets/bb1a2a85-3ba5-4759-874a-4fb096ee99ad">
</p>

## Aim
The aim of this repository is to start from scratch and build a simple neural network to automatically classify bean species. This project is the perfect fit for anyone who is new to the field of deep learning and wants to have a better understanding of neural network architecture. The implementation is done via [pytorch library](https://pytorch.org/docs/stable/index.html) which is an optimized tensor library for deep learning using GPUs and CPUs.

## Dataset
You can access the dataset [here](https://archive.ics.uci.edu/dataset/602/dry+bean+dataset)
- Contains images of 13,611 grains of 7 different registered dry beans.
- A total of 16 features; 12 dimensions and 4 shape forms, were obtained from the grains.
- This means there are 7 labels and 16 features.
- The images were taken with a high-resolution camera.


## Part 1: A Two Layer Neural Network
We will design and test a model with following traits, parameters, and techniques:
1. Preprocessing: Standard scaling each of the 16 features.
2. Data Split: 70% for training and 30% for testing
3. Feedforward neural network with one hidden layer.
4. The input layer has 16 inputs and 32 outputs and is a fully connected neural network
6. The hidden layer has 32 inputs and 7 outputs(7 final classes) and is a fully connected neural network
7. Initial Weights: normal distribution
8. Activation function: ReLU.
9. Cost Function: cross entropy
10. 50 epochs

You can access the colab notebook [here](https://colab.research.google.com/drive/1CopOg6KXu9KKkUqXwShRra7T7AIvpV-E?usp=sharing)

- Average Result Across 5 Repetitions:
  - Average Training Loss: 0.1819
  - Average Training Accuracy: 0.9316
  - Average Test Loss: 0.1812
  - Average Test Accuracy: 0.9323


## Part 2: A Three Layer Neural Network
I'ts the exact same methods and techniques used in the last part, only with a difference of a new hidden layer added to the neural network architecture.

1. Preprocessing: Standard scaling each of the 16 features.
2. Data Split: 70% for training and 30% for testing
3. Feedforward neural network with one hidden layer.
4. The input layer has 16 inputs and 32 outputs and is a fully connected neural network
5. The first hidden layer has 32 inputs and 16 outputs and is a fully connected neural network
6. Activation function: ReLU.
7. The second hidden layer has 16 inputs and 7 outputs(7 final classes) and is a fully connected neural network
8. Activation function: Sigmoid.
9. Initial Weights: normal distribution
10. Cost Function: cross entropy
11. 50 epochs

You can access the colab notebook [here](https://colab.research.google.com/drive/1CopOg6KXu9KKkUqXwShRra7T7AIvpV-E?usp=sharing)

- Average Result Across 5 Repetitions:
  - Average Training Loss: 0.1784
  - Average Training Accuracy: 0.9334
  - Average Test Loss: 0.1842
  - Average Test Accuracy: 0.9332

- The three layer neural network yields a slightly better result.


