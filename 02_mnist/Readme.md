# MNIST Neural Network (From Scratch)

This is a small project where I implemented a neural network from scratch using NumPy and trained it on the MNIST handwritten digits dataset. The goal was to understand what actually happens inside a neural network instead of relying on high-level libraries.

![Random MNIST sample](images/neural_network.png)

---

## What’s Inside

- MNIST dataset loading and normalization  
- Fully connected neural network built using NumPy  
- ReLU and Softmax activations  
- Categorical Cross-Entropy loss  
- Manual forward and backward propagation  
- Simple SGD-based training loop  

---

## Model Setup

- Input size: 784  
- Hidden layers: 128 → 64 (ReLU)  
- Output layer: 10 (Softmax)  

Loss: Categorical Cross-Entropy  
Optimizer: Stochastic Gradient Descent

---

## Current State

The model trains correctly and is able to predict handwritten digits.  
Training is done on the full dataset per epoch, and predictions are verified on random samples.

---

## Things to Improve

- Use mini-batch training instead of full-batch  
- Add a proper train/test split  
- Try a better optimizer (momentum or Adam)  
- Clean up inference for single-sample prediction  

---

## Final Note

This project is mainly about clarity and understanding.  
Accuracy can be improved, but the focus here was getting the fundamentals right.
