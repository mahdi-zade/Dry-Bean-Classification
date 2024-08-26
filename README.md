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


## Part 1: A two layer neural network
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
  - ds
  - ds
  - ds
  - d 


## Part 2: The Effect of Weight Initialization
In part one, the weights where initialized to be zero, now we will initialze the weights to be normal distribution with mean zero and several values of standard deviation.
The values for std(standard deviation) were set to [0,0.5,1,1.5,2,5,10].
for each of the values of std, training is repeated for 5 times and 25 epochs each and the final accuracy is set to be the average of the 5 training iterations. the final result is a plot 
![image](https://github.com/user-attachments/assets/ac9897ba-d277-4c5e-ba25-87f2f9d470ad)
![image](https://github.com/user-attachments/assets/608357b3-a244-4956-b892-41257b76740c)
- Discussions: So far initialing weights to be a normal distribution with a mean zero and standard deviation 1 seems logical.


## Part 3: Normalizing the input features
Obtain classification results for normalized and unnormalized input data and discuss the results.
- Theoretically, having the inputs values be between zero and one, should significantly decrease the computation time and give better results. Let's test it.
- weights are initialized to be a normal distribution with a mean zero and standard deviation 1.
- You can access the colab notebook [here](https://colab.research.google.com/drive/1wxbHO6VRS1BoKLn7-Ao2hrYrGLY85c41?usp=sharing)

- Results:
- For unnormalized data based on previous part: Average Accuracy: 0.4186
- For normalized input features: accuracy = Average Accuracy: 0.2650

  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>

- Discussion:
- Normalizing data seems to have negatively affected the final accuracy.

## Part 4: Adding One more hidden layer
- Results:
- For unnormalized input features: Average Accuracy: 0.3598
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>
- For normalized input features: accuracy = Average Accuracy: 0.5143
- 
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>

- Discussion: Adding a new layer seems to have negatively affected the final accuracy but normalizing data gives the best accuracy for the model yet.

## Part 4: Adding One more hidden layer
- Results:
- For unnormalized input features: Average Accuracy: 0.3598
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>
- For normalized input features: accuracy = Average Accuracy: 0.5143
- 
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>

- Discussion: Adding a new layer seems to have negatively affected the final accuracy but normalizing data gives the best accuracy for the model yet.

## Part 4: Adding One more hidden layer
- Results:
- For unnormalized input features: Average Accuracy: 0.3598
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>
- For normalized input features: accuracy = Average Accuracy: 0.5143
- 
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>

- Discussion: Adding a new layer seems to have negatively affected the final accuracy but normalizing data gives the best accuracy for the model yet.

## Part 5: Changing model architecture to Gaussian RBF
- Results:
- For normalized input features: accuracy = Average Accuracy: 0.2517
- 
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/5e54dd63-a9a8-4dc9-b41c-928213d0c085">
  </p>

- Discussion: Adding a new layer seems to have negatively affected the final accuracy but normalizing data gives the best accuracy for the model yet.


## Part X: Adding Momentum
The adam optimizer doesn't have a setting to chage momentum so we switch to SGD optimizer.
Momentum with values of [0.0, 0.5, 0.9, 0.99] are implemented
- Results:
- For normalized input features and different values for momentum:
- 
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/bf88baee-b882-4508-9457-aa191ee3ad31">
  </p>

- Discussion: increasing momentum seems to negatively affect the final accuracy.



فقط اونجایی که گفته از scratch بزن نمیخواد با همین کتاب خونه ها آماده بزن

سوال اول شبکه عصبی mlp ساده است

سوال دوم convention ساده

------------------------------------------------------------

https://github.com/esssyjr/Multi-class-Classification-of-Dry-Beanss/blob/main/Multi-class-Classification-of-Dry-Beans.ipynb


https://ceur-ws.org/Vol-2951/paper3.pdf
------------------------------------
Give me the pytorch code for this:
We want to do the manual calculation of the training of a model with the following specification:
We have an image with three channels in dimensions of 6 x 6. After passing the image through a 3x3 convolution filter with a stride equal to 3, this image reaches the size of 2x2, and after passing through the non-linear sigmoid layer, it is converted into a linear layer and after passing through the last linear layer, it reaches the final output.
The three-channel input image needs to be initialized pixel by pixel in the beginning, also the convolution filter needs to be specified. The bias values ​​in the convolution and linear layer are equal to zero, and the values ​​of the linear layer weights are equal to [2,1,1,-1]. The optimal output of this input is equal to -1.
Consider the cost function as the square error and perform one step of the training with the learning algorithm of SGD and the learning rate of 0.1.
