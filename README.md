# tensorflowdemo

In this script, we first load the MNIST dataset, which consists of 28x28 grayscale images of handwritten digits (0-9), and their corresponding labels. We then normalize the image data by dividing by 255 to scale the pixel values between 0 and 1.

Next, we define the model architecture using keras.Sequential(), which is a linear stack of layers. The input layer is a Flatten layer that flattens the 28x28 image data into a 1D array. This is followed by a Dense layer with 128 neurons and a ReLU activation function, and another Dense layer with 10 neurons (corresponding to the 10 possible digit labels) and a softmax activation function, which outputs a probability distribution over the possible labels.

We then compile the model using the Adam optimizer, sparse categorical cross-entropy loss function, and accuracy metric. We train the model on the training set using model.fit() for 10 epochs.

After training, we evaluate the model on the test set using model.evaluate(), which returns the test loss and accuracy. Finally, we make predictions on the first 5 test images using model.predict() and print the predicted labels and true labels for comparison.
