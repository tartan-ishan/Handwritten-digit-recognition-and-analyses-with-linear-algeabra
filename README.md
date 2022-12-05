# Handwritten-digit-recognition-and-analyses-with-numpy

The code is a simple implementation of a neural network in Python that implements a two-layer neural network for classification using the ReLU and softmax activation functions. 

‣It includes functions for initializing the network's parameters, performing forward and backward propagation, updating the parameters using gradient descent, and evaluating the performance of the model on a given dataset. The script can be used to train the neural network on the MNIST dataset and make predictions on new data.

‣The code starts by ***importing the required libraries***, including Pandas, Numpy, and Keras for data manipulation and machine learning. It then defines the ReLU activation function, its derivative, and the softmax function for classification, which are used in the forward propagation step of the model.

‣Next, the ***init_params*** function initializes the model parameters (weights and biases) for the two layers of the neural network using random values between -0.5 and 0.5. The ***forward_propagation*** function performs the forward pass through the network, computing the weighted sum and applying the ReLU activation function to the first layer, and the softmax function to the second layer.

‣The ***one_hot function*** converts the target labels (Y) into a one-hot encoded matrix, where each column represents a sample and the corresponding row indicates the class label. This is used in the backward propagation step, where the error is computed between the predicted output (A2) and the one-hot encoded labels.

‣The ***backward_propagation function*** computes the gradient of the error with respect to the model parameters, using the chain rule of differentiation. This is used in the ***update_params*** function, where the gradients are used to update the model parameters using the gradient descent optimization algorithm.

‣The ***get_predictions function*** extracts the predicted class labels from the output of the network (A2), by finding the indices of the maximum values in each column. The ***get_accuracy*** function compares the predicted labels with the true labels and computes the accuracy as the percentage of correct predictions.

‣Finally, the ***gradient_descent function*** ties all the previous functions together to train the neural network on the MNIST dataset, using the specified learning rate (alpha) and number of iterations. The trained model is then tested on the test set, and the accuracy is printed.
