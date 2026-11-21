# Deep Learning

Some PyTorch training projects and a simple agentic coding assistant.

# How LLMs Work

The basic idea is that a neural network predicts the next token, but I haven't trained one yet, so I only have a broad concept in mind.

# My Current Understanding of Neural Networks

A neural network is a combination of different layers, with multiple neurons in each layer. Assuming that the network consists of linear layers, each neuron starts off with randomly assigned weights and a bias. The neuron calculates its output by multiplying the inputs by their weights and then adding the bias. This output then becomes the input for the next layer, so a deep learning network fundamentally involves many matrix calculations. The final output is then compared with a desired value using a loss function, and the weights and biases are adjusted accordingly using an optimizer. This process is repeated for many epochs until the loss reaches a desired level.

# Some of My Trained Neural Networks

## Basic Neural Network Workflow

1. Prepare training and testing data.
2. Pick a loss function and optimizer.
3. Build the training loop.
4. Make predictions using the model.
5. Evaluate the results.
6. Improve the model.

## Linear Regression

This neural network consists of a single neuron and one layer. Multiple dots are generated using the function y = 0.7x + 0.3, and this data is split into a training set and a testing set. The objective of this neural network is to find the relationship (weight and bias) between the x and y coordinates by learning from the training data.

## Binary Classification

This neural network is similar to the linear regression one, except that it has multiple layers and multiple neurons in each layer. The training data is generated as two circles on a coordinate plane. The objective of this neural network is to classify the dots according to which circle they belong to. I also added two non-linear ReLU functions between the three linear layers so that the model could find non-linear patterns.

## Multi-class Classification

This model is similar to the binary classification one, but with more layers and more neurons in each layer so that the model could find the patterns.

# Agentic Coding Assistant (Simplified Version)

This agentic coding assistant follows this cycle:

1. The user sends a prompt to the agent, along with the system prompts.
2. The agent thinks and then chooses a tool from the list, which includes tools for reading and writing files, running terminal commands, searching code, and so on.
3. The context is updated each time.
4. Once the agent stops making tool calls, the agentic cycle ends.
5. The agent then outputs the results.

# Issues Encountered

1. Frequent tensor shape mismatches during training.
2. The model doesn't find the pattern properly (underfitting).
3. Adjusting the learning rate, number of epochs, layers, and neurons to achieve a lower loss.
4. The agent frequently lost track of its initial goals.
5. The agent struggles to call tools properly, often sending incorrect parameters.
6. The agent doesn't know how to interpret tool outputs properly.

# References
1. Some of the projects are based on https://www.learnpytorch.io
2. The simple coding agent is based on https://www.heyuan110.com/zh/posts/ai/2026-03-07-build-ai-agent-python/
