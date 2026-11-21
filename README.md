# Deeplearning
Some Pytorch training projects and a simple agentic coding assistant
# How LLMs Work
The basic idea is that the nueral network predicts the next token but I havent trained one yet so I only have a broad concept in mind.
# My Current Understandings on Nueral Networks
A nueral network is a combination of different layers and there are multiple neurons on each layer. Assuming that the network consists of linear layers, each nueron starts off with randomly assigned weights and biases and the nuerons calculates the output by multipling the input with the weight and than adding the bias. This output than becomes the input for the next layer so a deeplearning network is fundementally many matrix calculations. The final output is than compared with a desired value via a loss function and the weights and biases are than adjusted accordingly using a optimizer. This process is repeated for many epochs until the loss reaches a designated amount.
# Some of my trained nueral networks
## Linear Regression
This nueral network only consists of a single nueron and one layer. Multiple dots are generated using the function y = 0.7x+0.3 and this data is split between a training set and testing set. The objective of this nueral network is to find out the relationship (weight and bias) between the x and y coordinates by interpreting the training data. 
## Binary classification
This nueral network is similar to the Linear regression one except that this one has multiple layers and multiple neurons on each layer
