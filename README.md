# Image-Classification-with-TensorFlow

Network Regularization (CNN)

Regularization techniques are useful in learning a generalizable solution and help in avoiding the overfitting.
For the Deep Neural Network regularization is generally achieved by using a dropout technique.
Dropout will be added to the training. We have to compare both the solutions with and without dropout regularization. Batch normalization layer and train the model with tf.train.GradientDescentOptimizer will be added. Recording the accuracy with and without dropout. Showing
with the accuracy plots the performance gain on the test dataset with and without dropout. Accuracy vs training per epochs for both the cases will be shown at the end.

# Adding Dropout into the Network

We will add a dropout layer to overcome the problem of overfitting to some extent. Dropout randomly turns off a fraction of neurons during the training process, reducing the dependency on the training set by some amount. How many fractions of neurons we want to turn off is decided by a hyperparameter, which can be tuned accordingly. This way, turning off some neurons will not allow the network to memorize the training data since not all the neurons will be active at the same time and the inactive neurons will not be able to learn anything.

So let's create, compile and train the network again but this time with dropout. And run it for 20 epochs with a batch size of 64.
