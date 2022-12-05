# Handwritten-digit-recognition-and-analyses-with-numpy

### This code implements a two-layer neural network for classifying images of handwritten digits. The steps are as follows:

1. Import the necessary libraries, including Pandas for data manipulation, Numpy for mathematical operations, Pickle for saving and loading model parameters, Keras for loading the MNIST dataset, and Matplotlib for data visualization.
2. Define several helper functions for the activation functions and other operations used in the neural network, such as ReLU (rectified linear unit), softmax, and one-hot encoding.
3. Initialize the model parameters (weights and biases) for the two layers of the neural network, using random values.
4. Perform the forward propagation step, where the input data (X) is passed through the network to compute the outputs of the two layers (A1 and A2).
5. Transform the ground truth labels (Y) into a one-hot encoded format, which is used in the backward propagation step to compute the gradients of the model parameters.
6. Perform the backward propagation step, where the gradients of the model parameters are computed using the output of the forward propagation step and the one-hot encoded labels.
7. Update the model parameters using the computed gradients and a specified learning rate (alpha).
8. Perform the gradient descent optimization algorithm for a specified number of iterations, and print the accuracy of the model on the training data at regular intervals.
9. Save the trained model parameters to a file for later use.
10. Load the trained model parameters from the file and use them to make predictions on the test dataset, and print the accuracy of the model on the test data.
