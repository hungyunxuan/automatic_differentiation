

# Neural Network Framework with Automatic Differentiation

This repository provides a simple neural network framework built from scratch with automatic differentiation capabilities. It includes essential components such as neurons, layers, and a multi-layer perceptron (MLP), allowing you to create and train custom neural network models.

## Features

- **Automatic Differentiation**: Efficiently compute gradients for optimization.
- **Neural Network Modules**:
  - **`MyNeuron`**: Represents a single neuron with optional nonlinearity (ReLU).
  - **`MyLayer`**: A layer consisting of multiple neurons.
  - **`MyMLP`**: A multi-layer perceptron supporting multiple layers.

## Installation

No installation is required beyond Python itself. Simply clone the repository:

```bash
git clone https://github.com/yourusername/your-repo.git
```
You can create and train neural networks using the provided classes. Here’s a basic example:

```
from your_module_name import MyMLP

# Create a neural network with 3 input neurons, one hidden layer of 4 neurons, and an output layer of 2 neurons
mlp = MyMLP(input_size=3, output_sizes=[4, 2])

# Example input vector
input_vector = [Variable(1.0), Variable(2.0), Variable(3.0)]

# Perform a forward pass
output = mlp(input_vector)

print("Output:", output)
```

## Components Overview

- **MyModule: Base class for all network components.
- **MyNeuron: Defines individual neurons with weights and optional activation functions.
- **MyLayer: A collection of neurons forming a single layer.
- **MyMLP: Multi-layer perceptron that supports stacking multiple layers.


Credits: https://github.com/karpathy/micrograd/blob/master/trace_graph.ipynb  
