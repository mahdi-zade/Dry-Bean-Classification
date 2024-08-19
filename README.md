# Dry Bean Classification
<p align="center">
  <img width="1000" src="https://github.com/user-attachments/assets/bb1a2a85-3ba5-4759-874a-4fb096ee99ad">
</p>

## Aim
The aim of this repository is to start from scratch and build simple neural networks to classify bean images. at each step, the model and the parameters will be changed to check up the effect of each one the final result and hopefuly try achieving the best result in the end. This project is the perfect fit for anyone who is new to the field of machine learning and wants to have a better understanding of /neural network architecture.

## Dataset
You can access the dataset [here](https://archive.ics.uci.edu/dataset/602/dry+bean+dataset)
- Contains images of 13,611 grains of 7 different registered dry beans.
- The images were taken with a high-resolution camera.
- A total of 16 features; 12 dimensions and 4 shape forms, were obtained from the grains.
- This means there are 7 labels and 16 features.

## Part one: A two layer neural network
We will start with the simplest neural network which contains 1 hidden layer.
We will design and test a model with following traits, parameters, and techniques:
1. Feedforward neural network with one  hidden layer.
2. Activation function: ReLU.
3. Cost Function: cross entropy
4. Data Split: 70% for training and 30% for evaluation
5. Evaluation: Accuracy graph and loss function graph and also the confusion matrix.

You can access the colab notebook [here](https://colab.research.google.com/drive/1u9zS1-qVwK8sMGXzybIMF3BH9roumN7s?usp=sharing)

- Results: 0.6881 accuracy
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/f88bcb49-bfce-4fe0-81a6-3fb65c977cf8">
  </p>

  <p align="center">
    <img width="300" src="https://github.com/user-attachments/assets/1f830e93-8ef8-48cb-b8aa-fec3642905dd">
  </p>

## Part two: Normalizing the input data
Obtain classification results for normalized and unnormalized input data and discuss the results.
- Theoretically, having the inputs values be between zero and one, should significantly decrease the computation time and give better results. Let's test it.
- The changes made to the original code can be seen in the colab notebook.
- You can access the colab notebook [here](https://colab.research.google.com/drive/1wxbHO6VRS1BoKLn7-Ao2hrYrGLY85c41?usp=sharing)

- Results: 0.6881 accuracy
  <p align="center">
    <img width="500" src="https://github.com/user-attachments/assets/f88bcb49-bfce-4fe0-81a6-3fb65c977cf8">
  </p>

  <p align="center">
    <img width="300" src="https://github.com/user-attachments/assets/1f830e93-8ef8-48cb-b8aa-fec3642905dd">
  </p>


فقط اونجایی که گفته از scratch بزن نمیخواد با همین کتاب خونه ها آماده بزن

سوال اول شبکه عصبی mlp ساده است

سوال دوم convention ساده

------------------------------------------------------------

https://github.com/esssyjr/Multi-class-Classification-of-Dry-Beanss/blob/main/Multi-class-Classification-of-Dry-Beans.ipynb


https://ceur-ws.org/Vol-2951/paper3.pdf
