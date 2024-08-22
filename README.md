# KAN-v1: Kolmogorov Arnold Neural Network Tutorial

This repository provides a tutorial and implementation of the Kolmogorov Arnold Neural Network (KAN), a specialized type of neural network leveraging B-splines and custom linear layers. This guide covers how to set up, train, and evaluate the KAN model on the MNIST dataset.

## Overview

The KAN model integrates B-spline basis functions within neural network layers to create a flexible and powerful architecture for various tasks. This repository includes code for defining the KAN model, training it on the MNIST dataset, and evaluating its performance.

## Features

- Custom KAN model with B-spline basis functions
- Training and evaluation on MNIST dataset
- Use of advanced optimization techniques and learning rate scheduling
- Detailed documentation and tutorial for easy understanding and modification

## Requirements

To run the code, you will need Python and the following libraries:

- `torch` (PyTorch)
- `torchvision`
- `tqdm`

Code Explanation
KAN Model Definition
The KAN class implements the Kolmogorov Arnold Neural Network, which consists of several KANLinear layers. Each layer integrates B-splines for flexible and smooth interpolation.

Key Components:

KANLinear: A custom linear layer utilizing B-splines for transformations.
KAN: A sequential model composed of multiple KANLinear layers.
Training and Evaluation
The training script performs the following steps:

Data Loading: Loads and preprocesses the MNIST dataset.
Model Initialization: Sets up the KAN model, optimizer, and learning rate scheduler.
Training Loop: Trains the model for a specified number of epochs and updates learning rates.
Validation: Evaluates the model’s performance on a validation set.
Contributing
Feel free to submit issues or pull requests if you find bugs or have suggestions for improvements. Please follow the standard GitHub contribution guidelines.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
PyTorch and torchvision libraries for providing the framework and datasets.
The original authors and contributors of the Kolmogorov Arnold Neural Network concept. (Read more:https://arxiv.org/abs/2404.19756#)
