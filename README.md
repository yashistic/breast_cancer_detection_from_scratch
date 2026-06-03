# Breast Cancer Classification Using a Neural Network from Scratch

## Overview

This project started as an attempt to understand what actually happens inside a neural network instead of treating it as a black box.

Rather than using deep learning libraries such as TensorFlow or PyTorch, I implemented a feedforward neural network from scratch using NumPy. The goal was to learn how forward propagation, backpropagation, activation functions, and gradient descent work under the hood.

The model was trained to classify breast cancer tumors as either benign or malignant using diagnostic measurements from the Breast Cancer Wisconsin Dataset.

---

## Dataset

The project uses the Breast Cancer Wisconsin Dataset, which contains diagnostic features extracted from digitized images of breast mass samples.

* 569 total samples
* 30 numerical features
* Binary classification task

  * Benign (0)
  * Malignant (1)

---

## Neural Network Architecture

The network consists of:

* Input Layer: 30 features
* Hidden Layer 1: 16 neurons with ReLU activation
* Hidden Layer 2: 8 neurons with ReLU activation
* Output Layer: 1 neuron with Sigmoid activation

Architecture:

30 → 16 → 8 → 1

---

## Features Implemented

Everything was implemented manually using NumPy:

* Parameter initialization
* Forward propagation
* ReLU activation
* Sigmoid activation
* Backpropagation
* Gradient descent optimization
* Prediction pipeline
* Accuracy evaluation

No deep learning frameworks were used.

---

## Results

The model achieved approximately **92% test accuracy** on unseen data.

During experimentation, I observed a useful machine learning lesson: increasing the number of training iterations significantly improved training accuracy but eventually caused severe overfitting and poorer test performance. Reducing the training iterations led to much better generalization on unseen samples.

---

## What I Learned

This project helped me develop a deeper understanding of:

* How neural networks transform inputs through multiple layers
* How gradients are computed and propagated backward
* The role of activation functions such as ReLU and Sigmoid
* Gradient descent optimization
* The importance of evaluating on unseen test data
* The impact of overfitting on model performance

---

## Technologies Used

* Python
* NumPy
* Pandas

---

## Future Improvements

Some possible extensions to this project include:

* Mini-batch gradient descent
* Adam optimizer
* Learning rate scheduling
* Regularization techniques
* Training loss visualization
* Interactive deployment using Streamlit

---

## Author

Yash Mittal

Built as part of my journey to understand machine learning fundamentals by implementing core algorithms from scratch.
