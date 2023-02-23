# tensorflowdemo

This script uses the MNIST dataset, which consists of 28x28 grayscale images of handwritten digits (0-9), and their corresponding labels. 
The image data is normalized by dividing by 255 to scale the pixel values between 0 and 1.

Then defined the model architecture using keras.Sequential(), which is a linear stack of layers. The input layer bascally "flattens" the 28x28 image data into a 1D array. 

Then compile the model using the Adam optimizer, sparse categorical cross-entropy loss function, and accuracy metric. 
The model is then trained on the training set using model.fit() for 10 epochs.

After training, I then evaluate the model on the test set using model.evaluate(), which returns the test loss and accuracy. 

Finally, it makes some predictions on the first 5 test images using model.predict() and prints the predicted labels, and true labels, for comparison.

This was interesting for me, but made me realize I've so much to learn!
