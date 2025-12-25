# MNIST Neural Network Project

This repository contains two implementations of a neural network trained on the MNIST handwritten digits dataset. The same problem is approached from two different perspectives: building everything from scratch to understand the fundamentals, and using TensorFlow/Keras to follow a modern, practical workflow.

<img src="../images/neural_network.png" width="500">

---

## Project Structure

- `mnist_scratch.ipynb`  
  Neural network implemented entirely from scratch using NumPy.

- `mnist_tensorflow/`  
  MNIST implementation using TensorFlow and `tf.keras`.

---

## 1. MNIST – From Scratch (NumPy)

This notebook focuses on understanding what actually happens inside a neural network without relying on high-level libraries.

### What’s Inside

- MNIST dataset loading and normalization  
- Fully connected neural network built using NumPy  
- ReLU and Softmax activation functions  
- Categorical Cross-Entropy loss  
- Manual forward and backward propagation  
- Simple SGD-based training loop  

### Model Setup

- Input size: 784  
- Hidden layers: 128 → 64 (ReLU)  
- Output layer: 10 (Softmax)  

Loss: Categorical Cross-Entropy  
Optimizer: Stochastic Gradient Descent

### Current State

The model trains correctly and can predict handwritten digits.  
Training is performed over the dataset per epoch, and predictions are tested on random samples.

### Possible Improvements

- Switch to mini-batch training  
- Add a proper train/test split  
- Experiment with better optimizers (Momentum, Adam)  
- Improve single-sample inference flow  

---

## 2. MNIST – TensorFlow (`tf.keras`)

This implementation demonstrates how the same problem is solved using industry-standard tools.

### What’s Inside

- `tf.data.Dataset` pipeline with `map`, `batch`, and `prefetch`  
- Model defined using `tf.keras.Model` / `Sequential`  
- Built-in Dense layers and activations  
- Automatic backpropagation and optimization  
- Training using `model.fit` with callbacks  

### Model Characteristics

- Clear separation between data pipeline and model  
- GPU/CPU optimized training  
- Cleaner, shorter, and more maintainable code  
- Easier experimentation and scaling  

---


## Final Note

This repository is not about achieving state-of-the-art accuracy.  
The focus is understanding neural networks deeply and then applying that understanding using modern frameworks.
