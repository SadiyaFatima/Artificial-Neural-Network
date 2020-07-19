# Artificial-Neural-Network
What is a neural network?

Neural networks form the base of deep learning, which is a subfield of machine learning, where the structure of the human brain inspires the algorithms. Neural networks take input data, train themselves to recognize patterns found in the data, and then predict the output for a new set of similar data. Therefore, a neural network can be thought of as the functional unit of deep learning, which mimics the behavior of the human brain to solve complex data-driven problems.
The first thing that comes to our mind when we think of “neural networks” is biology, and indeed, neural nets are inspired by our brains.

What is an Artificial Neural Network?

Simply put, an ANN represents interconnected input and output units in which each connection has an associated weight. During the learning phase, the network learns by adjusting these weights in order to be able to predict the correct class for input data.We assign weights to different values and predict the output from them. However, in this case, we do not know the associated weight with each input, so we make an algorithm that will calculate the weights associated with them by processing lots of input data.

The original goal of the ANN approach was to solve problems in the same way that a human brain would. But over time, attention moved to performing specific tasks, leading to deviations from biology. ANNs have been used on a variety of tasks, including computer vision, speech recognition, machine translation, social network filtering, playing board and video games, medical diagnosis, and even in activities that have traditionally been considered as reserved to humans, like painting.

Components of ANNs:
1. Neurons
2. Connections and weights
3. Propagation function

Steps involved in the implementation of a neural network:
A neural network executes in 2 steps :
1. Feedforward:
On a feedforward neural network, we have a set of input features and some random weights. Notice that in this case, we are taking random weights that we will optimize using backward propagation.
2. Backpropagation:
During backpropagation, we calculate the error between predicted output and target output and then use an algorithm (gradient descent) to update the weight values.

Summarizing an Artificial Neural Network:

Take inputs

Add bias (if required)

Assign random weights to input features

Run the code for training.

Find the error in prediction.

Update the weight by gradient descent algorithm.

Repeat the training phase with updated weights.

Make predictions.

Key advantages of neural Networks:
ANNs have some key advantages that make them most suitable for certain problems and situations:
1. ANNs have the ability to learn and model non-linear and complex relationships, which is really important because in real-life, many of the relationships between inputs and outputs are non-linear as well as complex.
2. ANNs can generalize — After learning from the initial inputs and their relationships, it can infer unseen relationships on unseen data as well, thus making the model generalize and predict on unseen data.
3. Unlike many other prediction techniques, ANN does not impose any restrictions on the input variables (like how they should be distributed). Additionally, many studies have shown that ANNs can better model heteroskedasticity i.e. data with high volatility and non-constant variance, given its ability to learn hidden relationships in the data without imposing any fixed relationships in the data. This is something very useful in financial time series forecasting (e.g. stock prices) where data volatility is very high.


ANNs, due to some of its wonderful properties have many applications:

a. Classification of data:
Based on a set of data, our trained neural network predicts whether it is a dog or a cat?

b. Anomaly detection:
Given the details about transactions of a person, it can say that whether the transaction is fraud or not.

c. Speech recognition:
We can train our neural network to recognize speech patterns. Example: Siri, Alexa, Google assistant.

d. Audio generation:
Given the inputs as audio files, it can generate new music based on various factors like genre, singer, and others.

e. Time series analysis:
A well trained neural network can predict the stock price.

f. Spell checking:
We can train a neural network that detects misspelled spellings and can also suggest a similar meaning for words. Example: Grammarly

g. Character recognition:
A well trained neural network can detect handwritten characters.

h. Machine translation:
We can develop a neural network that translates one language into another language.

i. Image processing:
We can train a neural network to process an image and extract pieces of information from it.


About The project

Aim: The main aim of this proect is to help deploy a Python module that can be downloaded by uers via pip to create neural networks.

Implementation of a Neural Network In Python:

Import Required libraries:
First, we are going to import Python libraries. We are using NumPy for the calculations.

Assign Input values:
Next, we are going to take input values for which we want to train our neural network. Here we can see that we have taken two input features. In actual data sets, the value of the input features is mostly high.

Target Output:
For the input features, we want to have a specific output for specific input features. It is called the target output. We are going to train the model that gives us the target output for our input features.

Assign the Weights:
Next, we are going to assign random weights to the input features. Note that our model is going to modify these weight values to be optimum. At this point, we are taking these values randomly. Here we have two input features, so we are going to take two weight values.

Adding Bias Values and Assigning a Learning Rate:
Now here we are going to add the bias value. The value of bias = 1. However, the weight assigned to it is random at first, and our model will optimize it for our target output.
The other parameter is called the learning rate(LR). We are going to use the learning rate in a gradient descent algorithm to update the weight values. Generally, we keep the learning rate as low as possible so that we can achieve a minimum error rate.

Applying a Sigmoid Function:
Once we have our weight values and input features, we are going to send it to the main function that predicts the output. Now notice that our input features and weight values can be anything, but here we want to classify data, so we need the output between 0 and 1. For such, we are going to a sigmoid function.

Derivative of sigmoid function:
In gradient descent algorithm we are going to need the derivative of the sigmoid function.

Mathematics involved:

Calculate the dot product between inputs and weights Pass the result from step 1 through an activation function The result from Step 1 can be a set of any values. However, in our output we have the values in the form of 1 and 0. We want our output to be in the same format. To do so we need an activation function, which squashes input values between 1 and 0. One such activation function is the sigmoid function. Back Propagation We start by letting the network make random predictions about the output. We then compare the predicted output of the neural network with the actual output. Next, we fine-tune our weights and the bias in such a manner that our predicted output becomes closer to the actual output, which is basically known as "training the neural network". Calculating the cost Minimizing the cost

Contribution Guidlines:
This document provides a set of best practices for open source contributions - bug reports, code submissions / pull requests, etc.
