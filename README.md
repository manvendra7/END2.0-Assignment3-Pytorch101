# END2.0-Assignment3-Pytorch101


We already have the MNIST dataset and their corresponding labels. We generated 60000 random numbers between 0 and 9, stored that into data2 and added the label of the image y to create the new output label y2 which is the addition of image class and the random number.

The image data is represented as the tensor of (1,28,28) and the data2 is the tensor data representing the random number.



We have applied two methods to train our model to do the addition task -

Build a classifier model for both the task to predict the label for the image as well as to predict the addition of the image and the random number.


Passed the images through 8 convolution layers.

Changed the random numbers to one hot vector form.

Concatenate both the one hot vector from a random number and the output from the convolutional layer.

Passed it through fully connected 2 pre final layers.

In the output layer add two neurons one for image label and the other one for addition of image label and random number.

We have used crosentropy loss for both the output image labels as well as addition as we treated this as a classification problem.

Trained the model for 20 epochs passing and got the loss 0f 0.08



With the Second Approach we applied a classification model for the prediction of image labels and a regression model to perform the addition of labels and random numbers.



We passed the image through 2 convolution layers.

output from convolution operations was passed from 2 fully connected layers with 120 neurons and 60 neurons respectively and an output layer for predicting label of image.

We took the output1 stacked it with the random number and passed it through 2 fully connected layers to get the addition output.

Loss for regression

L2 loss is also known as mean squared error (MSE). L2 loss, as one can easily infer, is the mean of the squared differences between the predicted variable and the label variable.

Loss for classification

Cross-entropy

This approach did not work out well for us compared to the first approach.
