# Deeplearning

Some Pytorch training projects and a simple agentic coding assistant.

# How LLMs Work

The basic idea is that the nueral network predicts the next token but I havent trained one yet so I only have a broad concept in mind.

# My Current Understandings on Nueral Networks

A nueral network is a combination of different layers and there are multiple neurons on each layer. Assuming that the network consists of linear layers, each nueron starts off with randomly assigned weights and biases and the nuerons calculates the output by multipling the input with the weight and than adding the bias. This output than becomes the input for the next layer so a deeplearning network is fundementally many matrix calculations. The final output is than compared with a desired value via a loss function and the weights and biases are than adjusted accordingly using a optimizer. This process is repeated for many epochs until the loss reaches a designated amount.

# Some of my trained nueral networks

## Basic Nueral Network Workflows
1. Prepare training and testing data
2. Pick loss function and optimizer
3. Build the training loop
4. Make predictions using the model
5. Evaluate the results
6. Improving the model

## Linear Regression
This nueral network only consists of a single nueron and one layer. Multiple dots are generated using the function y = 0.7x+0.3 and this data is split between a training set and testing set. The objective of this nueral network is to find out the relationship (weight and bias) between the x and y coordinates by interpreting the training data. 

## Binary classification
This nueral network is similar to the Linear regression one except that this one has multiple layers and multiple neurons on each layer. The trainning data is generated using a Circle Coordinate Plane formula but this data is generated twice. The objective of this nueral network is to classify the dots to see which circle they belong in. I also added 2 non-linear ReLU between the 3 linear layers to ensure that this model could find non-linear patterns.

## Multi-class classification
This model is similar to the Binary classification one but with more layers and more neurons on each layer to ensure that model could find the patterns.

# Agentic Coding Assistants (Simplified Version)

This Agentic coding assistant follows the following cycle

1. The user sends a prompt along with the system prompts to the agent.
2. The agent thinks and than choose a tool from the lists which includes reading and writing files, terminal commands, searching code, etc...
3. The context is updated everytime
4. Once the agent did not make any tool calls the agentic cycle breaks.
5. The agent would than spit out the results

# Issues encountered
1. Frequent tensor shape mismatches during training.
2. Model doesnt find the pattern properly(underfitting)
3. Adjustments to the learning rate, epochs, layers, neurons to achieve a lower loss.
4. The Agent would frequently lost track of its initial goals.
5. The Agent struggles to call the tools properly often sending incorrect parameters.
6. The Agent doesnt know how to interpret the tool outputs properly.
