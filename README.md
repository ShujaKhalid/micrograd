# Simple Neural Network Implementation

This repository contains a basic implementation of a neural network, including classes for individual neurons, layers, and a multilayer perceptron (MLP).

## Components

- `Neuron`: A single neuron with `n` inputs. It computes the weighted sum of inputs and applies a ReLU activation function.

- `Layer`: A layer of neurons. Each neuron in the layer expects inputs from a single, separate input vector.

- `MLP`: A multilayer perceptron consisting of multiple layers of neurons, where the output of one layer is the input to the next.

## Usage

To use this neural network, create an instance of the `MLP` class with the desired input dimension and a list indicating the number of neurons per layer. Then, pass an input through the network by calling the instance with an input vector.

```python
from your_module import MLP

# Define the MLP structure
input_dim = 5
neurons_per_layer = [10, 10, 5]  # Example: 3 layers with 10, 10, and 5 neurons
mlp = MLP(input_dim, neurons_per_layer)

# Pass an input vector
input_vector = [Value(0.5), Value(0.1), Value(-0.2), Value(0.4), Value(0.9)]
output = mlp(input_vector)
